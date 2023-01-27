# AlexNet Paper Review

## 6 Result
우리 네트워크는 top-1 과 top-5 테스트 오류율에서 각각 37.5% 와 17.0%를 달성했다.

우리는 또한 우리의 모델을 ILSVRC-2012 대회에 입력하였고 이 결과는 Table 2에 기록한 것이다.
ILSVRC-2012 테스트셋 레이블들은 공식적으로 사용이 가능하지 않기 때문에 우리는 우리가 시도한 모든 모델에 대한 테스트 오류율을 기록할 수 없었다.
이 도표의 남은 부분중에서, 우리는 Validation과 Test Set의 오류 비율을 상호교환할수 있게 사용한다 왜냐하면 우리의 경험에서 그것들은 0.1%보다 많게는 다르지 않았기 때문이다.
다섯개의 비슷한 CNN들의 예측들을 평균낸것은 16.4%의 오류율을 나타내었다.
ImageNet Fall 2011(15M images,22K categories) release된 전체를 분류하기 위해 마지막 pooling layer에 6번째 Convolutional layer 추가한 하나의 CNN을 학습하고 그리고 나서 그것을 ILSVRC-2012 에 "fine-tuning" 한것은 16.6%의 오류율을 나타내었다.
CNN 2개의 예측들을 평균낸 것은 Fall 2011에 release된 전체 데이터로 앞서 언급한 5개의 CNN들과 함께 pre-trained 되었고 그것들은 15.3%의 오류율을 나타내었다.
두번째로 우수한 대회 출품작은 26.2%의 오류율을 달성하였다.

마지막으로 우리는 또한 ImageNet의 Fall 2009 버전에서의 우리의 오류율을 기록하였다.
이 데이터셋에서 우리는 이미지들의 반은 훈련에 사용하고 반은 테스팅에 사용하는 문헌의 관례를 따랐다.
테스트셋으로 설립된것이 없었기 때문에 우리의 split은 이전 저자들이 사용한 split와는 필연적으로 다를것이다.
그러나 이것은 결과에 눈에 띄게 영향을 주진 않았다.
우리의 top-1 and top-5 오류율은 이 데이터셋에서 각각  67.4% 와 40.9% 이고 위에 묘사된 네트워크 그러나 마지막 Pooling layer에 여섯번째 Convolution layer가 추가된 것으로 이러한 오류율을 얻었다.
이 데이터셋에서 최고 성능은 각각 top-1 ,top-5 오류율이 78.1% 와 60.9% 였던 것이다.
