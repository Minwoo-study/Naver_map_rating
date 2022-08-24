# Naver_map_rating

## 연구 개요

본 연구에서는 네이버 지도(map.naver.com)의 크롤러를 개발하여 리뷰들을 수집하고 Beomi 님의 KcELECTRA(https://github.com/Beomi/KcELECTRA)를 활용하여 별점 예측 모델을 개발하고 검증하여 의미있는 별점 예측 모델을 개발 할 것이다.  

### Navermap Review Crawling

**크롤링은 2가지 절차로 이루어진다.**
1. Selenium으로 사용자가 지정한 키워드로 검색한 모든 상점들의 상점 이름, 영업 정보, 별점, 리뷰 개수 등의  정보들을 추출하고 정규식으로 각 상점의 코드 번호를 추출하여 상점별 URL을 추출한다.
2. 반복문을 통해 수집된 모든 상점 URL에 Selenium을 이용해 접속하고, 모든 댓글을 조회할 수 있게 더보기 버튼을 클릭하여 모든 리뷰들을 BeautifulSoup을 이용해 수집하였다.


### KcELECTA
**이번 연구에서 Beomi님의 KcELECTRA 모델을 사용하였다.(https://github.com/Beomi/KcELECTRA)**
KcELECTRA는2 019.01.01 ~ 2021.03.09 사이에 작성된 댓글 많은 뉴스/혹은 전체 뉴스 기사들의 댓글과 대댓글을 모두 수집한 데이터로 네이버 지도의 댓글을 분석하는 이번 연구에 적합할 것으로 예상되었다. 
