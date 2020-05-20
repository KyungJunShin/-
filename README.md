진행 

1. 데이터 검사 및 이해
2. 입력 파이프 라인 구축
3. 모델 구축
4. 모델 훈련
5. 모델 테스트
6. 모델 개선 및 프로세스 반복

모델 정리

Sequential : 인공 신경망 챕터에서 입력층, 은닉층, 출력층 등을 구성하기위해 사용

Dense : 전결합층 추가(완전연결 신경망)

Conv2D(합성곱 계층), MaxPooling2D(풀링계층) : 컨볼루션 신경망

Flatten : 리스트 안의 리스트를 하나로 합쳐주는 함수

DropOut : 고의로 랜덤한 뉴런을 누락시킨 후 학습 시작

ImageDataGenerator : 클래스를 통해 객체를 생성할 때 파라미터를 전달해주는 것을 통해 데이터의 전처리를 쉽게할 수 있고, 또 이 객체의 flow_from_directory 메소드를 활용하면 폴더 형태로된 데이터 구조를 바로 가져와서 사용할 수 있다.

모델 순서

Dense -> Conv2D -> Relu or sigmoid -> MaxPooling2D --> 반복 후 SoftMAX추가
