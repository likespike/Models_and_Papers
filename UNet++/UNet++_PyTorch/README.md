# 출처
- https://github.com/4uiiurz1/pytorch-nested-unet


# 수정 사항
- git clone 관련 추가
- kaggle API로 dataset 다운 관련 추가
- Albumentations 부분
    - import albumentations 부분
    - FutureWarning 관련 augmentations 수정

 # prtrained_model 저장 위치
- https://drive.google.com/drive/folders/1KCEVGK33SRQLWCIRoJ95imEyz0xqgeqD?usp=sharing



# 개론
- U-Net이후의 seminal model인 DenseNet (CVPR 2017) 차용
    - ResNet이후 대부분의 task에서 성능을 올릴 수 있는 아키텍쳐 구조로 인정받음 
    - skip connection을 다음 블럭, 다다음 블럭, ... 식으로 넘겨주는 구조
        - 네트워크 구성: 이런 dense block을 몇 개 쌓았냐


# 구현 방법
- Nested dense convolutional blocks (중첩된 밀집 학성곱 블럭)
