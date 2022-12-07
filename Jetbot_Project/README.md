# 시각장애인을 위한 도로 안내 로봇
> 안내견의 역할을 대신하여 시각장애인에게 길을 안내하는 로봇

- 시각장애인들은 현재 훈련된 안내견을 통해 길을 안내받고 위험을 대비한다. 하지만, 안내견이 대형견이라는 이유로 위험한 존재로 여겨지거나 출입을 거부당하는 등 안내견을 동반하는 시각장애인들이 '출입 거부' 및 '차가운 시선'과 같은 고충을 겪고 있음을 여러 사례들로 찾아볼 수 있다.
- 따라서 이러한 문제를 해결하기 위해 로봇을 학습시켜 안내견의 역할을 대신하도록 하여 로봇을 통해 길을 안내 받으면 좋을 것 같다고 생각하여 이러한 아이디어를 제시하게 되었다.



## 구체적인 아이디어
- 현재 안내견은 보통 시각장애인의 왼편에 서기 때문에 Jetbot의 경우에도 시각장애인의 왼편에 있다고 생각하고 장애물을 마주칠 경우 항상 오른쪽으로 피하도록 구현

![small](https://user-images.githubusercontent.com/101259003/206207300-10a541b6-d411-46e2-b8e2-1d3985773b94.gif)

## 실행 방법

1. **Road Following**: [Jetbot Repository](https://github.com/NVIDIA-AI-IOT/jetbot/tree/master/notebooks/road_following)에 제공된 코드를 사용하여 데이터셋을 수집하고 Road Follow 모델을 훈련 및 최적화합니다 .

2. Collision Avoidance: [Jetbot Repository](https://github.com/NVIDIA-AI-IOT/jetbot/tree/master/notebooks/collision_avoidance)에 제공된 코드를 사용하여 데이터셋을 수집하고 Collision Avoidance 모델을 훈련 및 최적화합니다 .

## 사용 예제

직접 학습한 모델을 로드하여 사용

```python
import torch
import torchvision

road_following_model = torchvision.models.resnet18(pretrained=False)
road_following_model.fc = torch.nn.Linear(512,2)
road_following_model.load_state_dict(torch.load('best_rf_model_1207.pth'))

collision_avoidance_model = torchvision.models.alexnet(pretrained=False)
collision_avoidance_model.classifier = torch.nn.Linear(collision_avoidance_model.classifier[6].in_features,2)
collision_avoidance_model.load_state_dict(torch.load('best_model_1207.pth'))
```


<!-- Markdown link & img dfn's -->
[npm-image]: https://img.shields.io/npm/v/datadog-metrics.svg?style=flat-square
[npm-url]: https://npmjs.org/package/datadog-metrics
[npm-downloads]: https://img.shields.io/npm/dm/datadog-metrics.svg?style=flat-square
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[wiki]: https://github.com/yourname/yourproject/wiki
