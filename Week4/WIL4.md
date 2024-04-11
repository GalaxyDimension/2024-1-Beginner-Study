#### branch 관리의 필요성
+ 서로의 작업에 영향을 주지 않기 위해 branch 분리 필요
+ 작업별로 구분 필요
+ main branch의 안전한 관리 필요

#### branch 보호 규칙
+ Pull Request를 승인하도록 제한 가능
+ 특정 branch에 Push 기능자를 제한 가능

#### branch 전략
##### Git Flow
+ Vincent Driessen이 2010년 고안
+ branch를 관리
+ 배포가 수시로 이루어지는 현 시대의 웹앱과는 부적합

+ branch의 종류
  + Main Branches
    + main(master)
      + 기본으로 생성되는 branch
      + 영원히 존재하는 첫 번째 branch
      + 병합될 때마다 제품의 새로운 버전이 만들어짐
        
    + develop
      + 영원히 존재하는 두 번째 branch
      + feature branch의 기반

  + Supporting Branches
    + feature
      + develop 브랜치에서 분기하여 작업
      + 개발 완료 후 다시 develop으로 병합
      + 대부분의 이름 사용 가능
        
    + release
      + 배포 준비를 위한 branch
      + 자잘한 버그 수정/QA 작업
      + develop branch에서 분기하여 main branch로 병합
        
    + hotfix
      + 배포 환경에서 즉각적인 수정
      + main branch에서 분기
      + main, develop 모두에 병합 필요
    
##### GitHub Flow
+ 수시로 배포되는 상황이 Git Flow와 안 어울리는 것을 개선

+ branch 종류
  + main
    + 항상 배포 가능 상태
    + 병합 전에 충분한 test 필요
      
  + feature
    + main에서 분기하여 작업 후 다시 main으로 병합
    + 브랜치의 목적을 이름에 표기
    + 코드 리뷰가 더 중요

#### 태도
##### convention을 만들어 사용
+ 훗날 convention으로 의도 파악
  
##### 구글링을 꼼꼼히
+ 직접 찾기
+ 모를때만 주변 사람에게 묻기
  
##### 코드에 대한 주인 의식을 가지자
+ public repository에 코드는 곧 내 얼굴
+ 잘 설계된 코드를 짜도록 노력
  
##### 질문을 잘 하자
+ 좋은 질문을 할 수 있도록 노력
