# Gradient descent : Derivative
앞선 강의를 통해, gradient descent algoritm에서 $\alpha$ 와 derivative term이 의미하는 바를 확인했다. 이번에는 derivative term를 더 깊게 공부해보려 한다.
- $\alpha$ : learning rate -> how big of a step
- derivative term -> direction

## with one parameter
조금 더 직관적으로 이해하기 위해 parameter가 1개 예시를 사용한다. parameter $w$의 cost function은 다음과 같이 나타낼 수 있다.
$$ J(w) $$
- [ ] TBD : 이미지 넣기

gradient descent은 다음과 같이 표현할 수 있다.
$$ w = w - \alpha \frac{d}{dw} J(w) $$
우리의 큰 목표는 parameter $w$ 를 조절하여 cost를 최고화 하는 것이다.

### derivative term here means
- [ ] TBD : 이미지 넣기
선의 기울기(the slope)는 $J(w)$ 함수의 이 점(this point)에서의 derivative 이다.

**if this derivative is a positive number**
- [ ] TBD : 이미지 넣기
- $w$는 다음 식의 값으로 업데이트 된다. $w = w - \alpha * (positive number) $
- $\alpha$ (learning rate)는 항상 positive 값을 가진다.
- 결국, 새롭게 업데이트 된 $w$ 의 값은 작아진다(smaller)

w의 값이 작아졌기 때문에 왼쪽으로 이동하게 되며, 그래프를 보면 cost $J(w)$ 또한 줄어든 것을 알 수 있다. 우리의 목표는 cost $J(w) 를 최소화 하는 것이므로 옳은 방향으로 이동한 것이다. 

**if this derivative is a negative number**
- [ ] TBD : 이미지 넣기
- 결국, 새롭게 업데이트 된 $w$의 값은 증가한다(increasing)

w의 값이 증가했기 때문에 오른쪽으로 이동하게 되며, cost $J(w)$ 는 감소했다.
