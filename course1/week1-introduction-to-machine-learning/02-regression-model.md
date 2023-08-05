# Linear Regression with one variable
variable이 1개인 선형 회귀(linear regression)는 Univariate linear regression이라고 부르기도 한다.
- Uni : 라틴어로 one을 의미
- Variate : variable을 의미

## why are we choosing a linear function?
Since linear function is relatively simple and easy to work with, it gives us a foundation. Foundation will help us to get more complex models

## Desiging a learning algorithm
Learning algorithm will produce __some function__

### how to represent function, $f$ for Linear Regression with one variable?
$$f_{w,b}(x) = wx + b$$
Simpler notation
$$f(x)$$

$f(x)$ is a function that takes $x$ as input, and depending on the values of $w$ and $b$, $f(x)$ will output some value of a prediction $\hat{y}$

$w$ and $b$ are __parameters__