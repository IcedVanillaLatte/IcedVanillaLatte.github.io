---
title: "Hashcat 실습"
date: 2024-08-06 19:15:00 +0900
categories: [ETC]
tags: [hash, hashcat]
toc: true
toc_sticky: true
published: false
---

- 참고 사이트
	- [https://jekyllrb.com/docs/posts/](https://johyungen.tistory.com/261)
	- [<https://mmistakes.github.io/minimal-mistakes/docs/posts/>](https://github.com/initstring/passphrase-wordlist)


## 1. Hash 값

일반적인 리눅스 시스템에서 사용자 계정의 패스워드 값은 여기에서 확인할 수 있다.
```
$ sudo cat /etc/shadow
```

## 2. /etc/shadow 파일 형식
/etc/shadow 파일의 각 줄은 콜론(:)으로 구분된 여러 필드로 구성되어 있습니다. 일반적으로 각 줄은 다음과 같은 형식을 따릅니다:

```
username:password_hash:last_changed:min_age:max_age:warn:inactive:expire:reserved
```
여기서 주요 필드에 대한 설명은 다음과 같습니다:

- username: 사용자 계정 이름
- password_hash: 해시된 비밀번호. 이 필드가 해시된 비밀번호를 저장하는 부분입니다.
- last_changed: 마지막으로 비밀번호가 변경된 날짜(일수 기준, 1970-01-01 이후)
- min_age: 비밀번호 최소 사용 기간(일수)
- max_age: 비밀번호 최대 사용 기간(일수)
- warn: 비밀번호 만료 경고 기간(일수)
- inactive: 비활성화 기간(일수)
- expire: 계정 만료 날짜(일수 기준, 1970-01-01 이후)
- reserved: 예약 필드(미사용)

## 3. 비밀번호 해시 필드
password_hash 필드는 사용자 비밀번호를 해시하여 저장합니다. 이 필드는 보통 $id$salt$hashed 형식을 따릅니다:

- $id: 해시 알고리즘을 나타내는 식별자
  - $1$: MD5 해시 알고리즘
  - $2a$ 또는 $2b$: Blowfish 해시 알고리즘
  - $5$: SHA-256 해시 알고리즘
  - $6$: SHA-512 해시 알고리즘
- salt: 비밀번호 해시에 사용된 솔트 값. 솔트는 해시의 결과를 더욱 복잡하게 만들어 동일한 비밀번호라도 해시 결과가 다르게 나타나도록 합니다.
- hashed: 솔트와 비밀번호를 함께 해시한 결과 값.


## 4. Hashcat

Hashcat을 사용해서 비밀번호를 추출해보자.

Hashcat을 사용하여 무작위 대입 공격(brute-force attack) 또는 특정 단어 목록을 사용한 사전 공격(dictionary attack)을 수행할 수 있습니다. 사전 파일 없이 무작위 대입 공격을 수행하는 방법을 설명하겠습니다.

### 무작위 대입 공격 (Brute-force Attack)

1. **Hashcat 다운로드 및 설치**:
   - [Hashcat 다운로드 페이지](https://hashcat.net/hashcat/)에서 최신 버전을 다운로드하여 압축을 해제합니다.

2. **해시 파일 준비**:
   - `hash.txt`라는 파일을 생성하고, 주어진 해시 값을 파일에 저장합니다.

     예를 들어, `hash.txt` 파일 내용:
     ```
     $6$ACJDAAlu$0HrEd.d649nnNcjNUeIga4AokAWZEqQ1tFdZB/VL1bea0vJj6esNlwJWPGcrHVZqg7N.WiT3rXCB8pu0w8HtD.
     ```

3. **Hashcat 실행**:
   - 명령 프롬프트에서 Hashcat을 실행합니다. Hashcat 폴더로 이동한 후, 다음 명령을 실행합니다:

   ```sh
   hashcat.exe -m 1800 -a 3 -o found.txt hash.txt
   ```

   여기서:
   - `-m 1800`: SHA-512 해시 알고리즘을 지정합니다.
   - `-a 3`: 무작위 대입 공격 모드를 지정합니다.
   - `-o found.txt`: 찾은 비밀번호를 저장할 파일을 지정합니다.
   - `hash.txt`: 해시 값을 포함한 파일입니다.

4. **결과 파일 확인**:
   - Hashcat이 크래킹에 성공하면, `found.txt` 파일에 결과가 저장됩니다. `notepad found.txt` 명령어를 사용하여 결과를 확인할 수 있습니다.


### 고급 무작위 대입 설정

기본 무작위 대입 공격은 모든 가능한 문자 조합을 시도하지만, 특정 패턴을 지정할 수도 있습니다. 예를 들어, 8자리 비밀번호로 소문자, 숫자, 대문자, 특수 문자를 조합하여 공격하려면 다음과 같이 명령을 실행할 수 있습니다:

```sh
hashcat.exe -m 1800 -a 3 -o found.txt hash.txt ?a?a?a?a?a?a?a?a
```

여기서 `?a`는 모든 문자(소문자, 대문자, 숫자, 특수 문자)를 나타냅니다.

## 5. 그 외 공격 모드

Hashcat에서 `-a` 옵션 뒤에 올 수 있는 공격 모드(attack modes)는 다양한 해시 크래킹 방법을 지원합니다. 각 공격 모드는 특정한 방식으로 비밀번호를 시도하며, 사용자가 선택한 해시 타입과 크래킹 전략에 따라 달라집니다.

다음은 Hashcat의 `-a` 옵션 뒤에 올 수 있는 모든 공격 모드입니다:

### 공격 모드 목록

1. **`-a 0`**: **사전 공격 (Dictionary Attack)**
   - 주어진 사전 파일의 각 항목을 사용하여 해시를 크래킹합니다. 사전 파일에는 미리 정의된 비밀번호 목록이 포함되어 있습니다.

   **예제**:
   ```sh
   hashcat -a 0 -m 1000 hash.txt dictionary.txt
   ```

2. **`-a 1`**: **콤비네이션 공격 (Combination Attack)**
   - 두 개의 사전 파일을 결합하여 비밀번호를 시도합니다. 첫 번째 사전 파일과 두 번째 사전 파일의 조합을 통해 비밀번호를 생성합니다.

   **예제**:
   ```sh
   hashcat -a 1 -m 1000 hash.txt dict1.txt dict2.txt
   ```

3. **`-a 3`**: **무작위 대입 공격 (Brute-Force Attack)**
   - 모든 가능한 문자 조합을 시도하여 비밀번호를 찾습니다. 문자 집합과 길이를 지정하여 비밀번호를 생성합니다.

   **예제**:
   ```sh
   hashcat -a 3 -m 1000 hash.txt ?a?a?a?a
   ```

   여기서 `?a`는 모든 가능한 문자(소문자, 대문자, 숫자, 특수 문자)를 포함합니다.

4. **`-a 6`**: **사전 공격 + 마스크 (Dictionary + Mask Attack)**
   - 사전 파일의 각 항목에 대해 마스크를 적용하여 비밀번호를 시도합니다. 마스크를 사용하여 특정 위치에 특정 문자 집합을 추가할 수 있습니다.

   **예제**:
   ```sh
   hashcat -a 6 -m 1000 hash.txt dictionary.txt ?d?d?d
   ```

   여기서 `?d`는 숫자를 의미합니다.

5. **`-a 7`**: **마스크 공격 (Hybrid Mask + Password Attack)**
   - 사전 파일의 각 항목에 대해 지정된 마스크를 추가하여 비밀번호를 시도합니다. 마스크와 사전의 조합을 사용하여 비밀번호를 생성합니다.

   **예제**:
   ```sh
   hashcat -a 7 -m 1000 hash.txt dictionary.txt ?d?d?d
   ```

   여기서 `?d`는 숫자를 의미합니다.

6. **`-a 9`**: **직렬 대입 공격 (Straight Attack)**
   - 특정 패턴을 사용하여 사전 파일의 각 항목을 순차적으로 시도합니다. 이는 사전 공격의 일종으로, 패턴을 기반으로 비밀번호를 생성합니다.

   **예제**:
   ```sh
   hashcat -a 9 -m 1000 hash.txt dictionary.txt
   ```

7. **`-a 10`**: **다중 사전 공격 (Multiple Dictionary Attack)**
   - 여러 개의 사전 파일을 사용하여 비밀번호를 시도합니다. 사전 파일의 조합을 사용하여 비밀번호를 생성합니다.

   **예제**:
   ```sh
   hashcat -a 10 -m 1000 hash.txt dict1.txt dict2.txt
   ```

### 요약

- **`-a 0`**: 사전 공격 (Dictionary Attack)
- **`-a 1`**: 콤비네이션 공격 (Combination Attack)
- **`-a 3`**: 무작위 대입 공격 (Brute-Force Attack)
- **`-a 6`**: 사전 공격 + 마스크 (Dictionary + Mask Attack)
- **`-a 7`**: 마스크 공격 (Hybrid Mask + Password Attack)
- **`-a 9`**: 직렬 대입 공격 (Straight Attack)
- **`-a 10`**: 다중 사전 공격 (Multiple Dictionary Attack)

이 공격 모드들은 다양한 해시 크래킹 전략을 지원하며, 크래킹할 해시의 유형과 필요에 따라 적절한 모드를 선택하여 사용할 수 있습니다.
