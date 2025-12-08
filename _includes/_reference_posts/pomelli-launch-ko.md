제품을 출시하는 것은 언제나 가슴이 뛰는 일이지만, 서버가 3시간 만에 먹통이 된다면 어떤 기분일까요? 유저들이 트위터와 디스코드에서 접속이 안 된다고 포스트를 올리고 있는 상황의 긴장감은 잊지 못할 경험이었습니다. 

올해 7월에 Google Gemini 팀에서 Google Labs으로 합류해 일한지 약 3-4개월 만에 제품 출시를 경험할 기회를 얻었습니다. AI 제품을 만들고 싶어서 팀을 옮겼던 저는 이렇게 빨리 좋은 경험을 얻게 되어서 정말 운이 좋다고 생각합니다. 이번 글에서는 출시한 날의 경험을 공유해볼까 합니다.

## Pomelli란 무엇인가

[Pomelli](https://labs.google/pomelli)는 중소기업(Small and Medium-sized Business; SMB)을 위한 AI 마케팅 도구입니다. 각 비즈니스와 브랜드를 이해하고, 비즈니스에 맞춘 마케팅 캠페인과 광고 창작물을 쉽게 만들 수 있도록 도와줍니다. 더 자세한 내용은 [Google Keyword Blog](https://blog.google/technology/google-labs/pomelli/)을 참고해주세요.

![bdna](https://storage.googleapis.com/gweb-uniblog-publish-prod/images/Pomelli_Keyword_Blog_In-line_-_1.width-1000.format-webp.webp)
*비즈니스 DNA 생성하기*

![campaign](https://storage.googleapis.com/gweb-uniblog-publish-prod/images/Pomelli_Keyword_Blog_In-line_-_2.width-1000.format-webp.webp)
*마케팅 캠페인 만들기*

![creatives](https://storage.googleapis.com/gweb-uniblog-publish-prod/images/Pomelli_Keyword_Blog_In-line_-_3.width-1000.format-webp.webp)
*브랜드에 맞는 광고 창작물 생성하기*

<iframe width="560" height="315" src="https://www.youtube.com/embed/rsWPISYv6tQ?si=1c4Hfq0Wfldlvi0J" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

이번은 베타 출시인데, 아쉽게도 현재는 미국, 캐나다, 호주, 뉴질랜드에서만 이용할 수 있습니다. 내년에는 더 많은 국가에서 특히 한국에서 출시할 수 있기를 바랍니다!

## 출시 당일

당일 아침, 팀은 정말 들떠 있었습니다. 실시간 트래픽을 볼 수 있는 대시보드가 준비되어 있었고, 비교적 조용한 출시로 기획될 예정이었지만, 생각보다 출시한 순간부터 X(트위터)와 다른 SNS 채널에서 많은 관심을 받았습니다.

그런데 첫 트윗을 보낸 3시간 이후부터 서버가 녹기 시작했습니다. 새 유저들이 첫 단계인 비즈니스 DNA에서 다음 단계로 넘어갈 수 없다고 포스트를 올리기 시작했습니다. 저희가 해봐도 도저히 안됬죠.

자세히 보니 제가 작업한 부분에서 문제가 발생하고 있었습니다. 급하게 무슨 일이 일어나고 있는지 분석해야 했고, 코드의 일부가 문제가 있다는 것을 알아냈습니다. 이러한 상황 속에 기존 기능을 너무 많이 희생하지 않으면서도 문제가 되는 부분을 제거하는 긴급 버그 수정을 짜냈습니다. 팀원들이 발을 동동 구르는 상황에서 제 책상으로 돌아가 코딩을 하던 긴장감이 아직도 생생하네요.

다시 작동하기를 기도하며 코드를 배포했으나, 아직도 잘 작동하지 않았습니다. 이 시점까지 유저들은 거의 반나절은 제품을 못 쓰고 있었죠.. 우리는 심지어 그냥 웹사이트를 내리고, 나중에 다시 돌아오겠다고 공지하는 것까지 고려했었죠. 이렇게 된다면 정말 창피하고 난처한 상황이 되었을꺼 같은데.. 상상만해도 끔찍하네요.

하지만 그때 제 동료가 서버에서 또 다른 잠재적으로 관련된 문제를 발견했습니다. 바로 코드를 고치고 배포했더니 점점 서버가 정상으로 돌아왔습니다. 마케팅과 SNS 팀이 유저들에게 예상치 못한 트래픽으로 인한 장애를 경험했지만 이제는 정상 작동한다고 공지를 내보냈고, 우리 모두 퇴근할 수 있었습니다. 

일이 마무리된 것은 거의 자정이었습니다. 다행히 그날 발 뻗고 잠을 잘 수 있었네요. 

## 배운 점

### 성공 재난 (Success Disaster)

Google Labs PM 디렉터인 Jaclyn이 런칭을 회고하며 [블로그](https://blog.jaclynkonzelmann.com/p/embracing-the-success-disaster)에 글을 썼습니다.

그녀는 이를 **성공 재난(Success Disaster)**이라고 불렀습니다. 우리 제품이 관심과 트래픽을 얻는 데 성공했기 때문에 문제가 드러나 재난이 일어났다는 것입니다.

> "이런 종류의 문제는 (출시한 팀 입장에서는) 가지고 싶은 문제입니다. 일이 잘못된 이유는 뭔가가 엄청나게 잘 되었기 때문입니다."

평소에 같이 일하는 분이지만, 이 글을 읽고 그녀의 관점에 대해 정말 많이 감명 받았습니다. 그저 긍정적인 마인드가 아니라 무척이나 정확한 분석이 아닌가 싶습니다. 수백 명의 사용자만으로는 이 문제를 절대 발견하지 못했을 것이고, 수천 명 이상의 사용자가 제품을 사용해야만 발견할 수 있었던 문제였습니다.

베타 런칭한 한달 이상이 지난 시점, 정말 기대 이상으로 많은 사용자들이 Pomelli에 들어와 제품을 사용하는 걸 보고, 정말 무언가는 잘 되고 있구나라는 걸 느끼고 있습니다.

### 빠른 실험

Google Labs의 철학은 빠르게 런칭하고 빠르게 검증하는 것입니다. Google 같은 대기업에서는 이런 마인드셋과 환경을 갖기 어려울 수 있습니다. 이를 타파하기 위해 Labs는 말 그대로 그런 함정에 빠지지 않기 위한 실험실입니다.

https://labs.google 을 한번 둘러보시면, Google 같은 대기업이 작업하기 어려울 것 같은 많은 제품들이 있다는 것을 알 수 있습니다.

Pomelli를 런칭한 후, 저는 이제 이 철학이 실제로 무엇을 의미하는지 이해하고 체감하기 시작하고 있습니다.

### 더 큰 그림

그렇다고 Google Labs가 작은 시장만 노리는 제품을 만드는 것은 아닙니다. 빠르게 제품을 런칭하지만, 잠재적으로는 훨씬 더 큰 무언가의 씨앗을 심는 작업이라고 보셔야 합니다.

예를 들어, 저희 제품 Pomelli는 그저 콘텐츠 생성 도구가 아니라, Google이 전통적으로 약한 중소기업(Small and Medium Sized Business; SMB)들을 위한 AI 플랫폼으로 발전할 수도 있을 것입니다. [Forbes](https://www.forbes.com/sites/solrashidi/2025/10/31/will-googles-ai-bet-pay-off/
)는 이미 Pomelli의 미래에 대해서 저희보다도 더 상세하게 분석해 기사를 냈네요.

좀 더 크게 생각하고, 여러 단계 앞을 내다봐야 하지만, 빠른 출발과 검증을 위해서는 어딘가에서 작게 시작해야 합니다.

--

이번 제품 출시 경험은 제 커리어에서 잊지 못할 하이라이트였던 것 같습니다. 이 팀에 합류한 결정이 지금까지는 잘한게 아닌가 싶습니다.

앞으로도 더 많은 기능을 더해 제품을 발전시켜 나가려고 합니다. 이 과정 동안 다양한 AI 관련 제품 / 엔지니어링 문제들을 경험하고 있다보니, 이러한 배움을 글로 소화시켜 공유하도록 해보겠습니다.

