# 트위터 미세 조정

이 리포지토리는 트윗에서 GPT-3.5-Turbo를 미세 조정하는 방법을 보여줍니다. 특히 Elon Musk의 트윗을 예로 들어 설명합니다.

이 예제에서는 먼저 [Apify](https://apify.com/)를 사용하여 트위터에서 데이터를 내보냅니다.
이 데이터의 사본은 [dataset_twitter-scraper_2023-08-23_22-13-19-740.json](dataset_twitter-scraper_2023-08-23_22-13-19-740.json)에서 찾을 수 있습니다.

그런 다음 이 데이터를 GPT-3.5-Turbo 모델을 미세 조정하는 데 사용할 수 있는 형식으로 로드한 다음 정확히 그 작업을 수행하는 데 사용합니다. 이 작업은 `python ingest.py`를 실행하여 수행할 수 있습니다.

이 미세 조정된 모델을 프롬프트된 GPT-3.5-Turbo 모델과 비교하기 위해 Streamlit 앱이 생성됩니다.
이 앱은 `streamlit run app.py`로 실행할 수 있습니다.

Streamlit에서 호스팅되는 최종 앱 [여기](https://elon-twitter-clone.streamlit.app/)에 액세스합니다.
