# What I Learned / Week 1
## Git의 필요성
개발을 하다 보면 많은 어려움이 생긴다.

- 코드의 수정 관리
- 많은 양의 파일 관리
- 버전 관리
- 결국 개발은 협업으로 이루어짐

Git은 버전 관리, 협업을 위해 만들어진 오픈소스 소프트웨어.

Git을 통해 누가, 무엇을, 언제, 어떻게 수정했는지를 추적하고 원하는 상태의 코드를 사용할 수 있다.

## 파일의 생명 주기
![image](https://github.com/rowl2t/2024-1-Beginner-Study/assets/161618507/bbdc1908-a812-4039-8173-54a85080bd38)

Git에서 파일은 크게 Untracked / Tracked 상태로 나뉜다.

Tracked 상태에서 파일은 삭제되기 전까지 Unmodified - Modified - Staged 상태를 순환하게 된다.

## Git / Github를 통한 파일 관리
![image](https://github.com/rowl2t/2024-1-Beginner-Study/assets/161618507/dbfaae08-7429-47ec-b349-bf9f5df1012e)

### Git을 Github 계정과 연동
- `git config --global user.name "<username>"`
- `git config --global user.email "<email>"`

### Git으로 파일 관리
- **디렉토리 설정**
  - `git init` : 디렉토리에 Git 저장소 생성
  - `rm -r .git` : 해당 디렉토리의 Git 저장소 삭제
 
- **Git으로 관리할 대상 등록**
  - `git add .` : 해당 디렉토리의 모든 파일을 등록
  - `git add <filename>` : 특정 파일을 등록
  - `git rm --cached <filename>` : 등록된 파일을 Unstage로 되돌림
 
- **파일을 로컬 저장소로 이동**
  - `git commit -m "<message>"`
  - Commit Message의 종류(Type)는 다음과 같다.
    - **feat** : 새로운 기능을 추가한 경우
    - **refactor** : 기존 코드를 개선한 경우
    - **fix** : 버그를 수정한 경우
    - **chore** : 코드 외의 설정을 변경한 경우
    - **docs** : 문서화
    - **test** : 테스트 코드
  - 주로 `<Type>: <Comment>` 의 양식으로 작성함
 
- **로컬 저장소의 파일을 Github(Remote)로 업로드**
  - 업로드에 앞서 Github에서 Remote Repository를 생성
  - Local Repository를 생성한 Remote Repository에 연동
    ```
    git remote add origin <url>
    git branch -M main
    git push -u origin main
    ```
  - 이후 파일 관리는 add, commit 후 `git push origin main` 사용

## 과제 링크
<https://github.com/rowl2t/rowl2t>


