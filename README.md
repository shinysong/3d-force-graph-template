# 3d-force-graph-template

- 3d-force-graph [Github](https://github.com/vasturiano/3d-force-graph)
- 참고예제: [3d-force-graph/example/large-graph
  /index.html](https://github.com/vasturiano/3d-force-graph/blob/master/example/large-graph/index.html)
- 사용 데이터: [전국관광지정보표준데이터](https://www.data.go.kr/data/15021141/standard.do)

## 1. 프로젝트 소개

- 3D Force Graph를 이용한 시각화 예제
  - 3D Force Graph는 3D 공간에 노드와 링크를 표현하는 시각화 라이브러리이고, 원본 깃헙에 예제가 다양하게 존재함
- CSV 파일을 읽어와서 3D Force Graph에 사용하는 JSON으로 변환하는 코드
- 노드를 클릭하면 해당 관광지의 정보를 보여주는 infoBox

## 2. 프로젝트 구성

- index.html: 3D Force Graph를 보여주는 HTML 파일
- data.csv: 전국관광지정보표준데이터 CSV 파일
- data.json: 3D Force Graph에 사용하는 JSON 파일
- covert.ipynb: CSV 파일을 JSON 파일로 변환하는 코드

## 3. 사용 방법

`http-server`를 이용하여 index.html을 실행한다.
node.js 기반의 간단한 웹 서버로, 설치는 다음과 같다.

- 설치

```
npm install http-server -g
```

- 실행

```
http-server // index.html이 있는 루트 경로에서 실행
```

또는 VScode에서 [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)를 이용하여 실행한다.  
참고로 live server를 사용하면 코드가 수정될 때마다 자동으로 새로고침되기 때문에 개발중에 확인이 편리함
