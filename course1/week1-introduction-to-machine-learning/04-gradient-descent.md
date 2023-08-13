# Gradient Descent
Gradient descent is an algorithm can use to try __to minimize any function__

## How does it work?
1. star with some $w$, $b$

    _*$w$, $b$는 모델의 파라미터이다._

2. Keep changing $w$, $b$ to reduce $J(w,b)$ or any other function
    - spin around 360 degress and decide what **direction** would take you downhill **most quickly**
    - what is the best direction? : Mathmatically, the direction of steepest descent
3. Until we settle at or near a minimum

## Local Minima
Local minima or Local minimum means the bottoms of valleys. Functions can have more than 1 local minima. If you start going down the fist valley, gradient descent _won't_ lead you to the second valley.

## Impementing gradient descent
아래의 식에서는 $w$만을 언급했지만, 다른 parameter도 동일한 식을 사용하여 값을 update 한다.

$$w = w - \alpha \frac{d}{dw} J(w,b)$$
update parameter by taking the current value of parameter and adjusting it a small amount( $ -\alpha \frac{d}{dw} J(w,b) $ )
- $\alpha$ : Learning rate
    - usually a small positive number between 0 and 1
    - controls __how big of a step__ you take down hill
- $\frac{d}{dw} J(w,b)$ : derivative term of the function(in this case, cost function $ J(w,b) $ )
    - tell you in which __direction__ you want to take your baby step


### 중요한 점은
learning rate와 derivative term를 업데이트 하는 이 과정을 algorithm이 수렴(converges)할 때 까지 반복한다는 점이다. algorithm이 수렴하게 된다면, parameter들(위의 예에서는 $w$, $b$)이 더이상 변하지 않는 local minimum에 도달하게 된다.


## Simultaneous update
여러 parameter 값을 조정할 때 동시에 값을 업데이트(simultaneous update) 해야 한다.