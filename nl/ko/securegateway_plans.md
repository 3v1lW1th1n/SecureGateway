---

copyright:
  years: 2015, 2018
lastupdated: "2018-08-10"

---

# {{site.data.keyword.SecureGateway}} 서비스 플랜

v1.7.0 릴리스의 경우 모든 회사의 요구사항에 맞게 {{site.data.keyword.SecureGateway}}를 스케일링할 수 있도록 해주는 새로운 계층 지정 가격 모델이 도입되었습니다. 다음 표에서는 공개적으로 사용 가능한 각각의 플랜과 연관된 제한사항을 제공합니다.

![계층 지정 플랜 모델](./images/planDetails.png?raw=true "계층 지정 플랜 모델")

## 플랜 변경
플랜을 변경하는 경우 새 플랜은 업그레이드 또는 다운그레이드로 간주됩니다. 이는 각각의 플랜에서 허용되는 기본 게이트웨이 수를 통해 판별됩니다(예: Professional(5)에서 Enterprise(25)로의 변경은 업그레이드임). 업그레이드의 경우 서비스 중단이 발생하지 않지만 다운그레이드의 경우 모든 게이트웨이를 [비활성](/docs/services/SecureGateway/securegateway_faq.html#states) 상태로 업데이트하기 때문에 서비스가 복원되기 전에 게이트웨이 및 대상을 (새 플랜 한계까지) 재활성화해야 합니다.

<b>참고</b>: 표준 플랜에서 임의의 새 플랜으로 변환하는 경우 다운그레이드로 간주됩니다.


## 한계 초과 알림
허용되는 최대 게이트웨이/대상 수를 작성하는 경우 게이트웨이/대상의 대시보드에 경고 로그가 표시됩니다.

최대 클라이언트 수에 도달한 상태에서 새 클라이언트가 게이트웨이에 연결하려고 시도하는 경우 클라이언트 로그에 오류 로그가 표시되고 게이트웨이에서 새 클라이언트를 종료합니다.

데이터 사용량이 데이터 전송 허용량을 초과하는 경우 클라이언트 로그에 오류 로그가 표시되고 게이트웨이에서 클라이언트를 종료합니다.