# 리디 버그 바운티 프로그램

### 소개

리디는 고객 개인정보의 보안을 가장 중요한 가치로 여깁니다.

저희는 [버그 바운티](https://en.wikipedia.org/wiki/Bug_bounty_program) 프로그램을 통한 보안 전문가들의 도움으로 고객의 개인정보를 보호하고, 조직 전체에 걸친 보안 정책을 개선할 수 있다고 믿습니다.

만약 리디의 시스템에서 보안 관련된 문제를 찾아내셨다면 저희와 함께 [책임있는 공개](https://en.wikipedia.org/wiki/Responsible_disclosure) 절차를 진행해 주시기를 부탁드리겠습니다.

제보해주신 문제점은 저희 내부의 다른 어떤 업무보다 높은 우선순위로 처리를 진행하겠습니다.


### 범위

- 리디 (`ridi.com`)
- 리디셀렉트 (`select.ridi.com`)
- 최신 버전의 리디 iOS 애플리케이션
- 최신 버전의 리디 Android 애플리케이션
- 최신 버전의 리디페이퍼 펌웨어
- 그 외 <u>`paper.ridibooks.com`, `help.ridibooks.com`을 제외한</u> `*.ridibooks.com` 및 `*.ridi.com` 도메인에서 제공되는 모든 서비스


### 유효한 취약점

- 인증 우회 및 계정 탈취
- 열람 권한이 없는 콘텐츠 접근
- 제품적인 결함으로 인한 개인정보 유출
- 원격 코드 실행 (RCE)
- 클라이언트 측 코드 실행 (XSS)
- 기타 보안 결함 (SQL Injection, CSRF, etc.)
  - CSRF는 계정 탈취, 개인정보 유출 등으로 이어지는 경우만 유효로 인정


### 유효하지 않은 취약점

다음과 같은 경우는 포상에서 제외됩니다.

- 이미 다른 곳에 제보한 취약점
- 증명이 없이 가능성만 제시된 경우
- 패치가 완료된 최신 버전이 아닌 경우
- 재현이 불가능한 경우
- 피해가 매우 미미하거나 공격자가 굳이 취약점을 악용에 사용할 필요가 없는 경우
- 기타 통상적으로 버그 바운티에서 인정되지 않는 경우

### 유효하지 않은 취약점의 예

- 루팅된 기기에서만 동작하는 취약점
- 본인이 소유한 콘텐츠의 DRM 을 본인의 의사로 해제하는 경우
- 소프트웨어의 버전 정보 노출
- 사용자 장치에 대한 물리적 액세스 또는 MITM 공격을 요구하는 경우
- 서비스 거부 공격(DoS)
- `SameSite` 쿠키정책으로 보호되는 CSRF
- 세션 탈취나 개인정보 유출로 이어지지 않는 Open Redirect


### 포상

- 포상금액은 심각도와 보고서 등을 종합적으로 검토하여 결정됩니다.
  - 낮음(Low): 10~50만원
  - 보통(Medium): 50~100만원
  - 높음(High): 100~150만원
  - 치명적인(Critical): 200만원 이상
- 만약 같은 취약점에 대해 여러 개의 보고가 접수된다면, 최초로 명확한 보고를 제공해주신 분께 포상이 지급됩니다.
- 포상금은 매월 마지막 영업일이 포함된 주에 일괄 정산됩니다.
  - 포상 지급이 결정된 제보는 정산 완료 후 일괄적으로 안내메일을 보내드립니다.
  - 포상금은 제보된 취약점이 패치된 후 이행점검을 마쳐주시면 지급됩니다.


### 제보

취약점 보고 및 기타 문의 사항은 `help@ridi.com`으로 보내주세요.

보고서에는 아래와 같은 내용이 포함되면 좋습니다.

1. 취약점 요약
2. POC
3. 해당 취약점으로 인한 보안 위협
4. 예상되는 원인과 대응 방안

다음과 같은 경우 포상금 지급의 대상에서 제외될 수 있습니다.
- 너무 모호하거나 불명확한 보고
- 리디 버그 바운티 대응팀에서 이미 인지하고 있는 취약점을 포함한 제보


### [🏆 명예의 전당](/hall-of-fame "이미 접수는 되었으나 아직 공개되지 않은 취약점의 중복 제보를 막고, 중복 제보임의 공정성을 높이기 위해 에서 유효한 취약점 사례를 공개합니다.")
