# Git

(**버전**을 통해)코드 관리 도구



## SCM & VCS

* SCM: Source Code Management (소스 코드 관리)
* VCS: Version Contron System (버전 관리 시스템)



## Git?

* 버전 관리 도구
  * 변경 이력 트래킹
  * 언제든 특정 시점으로 이동 가능
* 백업 도구
* 협업 도구



## Git 버전 관리

> 중요: Git은 **폴더 단위**로 코드를 관리

* 커밋 == 버전 생성 == 스냅샷 촬영 == 현재 상태 저장



## git init

특정 폴더를 git으로 관리 시작

* `(master)`프롬프트에 표시
* `.git`폴더 생성
  * `.git`폴더 삭제 시 git 관리 중지



## git status

git에게 상태 확인

* `git init`직후

```bash
On branch master: master라고 하는 branch에 있어

No commits yet: 아직 commit 없어

nothing to commit (create/copy files and use "git add" to track)
: commit 할 게 없어 (트래킹 하고 싶으면 `git add` 명령어를 사용해)
```

* `a.txt`파일 생성 직후

```bash
Untracked files: 추적되지 않은 파일이 있어
(use "git add <file>..." to include in what will be committed)
a.txt (빨강)
commit 될 수 있게 포함하고 싶으면 `git add <파일명>`을 사용해
nothing added to commit but untracked files present (use "git add" to track)

```

* `git add a.txt`직후

```bash
Changes to be committed: commit될 변경 사항이 있어
(use "git rm --cached <file>..." to unstage)
new file: a.txt (초록)
```



## git add [파일명]

Staging Area(스냅샷 무대)에 파일 추가



## git commit -m "커밋 메시지"

버전을 생성

* 커밋(버전) 구성 요소
  * 해시(Hash)
  * 작성자
  * 날짜
  * 커밋메시지: 버전에 대한 설명

```bash
[master (root-commit) c244c22] First commit
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 a.txt
```



## git log

버전(커밋)들의 히스토리(로그)



## git config

설정

* `git config [설정할내용] [설정할값]`
  * `git config user.name 'John Kang'`
  * `git config user.email 'hphk.john@gmail.com'`
  * `git config --global`: 전역 설정



```bash
Author identity unknown: 작자 미상

*** Please tell me who you are.: 니가 누군지 말해주세요.

Run 다음을 실행하세요

git config --global user.email "you@example.com"
git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository
```

