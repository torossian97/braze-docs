---
nav_title: 대형 대조군 다루기
article_title: 대형 대조군 다루기
page_order: 2

page_type: solution
description: "이 도움말 기사에서는 대조군이 예상보다 클 수 있는 이유를 설명하고 이를 해결하기 위한 단계를 안내합니다."
tool: Canvas
---

# 대형 대조군 다루기

캔버스를 만들 때 다음 [예시](#example)와 같이 대조군과 배리언트 그룹 사이에 오디언스가 균등하게 나뉘기를 기대했을 수 있습니다. Braze가 그 이유와 해결 방법을 설명해 드리죠!

사용자가 가입하는 그룹은 설정에 따라 다릅니다. 이것은 대조군 또는 배리언트 그룹일 수 있습니다. 사용자가 모든 기준을 충족하면 [진입 단계][1]에서 캔버스에 들어갑니다. 캔버스를 설정할 때, 각 배리언트와 대조군에 들어갈 사용자 비율을 정의합니다.

만약 대조군이 배리언트 그룹에 비해 크다면 (그리고 이것이 본인의 의도가 아니라면) 다음을 권장합니다.
1. 진입 오디언스 필터를 "푸시 활성화 여부"로 설정하세요.
2. 진입 오디언스 필터를 "옵트인 또는 구독됨"으로 설정하세요.

캔버스를 대조군과 함께 만들 때, 엔트리 오디언스의 모든 사용자가 캔버스 내에서 메시지를 받을 수 있도록 하세요(예: 캔버스에는 푸시 및 이메일 메시지가 포함되어야 합니다).

## 사용 사례

다음 시나리오를 상상해 봅시다:
- 캔버스는 하나의 배리언트와 대조군을 가지고 있습니다.
- 배리언트의 첫 번째 단계는 푸시 알림입니다.
- 사용자의 90%는 배리언트에 들어가도록 선택되었고, 10%는 대조군에 들어가도록 선택되었습니다.

![캔버스 예제][41]

이 시나리오에서 캔버스에 들어가는 사용자의 90%가 배리언트에 들어갈 것입니다. 

활성 사용자로 돌아보면, 39.8k 사용자가 포함되어 있지만 그 중 73%만 푸시가 활성화되어 있음을 알 수 있습니다.

![항목 오디언스][42]

이는 사용자의 90%가 배리언트에 들어가도록 지정했더라도 실제로 모든 사용자가 푸시 알림을 받을 수 있는 것은 아니라는 것을 의미합니다. 푸시 알림을 받을 수 없는 이러한 사용자는 여전히 배리언트에 들어갑니다.

아직도 도움이 필요하신가요? [지원 티켓]({{site.baseurl}}/braze_support/)을 여세요.

_마지막 업데이트 날짜: 2020년 12월 3일_

[1]: {{site.baseurl }}/user_guide/engagement_tools/canvas/create_a_canvas/create_a_canvas/#step-2-use-the-entry-wizard-to-set-up-your-canvas
[41]: {% image_buster /assets/img_archive/trouble15.png %}
[42]: {% image_buster /assets/img_archive/trouble16.png %}
