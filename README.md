# lab6_202034827
# 오픈소스 SW 과제
## 202034827_박지원

---

## 1. Git의 중요성
- **Git**은 software 개발뿐만 아니라 문서 작업에서도 매우 중요한 version control 도구
- 여러 사람이 함께 작업할 때는 version control이 중요하다
- 
---

## 2. version control 방식
- 두 가지 주요 방식:
  1. **Changes**: file의 변화만을 저장하는 방식
  2. **Snapshots**: file의 satus를 capture하여 저장하는 방식

---

## 3. local, 중앙 집중식, 분산 버전 관리
- **local version 관리**: 한 컴퓨터에서 version 관리를 수행
- **중앙 집중식 version 관리**: 중앙 서버에 저장하고, 여러 클라이언트가 연결하여 사용
- **분산 version 관리**: 모든 user가 자신의 local 저장소를 가짐 (예: Git)

---

## 4. Git의 세 가지 상태
- **Modified**: Modified되었으나 아직 stage 되지 않은 상태
- **Staged**: commit 준비가 된 상태.
- **Committed**: commit 되어 저장소에 안전하게 저장된 상태

---

## 5. Git 설치
- **Linux**: package 관리자 이용하여 설치
  ```bash
  $ sudo apt install git
  ```

---

## 6. Git 설정 (최초 set)
세 가지 level에서 설정 파일 관리:

- **System level**: 모든 user의 set을 관리 (`/etc/gitconfig`)
- **Global level**: 현재 user에 대한 set을 관리 (`~/.gitconfig`)
- **Local level**: 특정 저장소에 대한 set을 관리 (`.git/config`)

```bash
$ git config --global user.name "Your Name"
$ git config --global user.email "your.email@example.com"
```

---

## 7. Git 저장소 초기화
Git 저장소를 초기화하려면:

```bash
$ git init
```

---

## 8. Git status 확인
현재 저장소의 status를 확인하려면:

```bash
$ git status
```

---

## 9. file stage에 add하기
특정 file을 stage에 추가하려면:

```bash
$ git add [file_name]
```

---

## 10. file unstage하기
파일을 언스테이지하려면:

```bash
$ git rm --cached [file_name]
```

---

## 11. file ignore 하기
`.gitignore` file을 사용하여 Git이 추적하지 않을 file 목록을 지정

---

## 12. commit
commit message를 포함하여 변경 사항을 저장하려면:

```bash
$ git commit -m "commit message"
```

---

## 13. branch name 변경
branch name을 변경하려면:

```bash
$ git branch -m [new_branch_name]
```
