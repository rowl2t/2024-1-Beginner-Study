# What I Learned / Week 2
## Fork
다른 사용자의 Repository를 자신의 계정으로 복사하여 독립적으로 관리할 수 있는 기능.

![스크린샷 2024-03-31 195323](https://github.com/rowl2t/2024-1-Beginner-Study/assets/161618507/f0fc1a39-789b-4200-8701-6cbf5f34c1eb)

`Create a new fork`를 클릭하면 동일한 내용의 새 Repository를 자신의 계정에 추가할 수 있다.

## Star
관심 있는 Repository나 프로젝트에 Star를 달아 따로 확인할 수 있는 기능.

Github에서 "북마크"와 같은 기능이다.

![스크린샷 2024-03-31 195854](https://github.com/rowl2t/2024-1-Beginner-Study/assets/161618507/03e43754-0a94-4261-8ed0-e8a45ef8f4c2)

`Create list`를 통해 리스트를 만들면 리스트별로 관리도 가능하다.

## Issue
Repository에서 작업 계획, 토론 및 추적을 위해 사용되는 기능.

![image](https://github.com/rowl2t/2024-1-Beginner-Study/assets/161618507/90aa4617-c2b3-45af-b2b3-2a290ef0dcad)

![image](https://github.com/rowl2t/2024-1-Beginner-Study/assets/161618507/e6b23d95-1419-476a-b6cd-3a307402a9f3)

## Branch
기존 브랜치(Main)에서 분기되어 생성되는 별도의 작업 공간으로, Fork와 달리 해당 Repository에 생성된다.

- 브랜치 확인
  - `git branch` : 현재 브랜치 확인
  - `git branch -a` : 모든 브랜치 확인

- 브랜치 생성 / 삭제
  - `git branch "<name>"` : 브랜치 생성
    - 브랜치 이름의 형식은 보통 `type/<issuenumber>-<description>`으로 한다.
  - `git branch -D "<name>"` : 해당 이름의 브랜치 삭제

- 브랜치 이동
  - `git checkout "<name>"` : 해당 이름의 브랜치를 이동
  - `git checkout -b "<name>"` : 해당 이름의 브랜치를 생성한 후 이동
 
## Pull Request / Merge
분기된 브랜치를 다시 병합하는 절차. Pull Request를 통해 새로운 변경을 제안하거나 병합 시 발생하는 충돌을 해결한다.

- Merge의 3가지 옵션
  - **Merge Commit** : 두 브랜치(Main과 새 브랜치)를 공통 부모로 하는 새로운 Commit을 생성.
  - **Squash and Merge** : 새 브랜치의 모든 Commit을 Main 브랜치 하위의 하나의 Commit으로 병합.
  - **Rebase and Merge** : 새 브랜치의 모든 Commit을 병합 없이 그대로 Main 브랜치 하위 Commit으로 변경. **Commit Hash가 변경되고 충돌이 많아 사용에 주의해야 한다.**





## 과제 링크
<https://github.com/rowl2t/2024-1-Beginner-Study/pull/2>
