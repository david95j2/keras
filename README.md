# keras 창시자에게 배우는 딥러닝

목차별로 따라하기

keras는 Python언어로 만들어진 high-level api 로 다시 말해 Tensorflow 위에 얹어서 사용하는 library 이다. 
Google 에서 지원하고 Pytorch 위에는 못 얹는다. 
또한 상대적으로 쉽다고 알려져 있다.

---
---

1. 사용자 친화적
케라스는 일반 사용 사례에 최적화된 간단하고 일관적인 인터페이스를 제공합니다. 이는 사용자 오류에 대해 명확하고 실용적인 피드백을 제공합니다.
 
2. 모듈화 및 구성 가능성
케라스 모델은 구성 요소의 설정에 의해 연결되는 식으로 거의 제한없이 만들 수 있습니다.
 
3. 쉬운 확장
연구를 위한 새로운 아이디어를 표현하기 위해 사용자 정의 설계 블록을 작성하면, 새로운 층(layers), 지표(metrics), 손실 함수를 생성하고 최첨단 모델을 개발할 수 있습니다.

---

1. 케라스는 개발자 경험을 우선시한다.

2. 케라스는 업계 뿐만 아니라 다양한 연구 커뮤니티에서 폭넓게 사용하고 있습니다.

3. 케라스는 모델을 쉽게 제품으로 바꿀 수 있습니다.

4. 케라스는 강력한 멀티 GPU 및 분산 처리 지원이 가능합니다


> import tensorflow as tf 
>
> tf.test.is_gpu_available()
> True
>
> tf.test.gpu_device_name() # 결과로 나오는 GPU는 본인 pc 설정에 따라 다를 수 있다.
>
> '/device:GPU:0'
>
> tf.config.experimental.list_physical_devices(device_type='GPU') # GPU가 어려 개 일 때 
>
> [PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')]


---

### ERROR 일지

> ImportError: cannot import name 'to_categorical' from 'keras.utils' 
>
> 해결책 : from tensorflow.keras.utils import to_categorical
>