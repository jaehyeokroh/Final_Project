# Tumor Classification Project

## Overview
이 프로젝트는 뇌 종양 이미지를 네 가지 카테고리로 분류하는 것이 목표입니다: glioma_tumor, meningioma_tumor, no_tumor, pituitary_tumor. 이 분류는 k-최근접 이웃(KNN) 알고리즘을 사용하여 수행할 예정입니다.
***
## Project Description
이 프로젝트의 주요 목표는 뇌 종양 이미지를 정확하게 분류할 수 있는 머신 러닝 모델을 개발하는 것입니다. Training 및 Testing Dataset은 네 가지 종양 유형을 나타내는 클래스로 구성된 이미지로 구성되어 있습니다.
***
## Training Dataset
Training Dataset은 각 종양 유형에 대한 하위 디렉터리로 구성되어 있습니다

-glioma_tumor

-meningioma_tumor

-no_tumor

-pituitary_tumor

각 하위 디렉터리에는 해당 범주에 속하는 뇌 종양의 이미지가 포함되어 있습니다. 이미지는 로드되어 표준화된 크기인 64x64 픽셀로 크기를 조정합니다.
***
## Algorithm
종양 분류에는 k-최근접 이웃(KNN) 알고리즘을 선택하였습니다. KNN은 데이터 포인트를 주변 k개 이웃의 주류 클래스를 기반으로 분류하는 간단하고 효과적인 머신러닝 알고리즘입니다. 이 프로젝트에서는 scikit-learn 라이브러리의 KNeighborsClassifier를 사용하여 KNN 알고리즘을 구현했습니다.
***
## Hyper-parameters
KNN 알고리즘의 주요 Hyper-parameters 입니다.

n_neighbors: 분류 중에 고려할 이웃의 수입니다. 이 프로젝트에서는 n_neighbors를 2로 설정했습니다.
weights: 예측에 사용되는 가중치 함수입니다. 'distance' 값은 가까운 이웃이 먼 이웃보다 더 큰 영향을 미친다는 것을 나타냅니다.
p: Minkowski 거리 측정을 위한 전원 매개변수입니다. 값이 1이면 맨해튼 거리를 나타냅니다. 이 프로젝트에서는 p를 1로 설정했습니다.
***
## Contact
작성자: 노재혁

학번: 20236707

이메일: nojh4237@cau.ac.kr
***
## License
This project is licensed under the MIT License.

