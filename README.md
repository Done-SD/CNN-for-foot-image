# CNN-for-foot-image
CNN 알고리즘을 활용하여 족저압 분류에 사용하는 코드입니다.


## 라이브러리
Python 3.8.3 에서 작동을 확인하였으며 사용된 라이브러리로는
pytorch, numpy, matplotlib, torchvision, torch입니다.


## 사용 환경
해당 프로그램은 Tekscan 사의 F-scan 장비를 활용하여 얻은 한쪽 발의 족저압 값을
60*21 이미지로 만들어 사용하는 알고리즘들입니다.
사용 도중에 60*60으로 리사이징 후 딥러닝 알고리즘에 사용하며
이러한 사이즈의 특징때문에 해당 알고리즘에서 쌓을 수 있는 최대의 깊이로 쌓았습니다.

dataset/train/ 
dataset/valid/
경로의 폴더 안에 폴더 안에 In/Out으로 구분한 폴더에
In-toeing 보행과 Out-toeing 보행의 족저압 데이터를 넣어서 사용 가능합니다.


## resNet18forfootimg.ipynb
해당 파일은 resNet18 알고리즘을 활용하여 족저압 이미지를 분류하는 코드입니다.
해당 코드는 공개되어있는 ResNet18 코드와 같은 알고리즘을 사용합니다.


## vgg16footimg.ipynb
해당 파일은 VGGNet16 알고리즘을 활용하여 족저압 이미지를 분류하는 코드입니다.
해당 코드는 공개되어있는 VGG16의 구조대로 만들었으며 fc레이어의 변인 수를 제외하면
공개되어있는 VGG16 코드와 유사합니다.
