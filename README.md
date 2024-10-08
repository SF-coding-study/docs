# docs

## 0. 작업 방법
1. 원격 레포지토리를 로컬 컴퓨터로 가져오기 (Code 클릭후 URL을 복사합니다.)
   <img width="944" alt="스크린샷 2024-09-24 11 29 54" src="https://github.com/user-attachments/assets/e89a443f-65fa-4de7-8885-526335bd874e">
2. 로컬에 저장하기 (저장하고 싶은 경로에서 명령어 실행)
   ```shell
   git clone https://github.com/SF-coding-study/study.git
   ```
3. 작업후 add, commit, push 합니다.

원격 레포지토리의 최신상태 가져오는 방법
> 작업 하는 폴더 경로에서 `git pull` 명령어 실행

## 1. 코드 업로드
### Git 코드 업로드 방법
> *주의* : 해당 내용은 Git업로드 flow예시입니다.<br>
> 자세한 규칙은 `폴더`, `commit 규칙` 항목을 따라 진행해주세요!

1. 원하는 파일 혹은 폴더를 git에 추가합니다.
   ```shell
   # 파일 추가 명령어 예시 : "git add [파일 상대경로]
   git add example.java
   
   # 폴더 추가 명령어 예시 :  "git add [폴더 상대경로]
   git add sanghwa
   ```
2. commit 메시지를 작성합니다.
   ```shell
   git commit -m "커밋 메시지 내용"
   ```
3. 원격에 업로드합니다.
   ```shell
   git push
   ```

### 폴더
1. 각자 개인 폴더를 생성하고, 그 안에서만 작성합니다.
2. 하위 폴더 구조는 자유롭게 만듭니다.
3. 다른 사람의 폴더 안에서 작업하지 않도록 주의합니다.
> 예시 : sanghwa > PGS > problem.java
### commit 규칙
- 코딩테스트 코드
  - commit 메세지: [문제 출처(플랫폼)] 문제이름 / 난이도 / 걸린시간
- 터미널 명령어 예시
```shell
git commit -m "[PGS] Hello World / 브론즈5 / 1분"
```
- 플랫폼 작성법 통일:
  - [BOJ] - 백준
  - [PGS] - 프로그래머스
  - [LTC] - 리트코드
  - [CFS] - 코드포스
  - [SEA] - 삼성SW Expert Academy
  - [AGS] - 알고스팟
  - [ETC] - 그외

- 과제 코드
  - 중간 과정
    - commit 메세지: 과제이름 / 작업내용
  ```shell
  git commit -m "AwesomePhoneBook / 사용자 입력 받기"
  ```
  - 완성
    - commit 메세지 : 과제이름 / done
  ```shell
  git commit -m "AwesomePhoneBook / done"
  ```
