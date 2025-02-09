---
nav_title: AI를 통한 콘텐츠 QA
article_title: AI를 통한 콘텐츠 QA
page_order: 10
description: "이 참조 문서는 메시지 작성기에서 AI를 사용하여 메시지 콘텐츠에 대한 품질 보증을 수행하는 방법을 다룹니다."
---

# AI를 통한 콘텐츠 QA

> AI를 사용하여 메시지 작성기에서 직접 메시지 콘텐츠에 대한 품질 보증을 수행하는 방법을 배우세요.

AI를 활용한 콘텐츠 QA는 GPT와 OpenAI의 기능을 사용하여 메시지의 내용을 검사하고, 맞춤법 오류, 문법 문제, 부적절한 어조, 공격적인 언어와 같은 비효율적인 요소를 식별하여 품질 기준을 준수하도록 합니다. 캠페인 또는 캔버스에서 푸시, SMS 또는 인앱 메시지를 작성할 때 **테스트** 탭에서 이 기능에 액세스할 수 있습니다.

## 주요 기능

AI를 활용한 콘텐츠 QA는 메시지 콘텐츠의 품질을 향상시키기 위해 다음과 같은 주요 기능을 제공합니다:

- **맞춤법 및 문법 검사:** 메시지에서 철자 및 문법 오류를 자동으로 검사합니다. 이는 수정 사항을 제안하고 콘텐츠의 전반적인 정확성을 향상시키기 위한 권장 사항을 제공합니다.
- **톤 분석:** 메시지의 톤을 평가하여 잠재적인 문제를 식별합니다. 의도된 어조가 원하는 의사소통 스타일과 일치하도록 도와주며, 오해나 의도치 않은 불쾌감을 피하는 데 도움이 됩니다.
- **공격적인 언어 감지:** 잠재적으로 공격적이거나 부적절한 언어가 있는지 메시지를 스캔하여 콘텐츠를 수정하고 존중하는 의사소통을 유지할 수 있도록 합니다.
- **우발적 콘텐츠 확인:** 코드, 마크업 언어 또는 테스트 메시지가 의도치 않게 추가되었을 수 있는지 감지합니다.

## AI를 사용하여 콘텐츠 QA에 접근하기

{% alert note %}
AI를 활용한 콘텐츠 QA는 현재 푸시 및 SMS 채널에서만 사용할 수 있습니다.
{% endalert %}

콘텐츠 검사기에 액세스하려면 다음 단계를 따르세요.

1. 푸시 또는 SMS 메시지를 작성한 후 **테스트** 탭으로 이동합니다.
2. **AI를 통한 콘텐츠 QA** 섹션을 찾으세요.
3. **콘텐츠 테스트**를 클릭합니다.

![AI를 통한 콘텐츠 QA는 테스트 탭에 있습니다.][1]{: style="max-width:60%"}

### 언어 지원

GPT는 [여러 언어](https://openai.com/research/gpt-4#:~:text=GPT%2D4%203%2Dshot%20accuracy%20on%20MMLU%20across%20languages)를 이해할 수 있지만, OpenAI는 공식적으로 이를 지원하지 않습니다. Braze는 메시지 콘텐츠가 OpenAI로 전송될 때 사본의 언어 또는 로케일에 대한 추가 정보를 전달하지 않으므로, 이를 결정하는 것은 GPT에 달려 있습니다.

결과는 작성 중인 언어에 따라 다를 수 있습니다.

## 효과적인 사용을 위한 팁

AI 기능을 활용한 콘텐츠 QA를 최대한 활용하기 위한 다음 팁을 고려하세요.

- **메시지 교정:** 비록 콘텐츠 검사기가 오류를 식별하는 데 도움을 줄 수 있지만, 여전히 콘텐츠를 수동으로 교정하는 것이 중요합니다. AI 생성 제안을 유용한 가이드로 활용하되, 정확성을 보장하기 위해 자신의 판단을 사용하세요.
- **톤 분석 이해하기:** 어조 분석 결과는 주관적이며 AI 모델의 이해를 기반으로 합니다. 그들이 유용한 인사이트를 제공할 수 있지만, 의도한 어조와 대화의 맥락을 고려하여 적절한 조정을 하세요.
- **플래그가 지정된 공격적인 언어를 다시 확인하세요.** 모욕적인 언어 감지는 견고하게 설계되었지만, 때때로 잘못된 긍정 사례를 표시할 수 있습니다. 플래그가 지정된 섹션을 주의 깊게 검토하고 필요한 경우 적절한 변경을 하세요.

## 내 데이터는 어떻게 사용되고 OpenAI로 전송되나요?

메시지 내용을 확인하기 위해 Braze는 OpenAI의 API 플랫폼으로 메시지를 보냅니다. Braze에서 OpenAI로 전송된 모든 쿼리는 익명화되므로, 메시지 내용에 고유하게 식별 가능한 정보를 포함하지 않는 한 OpenAI는 쿼리를 보낸 사람을 식별할 수 없습니다. [OpenAI의 API 플랫폼](https://openai.com/policies/api-data-usage-policies) 약관에 명시된 바와 같이, Braze를 통해 OpenAI의 API로 전송된 데이터는 모델을 학습하거나 개선하는 데 사용되지 않으며 30일 후에 삭제됩니다. OpenAI의 [사용 정책](https://openai.com/policies/usage-policies) 및 [공유 및 출판 정책](https://openai.com/policies/sharing-publication-policy)을 포함하여 관련 정책을 준수해야 합니다. Braze는 AI가 생성한 콘텐츠와 관련하여 어떠한 종류의 보증도 하지 않습니다.

[1]: {% image_buster /assets/img/content_qa_ai.png %}
