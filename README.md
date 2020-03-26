# pyspark_study

## why use pyspark ?([출처](https://www.guru99.com/pyspark-tutorial.html#8))

Pyspark gives the data scientist an API that can be used to solve the parallel data proceedin problems. Pyspark handles the complexities of multiprocessing, such as distributing the data, distributing code and collecting output from the workers on a cluster of machines.

> Pyspark는 데이터 과학자에게 parallel data proceeding 문제를 해결하는데 도움되는 API를 제공한다. Pyspark는 데이터 및 코드 배포, 클러스터 등 복합적인 내용들을 처리한다.

Spark can run standalone but most often runs on top of a cluster computing framework such as Hadoop. In test and development, however, a data scientist can efficiently run Spark on their development boxes or laptops without a cluster.

> Spark는 독립적으로 활용하기도 하나 대부분 Hadoop과 같은 cluster computing framework에서 활용된다. 하지만 데이터 과학자는 테스트 및 개발을 클러스터 없이도 효율적으로 사용할 수 있다.

One of the main advantages of Spark is to build an architecture that encompasses data streaming management, seamlessly data queries, machine learning prediction and real-time access to various analysis.

> Spark의 큰 장점 중 하나는 데이터 스트리밍 관리, 데이터 쿼리, 머신러닝을 이용한 예측 및 분석에 필요한 실시간 처리 등의 아키텍쳐를 구성할 수 있다는 것이다.

Spark works closely with SQL language, i.e., structured data. It allows querying the data in real-time.

> Spark는 SQL과 유사하게 동작한다. 실시간으로 쿼리를 활용하여 데이터를 처리할 수 있다.

Data scientist main's job is to analyze and build predictive models. In short, a data scientist needs to know how to query data using SQL, produce a statistical report and make use of machine learning to produce predictions. 

> 데이터 과학자의 주요 업무는 예측 모델을 분석하고 만드는 것이다. 따라서 데이터 과학자는 SQL을 활용하여 데이터를 처리할 줄 알아야 하며 머신러닝을 이용하여 예측 모델을 생성하고 이에 맞는 보고서를 작성할 수 있어야 한다. 

Data scientist spends a significant amount of their time on cleaning, transforming and analyzing the data. Once the dataset or data workflow is ready, the data scientist uses various techniques to discover insights and hidden patterns. The data manipulation should be robust and the same easy to use. Spark is the right tool thanks to its speed and rich APIs.

> 데이터 과학자는 데이처 처리, 변환 및 분석에 많은 시간을 할애한다. 데이터가 준비된 이후엔 그 속에 숨겨진 패턴과 인사이트를 찾기 위해 다양한 기술을 활용한다. 데이터를 처리하는 일은 robust해야하며 쉬워야 한다. Spark의 빠르고 다양한 API는 이러한 데이터 처리에 적합한 도구다. 

## 참고
- [How to install PySpark locally](https://medium.com/tinghaochen/how-to-install-pyspark-locally-94501eefe421)
- [Jupyter Lab에서 Spark 실행하기](https://lamanus.kr/68)
