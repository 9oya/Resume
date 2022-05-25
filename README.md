# LEE EUN SANG

## 프로젝트 수행이력 👨‍💻
### [보맵] 마이데이터 서비스 개발 (2021.10 ~ 2022.05.30)
시작: 2021.10.01\
출시: 2022.05.30
#### 프로젝트 경험:
마이데이터 서비스 프로젝트에 중간에 투입되어 기한내에 서비스를 개발완료해야 했습니다.\
프로젝트의 기획과 디자인이 상당부분 변경되었고 주요 기능은 정상동작하지 않았습니다.
기능성/취약성 점검을 위한 1차 개발완료 기한또한 촉박하여 화면단위 모듈을 새로만들기에도 부담되었습니다.

기능과 화면의 흐름을 `flow chart`, `sequence chart`를 이용해 도식화했습니다.
Android 그리고 백앤드 개발자분들과 기획/디자인 팀원들과 **적극적인 커뮤니케이션**을 통해 기존 모듈 수정과 새로운 화면모듈을 생산했습니다.\
보맵 iOS앱은 `ReactorKit` architecture를 사용합니다.
미완성 코드에서 `memory leak`과 `thread unsafe`한 화면 모듈들을 thread safe하게 수정하고 Xcode instrument와 
memory graph debug를 통해 memory leak을 잡아 내었습니다.
Thread safe 한 코드를 위해 reactor (view model) 에 State struct 에 mutable한 var 변수들을 담아 
view controller에서 단방향으로 접근하도록 했으며 그 외에 변수는 let constant로 동시 writing으로 발생할 수 있는 
`race condition`을 제어했습니다.

결과적으로 평소 잘 사용하지 않던 `xcode instruments`와 `memory graph debugger`를 학습하고 사용하여 문제를 해결하는 경험을 하였고 
해당 프로젝트를 기한내에 1차 개발 완료하여 기능성, 취약성 점검을 잘 마칠 수 있었습니다.

### [보맵] 메인화면 리뉴얼 (2022.02 ~ 2022.04.08)
시작: 2021.02.09\
출시: 2022.04.08
#### 프로젝트 경험:
최초회원가입 후 내 보험 연동 60% -> 75%\
메인화면 진입후 연동완료까지 5분 -> 3.3분

### [보맵] 회원가입 네이티브화 (2022.04 ~ 2022.05.09)
시작: 2021.04\
출시: 2022.05.09
#### 프로젝트 경험:
Intro화면 제거 A/B테스트 성과 전환률 70.7% -> 76.2%\
회원가입 Native화 전환률 76.2% -> 90%

### [보맵] 보장분석 개선 ( ~ 2021.03.10)
출시: 2021.03.10
#### 프로젝트 경험:
설문 개선 (2021.02.17)\
탭 메뉴 추가, 화면 플로우 개선 (2021.03.10)

### [보맵] 보장분석 확장 ( ~ 2021.05.20)
출시: 2021.05.20
#### 프로젝트 경험:
선택보장 치아 핏팅 추가

### [보맵] 채팅상담 서비스 개발 ( ~ 2021.06.09)
출시: 2021.06.09
#### 프로젝트 경험:
채팅상담 서비스 개발 (2021.06.09)\
플로팅 버튼 추가 (2021.07.28)\
상담 제3자동의 레이어 팝업 개선 (2021.09.15)\
-> 상담 건수 9.4% 증가\
-> 보험 가입 40.5% 증가

제3자동의 레이어 팝업 웹뷰 A/B테스트 추가 (2022.03.16)

## 자기소개 ✍️
### 프로젝트 팀 경험:
제가 속해 있던 보장분석 팀과 현재있는 플랫폼팀도 한번에 완변한 제품을 만드는 것이 아닌 실험과 데이터를 통해 사용자의 니즈를 측정하고 그에 따른 기획과 제품의 개선 방향을 정했습니다. 앞서 설명드린 보장분석 개선 프로젝트와 메인화면 리뉴얼, 회원가입 화면 네이티브화 와 같은 프로젝트들 모두 한 번에 배포가 아닌 점진적인 개선을 통해 유의미한 지표와 성과를 낸 프로젝트들 입니다.\
회원가입 네이티브화 프로젝트의 경우 가장 큰 지표개선이 된 프로젝트로 기존 전환률 70%대에서 90%까지 약 18%정도의 지표개선이 이루어 진 것으로 결과가 나왔습니다.\
메인화면 개편으로 내 보험정보 연동을 한 사용자의 지표가 기존 60%대에서 75%까지 개선되고 UX의 개선으로 유저가 연동을 메인화면에 진입후 연동을 완료하기까지의 시간또한 기존 5분대에서 3분대로 개선이 이루어졌습니다.

### 개발/배포 환경 경험:
Apple의 보안, 빌드, 배포 환경에 대한 전반적인 이해를 바탕으로 최근 Xcode13.3환경에서의 3rd party frameworks에 대한 빌드 버전관리와 지원이 중단된 하위 SDK 버전 업데이트 및 그에 의존된 frameworks와 그에 대한 service사용 코드와 로직에 대한 마이그레이션 작업을 진행했습니다. Test devices, provisioning profile관리와 CI/CD 빌드, 배포환경 점검과 Appsuite와 같은 난독화 툴에 대한 점검및 대응을 수행합니다.

### 좋은 개발자가 되기 위한 노력:
**팀에 협업을 중요시 합니다.** 비개발 분야 팀원들의 의견을 존중합니다. 적극적인 커뮤니케이션을 통해 팀이 더 나은 방향으로 갈 수 있다고 믿습니다. 비판에는 구체적인 근거와 방향성 제시가 포함되어야 한다고 생각합니다.

**평소 Computer science 공부와 Problem solving 연습**을 합니다. (Algorithm&DataStructure, Network, DataBase, OS, SoftwareEngineering) 언제나 부족하다고 생각하며 다시 전공서적 원서로 공부를 시작했습니다 :)

**Open source에 관심**이 있습니다. BOMAPP iOS 앱 홈 리뉴얼에 앱스토어 앱과 유사한 페이징, 스크롤링 기능에 요구되어 오픈소스를 알아보던 중 적절한 프레임워크를 찾지 못해 직접구현을 고려 했고 해당 기능을 프레임워크로 분리, 오픈소스화 시켜 관 리하려는 시도를 했습니다. 현재 주요기능과 RxSwift extention이 포함된 1.0.0버전 배포에 성공했습니다. (아직 개선작업 중으로 이후 검증이 완료되면 홍보 예정입니다.) (https://github.com/9oya/SSPager)

**Apple의 iOS플랫폼 Foundation에 대한 이해**를 높이려고 학습합니다. Apple developer document와 HIG를 가까이 하고 플랫폼에 대한 이해와
Foundation을 놓치지 않으려고 합니다.

**새로운 트랜드 follow up**에 필요성과 중요함을 이해하고 wwdc에 중요한 세션또는 topics 대한 요약 또는 정리를 하려고 합니다. (Scenedelegate, SwiftUI, Async/Await, …) 
