# Variable
- variable은 포괄적인 의미 그대로 받아들이면 된다. feature, parameter 모두 모델의 variable이며, 서로 다른 특징을 가지고 있는 variable이다.


# Parameter
- parameter는 모델을 구성하는 요소 중 하나로, 주어진 데이터로부터 parameter의 값을 추정할 수 있다.
- 새로운 데이터를 예측하기 위해 function을 사용하고, 이때 parameter를 필요로 한다. 
- model parameter의 예시
    - artifical neural network의 __weights__
    - support vector machine의 __support vectors__
    - linear regression 또는 logistic regression의 __coefficients__

# Hyperparameter
- hyperparameter는 모델의 외부에 있는 요소로 hyperparameter의 값은 data를 통해 추정할 수 없다
- 주어진 문제에서 모델의 hyperparameter의 최적의 값을 알 수 없다. 
- 경험에 의해 판단하거나(rules of thumb), 다른 예시를 참고하거나, 시행착오를 통해 최적의 값을 탐색한다.
> 많은 모델들은 데이터를 이용해 직접 추정할 수 없는 중요한 파라미터들을 가지고 있다. ... 이러한 유형의 모델 파라미터를 "tuning parameter"라고 부른다. 적절한 값(appropriate value)을 계산할 수 있는 공식이 존재하지 않기 때문이다 - \<Applied Predictive Modeling>
- hyperparameter를 parameter라고 부르는 경우가 있어 종종 헷갈리지만, 만약 parameter를 스스로(manually) 계산해야 한다면 hyperparameter에 해당된다
- hyperparameter의 예시
    - nural network의 __learning rate__
    - support vector machine의 __C, sigma__
    - KNN모델의 __k__

### References
- [datacamp : Hyperparameter Optimization in Machine Learning Models](https://www.datacamp.com/tutorial/parameter-optimization-machine-learning-models)