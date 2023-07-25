> git 정리
# git

## 버전 관리란?
""버전관리"" 는 무엇이고 우리는 왜 이것을 알아야 할까?
버전 관리 시스템은 파일 변화를 시간에 따라 기록했다가 나중에 특정 시점의 버전을 다시 꺼내올 수 있는 시스템이다. 이 책에서는 버전 관리하는 예제로 소프트웨어 소스 코드만 보여주지만, 실제로 거의 모든 컴퓨터 파일의 버전을 관리할 수 있다.


## 분산 버전 관리 시스템 (DVCS)

![DVCS](./assets/version_database.png)


## 세가지 상태

![areas](./assets/areas.png)
working directory(local)에서 작업을 수행한 뒤 staging area에 올리고, staging area에 올려져 있는 여러 파일들을 commit하여 message와 함께 push하여 git repository로 올린다.


## Branch

![Branch](./assets/git-model-branch.png)
Git의 Branch 모델은 원래 코드를 복사하여 원래 코드와는 상관없이 독립적으로 개발을 진행할 수 있게 하는 모델이다. Branch를 만들기, branch 사이 이동을 가볍게 수행할 수 있다. 주로 master branch(mac에선 main branch)에 원본을 두고, sub branch들을 만들어 수정 과정을 거친다. 아래의 명령어로 쉽게 branch를 만들 수 있다. branch를 merge 시킨 후엔, 보통 해당 branch를 삭제한다. (추후에 필요할 때 branch를 다시 생성)
```shell
git branch -c <branch name>
```


## fork & pull

Collaborator로 지정이 되어있지 않을 때 사용하는 cooperate 방식으로 코딩에 참여할 수 있다.
Fork를 통해 public repository에 있는 코드를 자신의 git repository로 복사해올 수 있다. 자신의 git repository(또는 local)에서 수정한 뒤 pull repository로 원본과 merge 시킬 수 있다.


## 명령어

```shell
git init
```
- `.git directory`를 생성하는 명령어

```shell
git add .
```
- `working directory`에 있는 파일, 폴더를 `staging area`에 추가
- add 하기전엔 파일이 저장이 되었는지 확인하기

```shell
git commit -m 'message'
```
- `staging area`에 올라간 파일들을 저장

```shell
git remote -v
```
- 현재 배정 되어있는 주소를 확인

```shell
git remote add origin <remoteurl>
```
- 원격저장소 주소를 `origin`이라는 별명으로 저장

```shell
git remote remove origin
```
- `origin`에 저장된 원격저장소 주소를 할당 해제

```shell
git push origin master
```
- `master` 브랜치를 `origin` 원격저장소로 업로드
- `origin`에 있는 자료가 `local` 자료의 수정전과 다를 경우 `pull`을 통하여 동기화 해야 `push` 가능

```shell
git clone <remote url>
```
- 원격저장소에 있는 레포를 현재 폴더에 복제

```shell
git pull origin master
```
- 원격 저장소에 마지막 코드 상태를 다운로드


## git 프로필 사이트

`<git user id>.github.io` 이름으로 repository를 생성할 경우 해당 주소로 git 프로필 사이트를 생성한다.
> 웹페이지 스켈레톤 코드는 startbootstrap에서 가져올 수도 있다