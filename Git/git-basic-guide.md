# Git 기본 사용법

```bash
git init
```
- repository 초기화. `.git` 디렉터리를 생성한다.
- `.git` 에는 현재 디렉터리의 관리 정보를 저장함. (변경 내역 등)

<br>

```bash
git status
```
- 현재 repository의 상태 표시.
- `-v` 변경점 표시

<br>

```bash
git pull # 로컬 브랜치와 같은 이름의 remote 브랜치에
git pull origin master
```
- 리모트 서버의 최신 소스를 가져와 로컬 소스에 Merge.

<br>

```bash
git fetch
```
- 새로 업데이트한 내용만 가져온다.

<br>

```bash
git add [filename]
```
- 스테이지 영역에 파일 추가.
- 스테이지 영역은 커밋 되기 전 임시로 사용하는 파일 영역.
- `-p` 변경사항 하나하나 확인.  
<택배상자에 보낼 물건 담기>

<br>

```bash
git commit -m "커밋 요약

자세한 내용"
```
- 스테이지에 기록된 시점의 파일을 리포지토리에 변경 내역에 반영.
- `-m` : 커밋에 메시지 추가.
- `-a` : 추가된 파일 자동으로 커밋.
- `-am` : 한번에 add하고 커밋.
- **커밋은 반드시 실행 가능한 단위로 해야한다.**  
<택배상자를 포장하기>

```bash
git log --graph
* commit 99cc14ef9ca110f2e5a26438fcc174029d905204 (HEAD -> master, origin/master)
| Author: g4dra <103wndnjs@gmail.com>
| Date:   Wed Jul 14 20:48:16 2021 +0900
| 
|     Git 기본 사용법
| 
* commit bc40cf56954976c8ee6e44ee26059260083f9684
  Author: g4dra <103wndnjs@gmail.com>
  Date:   Wed Jul 14 19:32:47 2021 +0900
  
      Added README.md
```
- 커밋마다 고유한 해시값 존재.

<br>

```bash
git push origin master
```
- 변경 사항을 리모트 서버에 업로드.
- `--set-upstream` 옵션을 사용하면 다음 푸쉬부터는 `git push`만 입력해도 처음 입력했던 브랜치에 푸쉬된다.
<택배 부치기>

```bash
git checkout <시점>
```  
- change 느낌. **HEAD가 가리키는 Branch를** 변경한다.
- <시점> 에는 Branch이름 혹은 Commit ID 가 들어간다.

```bash
git reset 
```
- roll back 느낌. **Branch가 가리키는 commit** 을 변경한다.
- `--hard` 옵션으로 working directory의 내용까지 변경한다. **위험!**