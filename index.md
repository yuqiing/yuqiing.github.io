# 向量介绍

---

## 1.1 向量和线性组合

- 二维空间中的向量具有两个分量

![image-20220109162601224](https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109162608.png)

- 向量的两个基本运算：向量加法、标量向量乘法

![image-20220109162624503](https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109162624.png)

![image-20220109162639465](https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109162639.png)

![image-20220109163856694](https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109163856.png)

- 将向量和标量的乘法与向量加法结合，得到的就是线性组合**linear combination**，比如两个向量的线性组合$c \boldsymbol{v}+d \boldsymbol{w}$，三个向量的线性组合$c \boldsymbol{u}+d \boldsymbol{v}+e \boldsymbol{w}$

- 在三维空间中，$\boldsymbol{u}$的所用线性组合组成一条直线，$\boldsymbol{u},\boldsymbol{v}$的所有线性组合组成一个平面，$\boldsymbol{u},\boldsymbol{v},\boldsymbol{w}$的所有线性组合充满整个三维空间（需要限制三个向量都不是零向量，都不共线，任一个向量不在其他两个向量构成的平面上）

## 1.2 向量的模和点积

- 点积：$\boldsymbol{v} \cdot \boldsymbol{w}=v_{1} w_{1}+v_{2} w_{2}$，注意结果是**标量**

> 一种对点积的应用理解：可以把原点看作跷跷板的支点，$\boldsymbol{v}$可以看作用来记录两边的孩子到支点的距离的向量， $\boldsymbol{w}$可以看作用来记录两边的孩子的重量的向量，点积的结果就是矩moments，当矩为0时，跷跷板平衡，比如$\left(v_{1}, v_{2}\right)=(-1,2),\left(w_{1}, w_{2}\right)=(4,2),w_{1} v_{1}+w_{2} v_{2}=0$![image-20220109164510983](https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109164511.png)

- 模(length)：length $=\|\boldsymbol{v}\|=\sqrt{\boldsymbol{v} \cdot \boldsymbol{v}}=\left(v_{1}^{2}+v_{2}^{2}+\cdots+v_{n}^{2}\right)^{1 / 2}$

- 单位向量(unit vector)：模为1的向量
- 求向量$\boldsymbol{v}$的单位向量$\boldsymbol{u}$：$\boldsymbol{u} =\boldsymbol{v} /\| \boldsymbol{v}\|$

- 对于相互垂直的向量
  - $\boldsymbol{v} \cdot \boldsymbol{w}=0$
  - $\|\boldsymbol{v}\|^{2}+\|\boldsymbol{w}\|^{2}=\|\boldsymbol{v}-\boldsymbol{w}\|^{2}$

![image-20220109165741101](https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109165741.png)

- 余弦公式：<img src="https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109170125.png" alt="image-20220109170125556" style="zoom: 50%;" />

> <img src="https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109171029.png" alt="image-20220109171029140" style="zoom:50%;" />
>
> 由图易得$\cos \alpha=v_{1} /\|\boldsymbol{v}\|$，$\sin \alpha=v_{2} /\|\boldsymbol{v}\|$，同理$\cos \beta=w_{1} /\|\boldsymbol{w}\|$，$\sin \beta=w_{2} /\|\boldsymbol{w}\|$，两向量的夹角$\theta = \beta - \alpha$，由三角公式$\cos (\beta - \alpha) = \cos \beta \cos \alpha+\sin \beta \sin \alpha$得
>
> ![image-20220109171537398](https://imgbed-1305362743.cos.ap-nanjing.myqcloud.com//picgo20220109171537.png)

- 施瓦兹不等式（Schwarz Inequality）：$|\boldsymbol{v} \cdot \boldsymbol{w}| \leq\|\boldsymbol{v}\|\|\boldsymbol{w}\|$（由$\cos \theta$的绝对值不大于1）
- 三角不等式：$\|\boldsymbol{v}+\boldsymbol{w}\| \leq\|\boldsymbol{v}\|+\|\boldsymbol{w}\|$

- 几何平均数不大于算术平均数：$\sqrt{x y} \leq \frac{x+y}{2}$

> 将$\boldsymbol{v}=(a, b)$ 和 $\boldsymbol{w}=(b, a)$代入三角不等式，得到$2 a b<a^{2}+b^{2}$，得到$a b \leq \frac{a^{2}+b^{2}}{2}$，代入$x=a^{2}$ 和 $y=b^{2}$得到$\sqrt{x y} \leq \frac{x+y}{2}$

> 在$n$维空间中，至多有$n+1$个向量可以互相之间的夹角大于90度

## 1.3 矩阵





