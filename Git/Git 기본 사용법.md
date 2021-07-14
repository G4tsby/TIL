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
- 현재 repository의 상태 표시

<br>

```bash
git add [filename]
```
- 스테이지 영역에 파일 추가.
- 스테이지 영역은 커밋 되기 전 임시로 사용하는 파일 영역.

<br>

```bash
git commit -m "커밋 요약

자세한 내용"
```
- 스테이지에 기록된 시점의 파일을 리포지토리에 변경 내역에 반영.
- `-m` : 커밋에 메시지 추가
- `-a` : 추가된 파일 자동으로 커밋
- `-am`