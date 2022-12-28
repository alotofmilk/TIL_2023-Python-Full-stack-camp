# 깃허브 정리 ✨

## 개념 정의 👻
- working directory -> 작업 공간
- staging area -> 버전으로 기록하기 위한 임시 저장 공간
- repository -> 커밋(버전)들이 기록되는 곳

> **작업을 하고 -> 변경된 파일을 모아 (add) → 버전으로 남긴다 (commit)**


#### 낯선 표현들 정리하기 ⭐
- Untracked files : 파일이 만들어지긴 했는데, 아직 add 되진 않았다는걸 의미!
- Changes to be commited : 커밋될 변경 사항들. 이 파일은 `git add` 입력까지 진행되었다는 뜻!
- nothing to commit, working tree clean : `working directory`와 `staging area` 모두 비어있다는 뜻

## 명령어 정리 📝

#### 먼저 git 돌릴 계정을 설정해보자! 😋
- git config --global user.email "깃허브 계정 이메일"
- git config --global user.name "깃허브 계정 닉네임"

#### git init
저장소를 만드는 선언. 이제 `.git` 이라는 폴더가 생성된다! 이제 이 폴더 안에 버전을 기록할 수 있다는 뜻. 즉, 다시 말해 `깃 관리를 시작하겠다`는 선언!

#### git add <파일 이름>
working directory -> staging area로 이동할 때 `add`를 사용한다! 커밋하려면 반드시 써줘야하는 명령어. working directory와 repository를 이어주는 징검다리 역할이라고 생각하면 편할듯!

`working directory` 안에 있는 파일들은 모두 untracked 상태. `git add`를 통해 tracked로 바꿔줄 수 있다!

git은 `tracked` 상태인 파일들만 `modified` 여부를 관리할 수 있기 때문에, 파일이 수정되면 `git add`를 통해 다시 스테이지에 등록해주어야 한다!

#### git commit -m <커밋 메시지>
**커밋** 한다는 건 무슨 뜻일까? 😗
> staged 상태의 파일들을 버전으로 기록하겠다는 걸 의미한다! 즉, 다시 말해 add를 통해 staging area에 들어온 파일들을 버전으로 남기는걸 의미한다.

변경 사항을 나타낼 수 있도록 꼭! 명확하게 작성하자.
git은 파일이 달라지지 않으면 성능을 위해 파일을 새로 저장하지 않는다!

#### git status
working directory와 staging area 내역을 조회하고 싶을 때 입력하는 명령어! 커밋 내역을 보고싶을 때 사용하는 명령어는 아니라는 점에 유의하자.

#### git log
커밋 내역을 보고싶을 때 이걸 입력하면 된다! 조금 응용해본다면 다음과 같이 사용해볼 수도 있다.
- **git log -1**
    > 최근 1개의 commit 내역을 보고싶을 때!
- **git log --oneline**
    > 커밋 내역을 한 줄로 출력해보고 싶을 때 사용
- **git log -2 --oneline**
    > 위 2개 명령어를 짬뽕해본거~
    > 최근 2개의 commit 내역을 한 줄로 출력해보기

#### git config --global -l
지금 git을 돌리고 있는 계정이 `어떤 계정인지 확인`하고 싶을 때 사용하는 명령어