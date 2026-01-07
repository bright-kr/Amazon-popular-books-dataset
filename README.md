# Amazon-popular-books-dataset
Amazon에서 가장 많은 리뷰를 받았으며 가장 많이 판매된 도서의 GitHub データセット입니다.
이 Amazon データセット에는 190,000권이 넘는 베스트셀러 도서가 포함되어 있습니다. 이 Amazon データセット의 각 도서 제목은 10,000개 이상의 독자 리뷰를 확보하여, 제공되는 도서 중 가장 인기 있는 도서로 두드러집니다. 

<h2>Key data points included in this free dataset:</h2>

* ```ASIN```
* ```ISBN10```
* ```Categories```
* ```Reviews count```
* ```Avg. rating```
* ```Number of sellers```
* ```URL```
* ```Image```
* ```Final price```
* ```Title```
* ```Description```
* ```Availability```

---
![Amazon dataset sample](https://github.com/luminati-io/Amazon-popular-books-dataset/blob/main/Datasets%20ads%20for%20Amazon.png)

<h3>How was this Amazon dataset created</h3>
  
이는 "Amazon bestseller products (public data)" データセット에서 포크된 샘플 서브셋이며, 해당 データセット는 총 <b>1,742,990개의 Amazon 베스트셀링 제품</b>으로 구성되어 있습니다. 데이터는 로ーテーティングプロキシ인 レジデンシャルプロキシ와 Web Unlocker 인프라를 통합하는 <b>Bright Data Amazon Scraper</b>를 사용하여 Amazon에서 독점적으로 추출되었습니다. 

5월 둘째 주에 추출된 전체 データセット는 Bright Data データセット 제어 패널에서 제공되는 스마트 필터 쿼리를 사용하여 더 작은 서브셋으로 축소되었습니다.


<h2>Data point filter queries used for filtering this Amazon data subset:</h2>

*   	categories: "Books"
*   	reviews_count: {"$gte":10000}

추가로 사용할 수 있는 필터 쿼리 값: <b>ASIN, brand, # of sellers, price after discount, timestamp, best-seller rank, and more.</b>

データセット는 최대한의 필터링 및 표시 속도를 위해 **snowflake**에서 호스팅됩니다.

사용 가능한 データセット 파일 형식: <b>JSON, NDJSON, CSV, XLSX</b>.

データセット 전달 방식 옵션: <b>API download, Amazon S3, Google cloud, Microsoft Azure, SFTP</b>.

전체 データセット는 <b>[Bright Data's Amazon datasets page](https://brightdata.co.kr/products/datasets/amazon)</b>에서 구매할 수 있습니다. 스마트 필터를 사용한 후 더 작은 서브셋을 구매하면 최종 가격이 낮아질 수 있습니다. 이 データセット는 월간/주간/일간 갱신으로 제공되며, 전달에는 1일만 소요됩니다.


<h2>More eCommerce datasets available from Bright Data:</h2>

*   1,000,000 "Amazon Sellers" 
*   544,000,000 "Amazon Products and Reviews" 
*   375,000,000 "Walmart products and Reviews" - Walmart データセット에 대해 더 알아보려면 [here](https://brightdata.co.kr/products/datasets/walmart)를 확인하십시오.

<h2>Free access to web data collection tools and datasets for academic researchers and NGOs</h2>

Bright Initiative는 다양한 환경 및 사회적 대의를 촉진하는 학계 교수진, NGO 및 NPO에 Bright Data의 웹 데이터 수집 플랫폼에 대한 접근을 제공합니다. [here](https://brightinitiative.com/)에서 신청서를 제출할 수 있습니다.