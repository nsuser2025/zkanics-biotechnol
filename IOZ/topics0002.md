#### IOZのLegendre多項式展開

<p>
$\theta_{1} = 0$, $\phi_{1} = 0$, $\phi_{2} = 0$ のときは
</p>

$$
\begin{align}
&{\bf e}\_{2} = (\sin\theta\_{2}, 0, \cos\theta\_{2}) \\\\
&{\bf e}\_{3} = (\sin\theta\_{3}\cos\phi\_{3}, \sin\theta\_{3}\sin\phi\_{3}, \cos\theta\_{3}) \\\\
&\cos\theta\_{32} = {\bf e}\_{2}\cdot{\bf e}\_{3} = \cos\theta\_{2}\cos\theta\_{3}
                    + \sin\theta\_{2}\sin\theta\_{3}\cos\phi\_{3} \tag{1}
\end{align}
$$

<p>
$x \equiv \cos\theta$ とすると
</p>

$$
\begin{align}
t(r\_{1},r\_{2},x\_{2})
&= \int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} ~\rho(r\_{3})
\int^{2\pi}\_{0} d\phi\_{3} \int^{1}\_{-1} dx\_{3}
~c(r\_{1},r\_{3},x\_{3}) ~h(r\_{3},r\_{2},x\_{32}) \tag{2}
\end{align}
$$

<p>
（2）のLegendre多項式展開
</p>

$$
\begin{align}
c(r\_{1},r\_{3},x\_{3})
&= \sum\_{i} \hat c\_{i}(r\_{1},r\_{3}) ~P\_{i}(x\_{3}) \tag{3} \\\\
h(r\_{3},r\_{2},x\_{32})
&= \sum\_{j} \hat h\_{j}(r\_{3},r\_{2}) ~\color{red}{P\_{j}(x\_{32})} \\\\
&= \sum\_{j} \hat h\_{j}(r\_{3},r\_{2}) ~\color{green}{P\_{j}(x\_{2})P\_{j}(x\_{3})} \tag{4} 
\end{align}
$$

$$
\begin{align}
\hat t\_{n}(r\_{1},r\_{2})
&= \frac{2n+1}{2} \sum\_{ij} \int^{1}\_{-1} dx\_{2}
\int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} \int^{2\pi}\_{0} d\phi\_{3}
\int^{1}\_{-1} dx\_{3} ~\hat c\_{i}(r\_{1},r\_{3}) ~\rho(r\_{3}) \\\\
&\times \hat h\_{j}(r\_{3},r\_{2}) 
~\color{red}{P\_{n}(x\_{2})P\_{j}(x\_{2})P\_{i}(x\_{3})P\_{j}(x\_{3})} \\\\ \\\\
&= \frac{2n+1}{2} \int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} \int^{2\pi}\_{0} d\phi\_{3}
~\hat c\_{n}(r\_{1},r\_{3}) ~\rho(r\_{3}) ~\hat h\_{n}(r\_{3},r\_{2})
\color{green}{\biggl(\frac{2}{2n+1}\biggr)^{2}} \\\\ \\\\
&= \frac{4\pi}{2n+1} \int^{\infty}\_{0} dr\_{3} ~r^{2}\_{3} 
~\hat c\_{n}(r\_{1},r\_{3}) ~\rho(r\_{3}) ~\hat h\_{n}(r\_{3},r\_{2}) \tag{5}
\end{align}
$$

<p>
<span style="color:blue">
※ Legendre多項式展開
</span>  
</p>

$$
\color{blue}{
\begin{align}
f(x) &= \sum^{\infty}\_{n=0} \hat f\_{n} P\_{n}(x) \tag{6} \\\\
\hat f\_{n} &= \frac{2n+1}{2} \int^{1}\_{-1} dx ~f(x)P_{n}(x) \tag{7}
\end{align}
}
$$

<p>
<span style="color:blue">
※ Legendre多項式の直交性
</span>  
</p>

$$
\color{blue}{
\begin{align}
\int^{1}\_{-1} dx ~P\_{n}(x) P\_{m}(x) = \frac{2}{2n+1} \delta\_{mn} \tag{8}
\end{align}
}
$$

<p>
<span style="color:blue">
※ Legendre多項式の加法定理  
</span>  
</p>

$$
\color{blue}{
\begin{align}
P\_{j}(x\_{32})
&= P\_{j}(x\_{2})P\_{j}(x\_{3}) + 2 \sum^{j}\_{m=1}
\frac{(j-m)!}{(j+m)!} P^{m}\_{j}(x\_{2})P^{m}\_{j}(x\_{3}) \cos [m(\phi\_{2}-\phi\_{3})] \tag{9}
\end{align}
}
$$

<p>
<span style="color:blue">
$P^{m}_{j}$: Legendre陪多項式（Associated Legendre polynomial） 
</span>  
</p>

<p>
<span style="color:blue">
$\phi_{2}=0$のとき, (9)の右辺第2項は $\int^{2\pi}_{0} d\phi_{3}$ でゼロになる.
</span>  
</p>

---
