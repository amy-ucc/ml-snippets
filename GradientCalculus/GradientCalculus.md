<font color='yellow'>**Written answer:**

$\: \hat{\mathbf{y}} = \mathbf{X.^2} \hat{\beta}\:$  

$\hat{y_i} = b_0 + b_1x_i$

$L_3(\hat{\beta}) = \sum_{i=1}^{n} ({y_i-\hat{y_i}})^2$

$L_3(\hat{\beta}) = \sum_{i=1}^{n} ({y_i - b_0 - b_1x_i})^2$

r = residuals   
For every i wrt $b_1$:  

$\frac{\partial L_3}{\partial b_1} = \frac{\partial L_3}{\partial u} \frac{\partial u}{\partial b_1} = -2(y_i - b_0 - b_1x_i)x_i$

$= -2(y_i - \hat{y_i})x_i$

$= -2(r_i)^2(x_i)$  

sum all i:

$\sum_{i=1}^{n}(-2(r_i)(x_i))$  
  
For every i wrt $b_0$:  

$\frac{\partial L_3}{\partial b_0} = \frac{\partial L_3}{\partial u} \frac{\partial u}{\partial b_0} = -2(y_i - b_0 - b_1x_i)$

$= -2(y_i - \hat{y_i})$

$= -2(r_i)$ 
 
sum all i:

$\sum_{i=1}^{n} (-2(r_i))$


Gradient:

$\bigtriangledown = \begin{bmatrix} \sum_{i=1}^{n} (-2(r_i))  \\ \sum_{i=1}^{n}(-2(r_i)(x_i)) \end{bmatrix}$


</font>