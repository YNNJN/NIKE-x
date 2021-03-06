# Nike x

> 나이키의 콜라보레이션 이력에 대한 Text Mining 프로젝트



<br>

<br>

## 1. Python Web Crawler

- [Nike news > Collaborations](https://news.nike.com/collaborations) 페이지의 제목, 썸네일, 본문 내용을 크롤링 함

  - 이 때 `BeautifulSoup`, `requests`의 라이브러리를 이용함

- 패션 산업에서 **cross mark(x)**가 콜라보레이션을 의미하는 것에서 착안하여 **brand x brand**를 추출함

  - 이 때 `nltk` 라이브러리를 활용한 자연어처리로 명사를 추출함

- 나이키의 해당 기간 동안의 매출을 메타 데이터로 하여, 상품군과 브랜드에 대한 Time-series 데이터 분석을 진행하기 위해 뉴스의 일자와 함께 테이블 형태로 정리함

- 2011년 11월 ~ 2020년 2월의 기간에 대하여, 전체 175건의 데이터를 확보함

  <br>

<img width="376" alt="cleansing_data" src="https://user-images.githubusercontent.com/60057425/85949073-83bec180-b98f-11ea-8f3b-224c28d2b13b.png">

<br>

(위의 이미지는 데이터의 일부만을 표시함. 전체 데이터는 [github](https://github.com/YNNJN/NIKE-x/blob/master/data/data_cleansing.csv)에서 확인 가능함)



<br>

<br>

## 2. Visualization

- [Nike news > Collaborations](https://news.nike.com/collaborations) 페이지의 본문 내 명사인 단어에 대해 `wordcloud`와 `frequency graph`로 시각화를 진행함

- 영문페이지이지만 포르투갈어로 표기된 부분이 일부 존재하여, `googletrans` 라이브러리를 이용해 포르투갈어를 영어로 번역한 데이터를 시각화에 이용함

  <br>

  > Word cloud

  <img width="1680" alt="wordcloud" src="https://user-images.githubusercontent.com/60057425/85949450-dac59600-b991-11ea-938c-f8ef61e7f731.png">

  > Frequency graph

<img width="1680" alt="frequency" src="https://user-images.githubusercontent.com/60057425/85949454-e31dd100-b991-11ea-8899-141b300e0dc5.png">





