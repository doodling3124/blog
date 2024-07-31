---
title: "一元线性回归"
lastmod: 2024-07-26T21:53:39+08:00
draft: false
tags: [机器学习]
---

回归函数:$$f_{w,b}(x) = wx + b$$
代价函数:$$J(w,b) = \frac{1}{2m}\sum_{i=1}^m(f_{w,b}(x_i)-y_i)^2$$ 
梯度下降法同时更新w和b:  
$$tmp_w=w-\alpha\frac{\partial J(w,b)}{\partial w}=w-\alpha\frac{1}{m}\sum_{i=1}^m(f_{w,b}(x_i)-y_i)x_i$$
$$tmp_b=b-\alpha\frac{\partial J(w,b)}{\partial b}=b-\alpha\frac{1}{m}\sum_{i=1}^m(f_{w,b}(x_i)-y_i)$$
$$w = tmp_w$$
$$b = tmp_b$$

\\(\alpha\\)是学习率,用来控制下降幅度
