# ML-Linear-Regression-Python-Implementaion







$y = wx + b$ 

For a given x, I want to predict the best possible y. In order to do that I want to have such a  good combination of w and b that will help me to get the best possible y. 

The only thing that we can influence in b and m. We cant chage the x since it is a given data. 


Mean Squared Error:<br>
$J = \frac{1}{n}\sum_{i =1}^{m}(\hat{y_i} - y_i)^{2}$ <br>
$  = \frac{1}{n}\sum_{i =1}^{m}((wx + b) -y_i)^{2}$


We need to change w and b to minimize the error.

How to do that ? <br>

$\frac{\partial J}{\partial w} = \frac{1}{m}\sum_{i = 1}^{m} ((wx_i + b) - y_i) (x_i)$ <br>
$\frac{\partial J}{\partial w} = \frac{1}{m}\sum_{i = 1}^{m} (x_i)((wx_i + b) - y_i) $

<br>

$\frac{\partial J}{\partial b} = \frac{1}{m}\sum_{i = 1}^{m}((wx_i + b) - y_i) $


<br>
$\bbox[orange, 8px]{w = w -\alpha\frac{\partial J }{\partial w}}$
<br>
$\bbox[orange, 8px]{b = b -\alpha\frac{\partial J }{\partial b}}$

<hr>
$\alpha = \text{Learning Rate}$
