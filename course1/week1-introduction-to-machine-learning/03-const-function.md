# Cost function
Cost function will tell us how well the model is doing so that we can try to get it to do better. 
- how well the model is doing : 모델이 얼마나 잘 하고 있는 지

## Parameters
아래의 model에서 $w$와 $b$는 모델의 파라미터이다. 
$$f_{w,b}(x) = wx + b$$
[Learn more about parameters](https://github.com/jeon-yewon/Machine-Learning-Specialization/blob/main/course1/week1-introduction-to-machine-learning/a01-paramter-and-variable.md)

### Find parameters($w$,$b$)
- 모든 $(x^{(i)}, y^{(i)})에 대해 $예측 값 $\hat{y}^{(i)}$이 실제 target 값인 $y^(i)$에 가까운 값이 될 수 있도록하는 $w$, $b$를 찾는다
- 즉, how to measure how well a line __fits__ the training data

## Cost Function Formula
예측값 $\hat{y}$에서 실제 target 값인 $y$를 뺀 결과 값을 __error__ 또는 오차라고 한다.이때 오차 값을 제곱하면 __squared of the error__ 라고 한다.

따라서 training set 전체에 대한 squared of the error는 아래의 식으로 계산할 수 있다.
$$\sum_{i=1}^{m}(\hat{y}^{(i)} - y^{(i)})^2$$

그런데 위의 식에서 $m$ 즉 training example 개수가 더 많아지면 결과 값이 더욱 커진다. 그래서 전체 error 값의 합이 아닌 평균 값을 사용한다.

By conevention, people use
$$J(w,b) = \frac{1}{2m} * \sum_{i=1}^{m}(\hat{y}^{(i)} - y^{(i)})^2$$

and also use
$$J(w,b) = \frac{1}{2m} * \sum_{i=1}^{m}(f_{w,b}(x^{(i)}) - y^{(i)})^2$$

이때의 cost function은 Squared error cost function이라고 부른다. 이 말은, 다른 방식으로 계산하는 cost function이 있다는 말이다. Squared error cost funtion은 linear regression에서 보편적으로 가장 많이 사용되는 cost function이다. 

## Cost Function Intuition
Squared error cost function에서 우리는 가장 적은 결과 값을 가지는 Cost function $J$를 찾는다.