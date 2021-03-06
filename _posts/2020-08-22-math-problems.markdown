---
layout: post
title:  "一些数学问题 loading..."
date:   2020-08-22 14:56:29 +0800
categories: math
---

### 1.收敛【convergence】

收敛类型有收敛数列、函数收敛、全局收敛、局部收敛。



**收敛数列**：令{An}为一个数列，且a为一个固定实数，如果对于任意给出的b>0,存在一个正整数N，使得对于任意n>N, 有|An-a|<b恒成立，就称数列{An}收敛于a（极限为a），即数列{An}为收敛数列。



**函数收敛**：定义方式与数列收敛类似。柯西收敛准则：关于函数f(x)在点x0处的收敛定义。对于任意实数b>0,存在c>0,对任意x1,x2满足0<|x1-x0|<c,0<|x2-x0|<c,有|f(x1)-f(x2)|<b。

收敛的定义方式很好的体现了数学分析的精神实质。

如果给定一个定义在区间i上的函数列，u1(x）， u2（x） ，u3（x）......至un（x）....... 则由这函数列构成的表达式u1（x）+u2（x）+u3（x）+......+un（x）+......⑴称为定义在区间i上的（函数项）无穷级数，简称（函数项）级数
对于每一个确定的值X0∈I,函数项级数 ⑴ 成为常数项级数u1（x0）+u2（x0）+u3（x0）+......+un（x0）+.... （2） 这个级数可能收敛也可能发散。如果级数（2）发散，就称点x0是函数项级数（1）的发散点。函数项级数（1）的收敛点的全体称为他的收敛域 ，发散点的全体称为他的发散域 对应于收敛域内任意一个数x，函数项级数称为一收敛的常数项 级数 ，因而有一确定的和s。这样，在收敛域上 ，函数项级数的和是x的函数S（x），通常称s（x）为函数项级数的和函数，这函数的定义域就是级数的收敛域，并写成S（x）=u1（x）+u2（x）+u3（x）+......+un（x）+......把函数项级数 ⑴ 的前n项部分和 记作Sn(x)，则在收敛域上有lim n→∞Sn(x)=S(x)
记rn(x)=S(x)-Sn(x),rn(x)叫作函数级数项的余项 （当然，只有x在收敛域上rn（x）才有意义，并有lim n→∞rn (x)=0

**迭代算法的敛散性**：

1.全局收敛：对于任意的X0∈[a,b],由迭代式Xk+1=φ（Xk）所产生的点列收敛，即其当k→∞时，Xk的极限趋于X*，则称Xk+1=φ（Xk）在[a，b]上收敛于X*。
2.局部收敛
若存在X*在某邻域R={X| |X-X*|<δ},对任何的X0∈R，由Xk+1=φ（Xk）所产生的点列收敛，则称Xk+1=φ（Xk）在R上收敛于X*。

### 2.证明lim(x->+∞)（1+1/x）^x=e

![image001](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/math/image001.png)

![image002](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/math/image002.png)

![image003](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/math/image003.png)

### 3.均值不等式原理

![image004](https://raw.githubusercontent.com/WELLINGWANG/WELLINGWANG.github.io/master/images/math/image004.png)

