# I-vetors-SVM
SVM model using i-vector. <br>
AI-Hub에 등재된 정신건강진단 및 예측을 위한 멀티모달 데이터 학습모델. <br>
Link URL : <a href="https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=573">AI-Hub</a><br>
[go](https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=573){:target="_blank" rel="noopener noreferrer"} 
## i-vectors
전체 가변 행렬을 이용해 GSV(Gaussian Mixture Model Super Vector)를 낮은 차수로 표현함. <br>
즉, Gaussian mixture model (GMM) 슈퍼벡터를 하나의 Total-variability 공간으로 표현함. <br> <br>

다차원의 벡터형태를 200에서 400차원의 형태로 변환.<br>
대상화자가 아닌 일반적인 배경 화자들의 발성 특징 분포를 표현하는 하나의 모델(UBM)을 통해서 평균만 재학습해서 나온 다차원의 GSV를 200~400차원의 i-vector(identity vector) 형태로 변환하는 작업을 말함.
><a href="https://www.slideshare.net/NaverEngineering/ss-117073508">References</a>

#### kaldi(pykaldi)라는 Python에서 제공하는 툴로 추출이 가능함.  
><a href="https://kaldi-asr.org/doc/">kaldi</a>

## i-vector history
![image](https://user-images.githubusercontent.com/57596337/150733209-4acbd21d-6679-4d00-9239-17d14335a4ce.png)
## Supervised domain adaptation for i-vector based speaker recognition.
![image](https://user-images.githubusercontent.com/57596337/150732732-47821709-af78-4942-ba50-a96e9ce1b969.png)

## Purpose
추출한 i-vector 특징을 SVM으로 학습시켜 정확도(pos label, f1-score etc..)를 검증.



