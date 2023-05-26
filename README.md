# Pytorch를 활용한 UNet 모델링

이 저장소는 U-Net 아키텍처를 사용한 PyTorch CNN(Convolutional Neural Network) 구현을 보여주는 것입니다. 이 저장소는 취업 준비를 위한 포트폴리오로 사용되며, 면접관분들께 좋은 인상을 주기 위해 각 구성 요소에 대한 상세한 설명이 포함되어 있습니다.

## 저장소 내용

저장소에는 다음과 같은 구성 요소들이 포함되어 있습니다:

### 1. `datasets` 폴더

`datasets` 폴더에는 훈련 및 평가에 사용되는 데이터셋이 포함되어 있습니다. 이 데이터셋은 U-Net 모델을 훈련하고 성능을 평가하는 데 필수적입니다.

### 2. `data_read.py`

`data_read.py` 스크립트는 입력 데이터를 읽고 전처리하는 역할을 담당합니다. 데이터셋을 로드하고 필요한 변환 또는 증강을 수행합니다. 

### 3. `dataset.py`

`dataset.py` 스크립트는 PyTorch의 Dataset 클래스를 활용하여 데이터셋을 구성하는 데 사용됩니다. 데이터셋을 로드하고 전처리된 데이터를 모델에 공급합니다.

### 4. `eval.py`

`eval.py` 스크립트는 훈련된 모델을 평가하는 데 사용됩니다. 저장된 모델 파라미터를 로드하고, 정확도, 정밀도, 재현율, F1 스코어 등 다양한 평가 메트릭을 계산합니다. 이 스크립트는 모델의 성능에 대한 포괄적인 분석을 제공합니다.

### 5. `model.py`

`model.py` 스크립트는 U-Net 모델의 구현을 포함하고 있습니다. 이 스크립트는 U-Net 아키텍처를 정의하고 모델의 forward pass를 처리합니다.

### 6. `run_unet.ipynb`

`run_unet.ipynb` 노트북 파일은 U-Net 모델의 실행 예시를 제공합니다. 데이터셋을 로드하고 모델을 초기화하며, 훈련 및 평가 과정을 수행하는 코드를 포함하고 있습니다.

### 7. `train.py`

`train.py` 스크립트는 U-Net 모델을 훈련하는 데 사용됩니다. 데이터 로딩, 모델 초기화, 훈련 루프, 모델 파라미터 저장 등을 처리합니다.

### 8. `util.py`

`util.py` 스크립트에는 유틸리티 함수들이 포함되어 있습니다. 이러한 함수들은 모델 훈련 및 평가에 유용하게 사용될 수 있습니다.

각 구성 요소에 대한 자세한 설명과 사용법은 해당 파일 내에 주석으로 제공되어 있습니다. 추가로, 훈련과 평가에 필요한 데이터셋과 사전 학습된 모델은 `datasets` 폴더와 `model_checkpoint` 폴더에 저장되어 있습니다. 이 저장소를 사용하여 U-Net 모델을 훈련하고 평가할 수 있습니다.

