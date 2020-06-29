# RecyclingClassificationApp
2020 Spring Capstone Project
<br>
#### Youtube
<a href="https://youtu.be/KR85F_D26dg"><img src="https://user-images.githubusercontent.com/36736904/86003151-5be16380-ba4c-11ea-96d2-433d708baece.png" align="center" height="300"></a>
<br>

## 문제 정의
#### 재활용 쓰레기를 알맞게 분류하는 네트워크를 딥 러닝을 이용해 제작하고 이를 활용해 재활용 분류 어플리케이션을 제작하는 것
<br>

## 개발 계기
#### 올바른 분리배출 방법 안내 + 재활용에 대한 인식 개선
한국의 분리수거 비율은 86%, 실제 재활용 비율은 52%

=>올바른 방법으로 분리수거 하지 않아 선별 작업에 비용이 많이 들기 때문
<br>

## 개발한 어플리케이션
<img src="https://user-images.githubusercontent.com/36736904/86004745-b11e7480-ba4e-11ea-8f1e-5af8973ffb0e.png" height="200">

<br>

## 접근 방법
#### 한국의 재활용품을 실제 상황에서 촬영한 것과 유사한 데이터셋 구성 + transfer learning으로 7개의 재활용품을 구분하는 모델 제작
- 기존의 연구에서는 실제 상황에서 촬영한 데이터셋을 사용하지 않았음
- 인공지능을 이용해 기계에 버려진 재활용품을 분류하는 것은 있었으나 기계를 설치하고 직접 찾아야 한다는 단점 존재 <br>
  (네프론, Bin-e) 
#### 전체 과정
<img src="https://user-images.githubusercontent.com/36736904/86004046-a8796e80-ba4d-11ea-8ba0-4398ddd154fc.png" height="200">
<br>

## 데이터셋, 데이터 분류 기준
Link: https://drive.google.com/file/d/12F26-RudTbxE7yhvr3rUMjX7pxHihoaF/view?usp=sharing
<br>
  
#### Pure Dataset
Kaggle에서 얻은 일정한 환경에서 촬영된 재활용품 이미지, 5종류

<img src="https://user-images.githubusercontent.com/36736904/86005761-fe4f1600-ba4f-11ea-9eff-b9492488779a.png" height="300">
<br>

#### Fake Dataset
합성을 통해 제작한 재활용품 이미지, 7종류

<img src="https://user-images.githubusercontent.com/36736904/86005858-250d4c80-ba50-11ea-8188-535ac59af370.png" height="300">
<img src="https://user-images.githubusercontent.com/36736904/86005942-3e15fd80-ba50-11ea-8436-e377a2fb8326.png" height="200">

##### Affine Transform
<img src="https://user-images.githubusercontent.com/36736904/86006012-55ed8180-ba50-11ea-954c-4094da85ff87.png" height="300">
<br>

#### Real Dataset
실제 재활용품을 촬영하거나 인터넷 검색을 통해 얻은 이미지, 7종류

<img src="https://user-images.githubusercontent.com/36736904/86006234-a2d15800-ba50-11ea-83d6-3a87de6d65fa.png" height="300">
<br>

### 데이터 분류 기준
대한민국 환경부 기준에 따라 7가지로 분류

<img src="https://user-images.githubusercontent.com/36736904/86005400-91d41700-ba4f-11ea-83bf-d7d75200f79e.png" height="200">
<br>

## 개발한 모델과 성능
https://drive.google.com/file/d/1CGSY-A6vzdUH79FIbDf19lwRt2tCRd6F/view?usp=sharing

#### BaseLine
<img src="https://user-images.githubusercontent.com/36736904/86006406-ddd38b80-ba50-11ea-91c8-1b48ec7f2cdf.png" height="300">
<br>

#### 개발한 모델
<img src="https://user-images.githubusercontent.com/36736904/86006458-f5127900-ba50-11ea-9e9b-65d57189c958.png" height="300">
<br>

#### 성능비교
<img src="https://user-images.githubusercontent.com/36736904/86006506-065b8580-ba51-11ea-80b6-3e5fa2cbe389.png" height="300">
<br>

#### GRAD-CAM
<img src="https://user-images.githubusercontent.com/36736904/86006580-2723db00-ba51-11ea-9d84-76f49b15721b.png" height="300">
<br>

## 어플리케이션 적용 결과
유튜브 영상 참고

<img src="https://user-images.githubusercontent.com/36736904/86006744-605c4b00-ba51-11ea-8b1e-b72252a15df2.png" height="300">
<img src="https://user-images.githubusercontent.com/36736904/86007009-cb0d8680-ba51-11ea-9ffe-e7d6f5b041b3.png" height="300">

#### 카메라로 이미지를 촬영한 후 결과를 바로 확인할 수 있음
#### 사진첩의 이미지를 물체 중심으로 크롭해 넣어 결과를 바로 확인할 수 있음
#### 재활용품을 동영상 촬영해 실시간으로 어떤 종류의 재활용품인지 판단 가능


