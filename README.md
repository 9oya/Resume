# LEE EUN SANG

### [보맵] 마이데이터 서비스 개발 (2021.10 ~ 2022.05.30)
시작: 2021.10.01\
출시: 2022.05.30
#### 프로젝트 경험:
마이데이터 서비스 프로젝트에 중간에 투입되어 기한내에 서비스를 개발완료해야 했습니다.\
프로젝트의 기획과 디자인이 상당부분 변경되었고 주요 기능은 정상동작하지 않았습니다.
기능성/취약성 점검을 위한 1차 개발완료 기한또한 촉박하여 화면단위 모듈을 새로만들기에도 부담되었습니다.

기능과 화면의 흐름을 `flow chart`, `sequence chart`를 이용해 도식화했습니다.\
Android 그리고 백앤드 개발자분들과 기획/디자인 팀원들과 **적극적인 커뮤니케이션**을 통해 기존 모듈 수정과 새로운 화면모듈을 생산했습니다.

보맵 iOS앱은 `ReactorKit` architecture를 사용합니다.\
미완성 코드에서 `memory leak`과 `thread unsafe`한 화면 모듈들을 thread safe하게 수정하고 Xcode instrument와 
memory graph debug를 통해 memory leak을 잡아 내었습니다.
Thread safe 한 코드를 위해 reactor (view model) 에 State struct 에 mutable한 var 변수들을 담아 
view controller에서 단방향으로 접근하도록 했으며 그 외에 변수는 let constant로 동시 writing으로 발생할 수 있는 
`race condition`을 제어했습니다.\
결과적으로 평소 잘 사용하지 않던 `xcode instruments`와 `memory graph debugger`를 학습하고 사용하여 문제를 해결하는 경험을 하였고 
해당 프로젝트를 기한내에 1차 개발 완료하여 기능성, 취약성 점검을 잘 마칠 수 있었습니다.
