# ML-Linear-Regression-Python-Implementaion







$y = mx + b$ 

For a given x, I want to predict the best possible y. In order to do that I want to have sucha  good combination of m and b that will help me to get the best possible y. 

The only thing that we can influence in b and m. We cant chage the x since it is a given data. 


Mean Squared Error:<br>
$E = \frac{1}{n}\sum_{i =1}^{n}(y_i - \hat{y_i})^{2}$ <br>
$  = \frac{1}{n}\sum_{i =1}^{n}(y_i - (wx + b))^{2}$


We need to change w and b to minimize the error.

How to do that ? <br>

$\frac{\partial E}{\partial w} = \frac{1}{n}\sum_{i = 1}^{n} 2(y_i - (wx_i + b)) (-x_i)$ <br>
$\frac{\partial E}{\partial w} = -\frac{2}{n}\sum_{i = 1}^{n} (x_i)(y_i - (wx_i + b)) $

<br>

$\frac{\partial E}{\partial b} = -\frac{2}{n}\sum_{i = 1}^{n}(y_i - (wx_i + b)) $


<br>
$\bbox[orange, 8px]{w = w -\alpha\frac{\partial E }{\partial w}}$
<br>
$\bbox[orange, 8px]{b = b -\alpha\frac{\partial E }{\partial b}}$

<hr>
$\alpha = \text{Learning Rate}$
