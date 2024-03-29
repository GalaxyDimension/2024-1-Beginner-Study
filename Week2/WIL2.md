#### Fork
+ 오픈 소스 프로젝트를 공부하거나 Contributors가 되고 싶을 때, 해당 원격 저장소(Remote Repository)를 자신의 원격 저장소로 복사할 수 있다.

#### Star
+ 관심 있는 Repository나 프로젝트에 star를 달아 “북마크”와 같이 관리

#### Issue
+ Repository에서 작업 계획, 토론 및 추적을 위해 활용

#### Branch
+ 기존 브랜치에서 분기되어 생성되는 별도의 작업 공간
+ fork와 달리 같은 Repository에 생성됨
  ##### 현재 브랜치 확인 - git branch (-a:모든 브랜치 확인시)
  ##### 브랜치 생성 - git branch (-D:삭제시) "<브랜치 이름>"
  ##### 브랜치 이동 - git checkout (-b:생성하면서 이동시) "<브랜치 이름>"
  ##### "type/ - <issue 번호> <간략한 설명>"
 

#### Pull Request
+ 분기된 Branch를 다시 병합하기 위한 절차
+ 새로운 변경을 제안하거나 병합시 발생하는 충돌을 해결
+ Merge에 앞서 코드 리뷰

#### Merge
+ Merge에는 3가지 옵션이 존재(Merge Commit/Squash and Merge/Rebase and Merge)
  + Merge Commit - 커밋이 그대로 main 브랜치로 병합
  + Squash and Merge - 하나의 커밋으로 main 브랜치로 병합
  + Rebase and Merge - 커밋의 base를 재설정, 모두 새로운 커밋으로 변경/commit hash가 변경(무수한 충돌 가능성이 있음)
    ###### commit hash란 식별을 위해 사용하는 40자리 길이의 16진수(SHA-1 해시 함수를 사용)

<https://github.com/GalaxyDimension/2024-1-Beginner-Study/pull/3>
