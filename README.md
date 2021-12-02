# News Topic Classification
데이콘 주관 뉴스포틱 분류 AI 경진대회 데이터셋을 활용한 프로젝트. <br/>
Dacon 뉴스 토픽 분류 AI 경진대회 : https://dacon.io/competitions/official/235747/overview/description

## 데이터 분석

데이터 분포도를 통해 어느정도 inbalanced data distribution을 갖고있다는 점을 확인

![](sample/data_distribution.png)

Easy Data Augmentation을 활용해 클래스 분포를 균일하게 설정

![](sample/auged_distribution.png)

## 전처리 적용

- 숫자, 영어, 한글이 아닌 특수문자에 종류 확인
- 대표 나라 이름 및 경제항목은 일치하는 한글로 변환하고 기타 특수문자는 삭제
- PykoSpacing을 사용해 띄어쓰기 교정

검출한 특수문자

![](sample/special_case.png)

## 모델 학습 결과
