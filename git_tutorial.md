간단하게 git을 배울 수 있는 웹사이트</br>
https://learngitbranching.js.org/?locale=ko

로컬저장소와 원격저장소

branch
merge
rebase
상대 참조
cherry-pick
인터렉티브 리베이스
staging area
restore

## 명령어
Git command-line interface

### 기초
git help <command>: git 명령어에 대한 도움말.
git init: .git 디렉토리에 데이터가 저장된 새 git 저장소를 만든다.
git status: 진행 상황을 알려준다.
git add <filename>: **스테이징 영역**에 파일을 추가.
git commit: 새로운 **커밋**을 만든다.
git log: 평면화된 history의 로그를 표시.
git log --all --graph --decorate: DAG을 사용하여 history를 시각화.
git diff <filename>: 마지막 커밋 이후 차이점을 보여준다.
git diff <revision> <filename>: 스냅샷 간 파일의 차이를 보여준다.
git checkout <revision>: HEAD와 현재 분기를 업데이트.

### Branching and merging
git branch: 분기를 보여준다.
git branch <name>: 분기를 생성.
git checkout -b <name>: 분기를 생성하고 전환.
git branch <name>; git checkout <name> 과 동일.
git merge <revision>: 현재 분기를 병합.
git mergetool: 병합 충돌을 해결하는 데 도움이되는 멋진 도구를 사용.
git rebase: 패치 세트를 새로운 베이스로 배치.

### Remotes
git remote: remote 를 나열.
git remote add <name> <url>: remote를 추가.
git push <remote> <local branch>:<remote branch>: remote로 객체를 보내고 remote 참조를 업데이트.
git branch --set-upstream-to=<remote>/<remote branch>: 로컬과 remote branch 사이의 통신을 설정.
git fetch: 원격에서 객체 / 참조를 검색.
git pull: git fetch; git merge와 동일.
git clone: 원격에서 저장소를 다운.

### Undo
git commit --amend: 커밋 내용 / 메시지 를 편집.
git reset HEAD <file>: 파일을 unstage.
git checkout -- <file>: 변경 사항을 취소.

### Advanced Git
git config: Git을 고도의 사용화한다.
git clone --depth=1: 전체 버전 history 없는 shallow 클론을 한다.
git add -p: 대화형 스테이징을 한다.
git rebase -i: 대화형 리베이싱을 한다.
git blame: 누가 특정 라인을 마지막으로 편집 하였는지 보여준다.
git stash: 작업 디렉토리에 대한 수정 사항을 일시적으로 제거.
git bisect: history를 이진 탐색. (e.g. for regressions)
.gitignore: 의도적으로 추적되지 않는 파일을 지정ㄴㄴ.
