**15.1) Integrais Duplas sobre Retângulos** (Questão 1)

**Valor Médio**
$$f_{medio} = \frac{1}{A(R)} \int _{R}\int f(x,y)dA$$
$A(R)$ é a área de $R$
---
**15.5) Aplicações de Integrais Duplas**
**Função densidade do produto** (Questão 4)
$$h(x,y)=f(x,y)g(x,y)$$


**Probabilidade com variáveis contínuas independentes**
- A densidade conjunta é:
$$
f_{X,\alpha}(x,\alpha) = f_X(x)\,f_\alpha(\alpha)
$$
- Para calcular a probabilidade de um evento \(A\), integra-se a densidade conjunta sobre a região correspondente:
$$
P(A) = \iint_A f_{X,\alpha}(x,\alpha)\,dx\,d\alpha
$$
- Se $X \sim U(a,b)$, então:
$$
f_X(x) = \frac{1}{b-a}, \quad a \leq x \leq b
$$
- Se $\alpha \sim U(0,\pi)$$, então:
$$
f_\alpha(\alpha) = \frac{1}{\pi}, \quad 0 \leq \alpha \leq \pi
$$

**Estratégia**
Barra de comprimento $2$ em avenida de largura $10$. Sejam $(X \sim U(0,5))$ e $\alpha \sim U(0,\pi)$ 

1. Função densidade de probabilidade:
	1. $f(x) = \frac{1}{5} se \space 0 \leq x\leq 5$
	2. $f(x) = 0$ se caso contrário
	3. $f(\alpha) = \frac{1}{\pi} se \space 0 \leq \alpha\leq \pi$
	4. $f(\alpha) = 0$ se caso contrário

2. (Intervalo). A barra cabe inteira se:  
$$
X + \sin\alpha \leq 5
$$

3. A probabilidade é $P(A) = \int _{A}\int x,\alpha f(x,\alpha)dxd\alpha$:  
$$
P = \int_0^\pi \int_0^{5-\sin\alpha} \frac{1}{5\pi}\,dx\,d\alpha
$$
4. Integrando em $x$:
$$
P = \frac{1}{5\pi} \int_0^\pi (5 - \sin\alpha)\,d\alpha
$$
$$
P = \frac{1}{5\pi}(5\pi - 2)
$$
$$
P = 1 - \frac{2}{5\pi}
$$
$$
P = 1 - \frac{2}{5\pi} \approx 0.8727
$$
---
**15.10) Mudança de Variáveis em Integrais Múltiplas** (Questão 2)
**Determinante Jacobiano**
$$J = \begin{bmatrix} \frac{\partial x}{\partial u} & \frac{\partial x}{\partial v} \\\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v} \\\end{bmatrix}$$

**Estratégia**
* Calcular o volume entre $z=0$ e $z = 1 - \frac{x^2}{4}-\tfrac{y^2}{9}$

1. Interseção do plano $z$ com o paraboloide:
$$
\frac{x^2}{4} + \frac{y^2}{9} \leq 1
$$

2. Mudança de variáveis sugerida:
$$
u = \frac{x}{2}, \quad v = \frac{y}{3} \quad \Rightarrow \quad x = 2u, \; y = 3v
$$

3. O determinante Jacobiano:  
$$
J = \begin{bmatrix} \frac{\partial x}{\partial u} & \frac{\partial x}{\partial v} \\\frac{\partial y}{\partial u} & \frac{\partial y}{\partial v} \\\end{bmatrix} = \begin{bmatrix} 2 & 0\\ 0 &3\end{bmatrix} =6
$$
4. Integração original:

$$
V = \iint_{u^2+v^2 \leq 1} 6(1 - u^2 - v^2)\,du\,dv
$$

5. Passando para coordenadas polares $u = r\cos\theta,\; v = r\sin\theta$:  2
$$
V = \int_0^{2\pi} \int_0^1 6(1-r^2)r\,dr\,d\theta =
\int_0^1 6(1-r^2)r\,dr = \frac{\pi}{2}
$$
$$
V = 3\pi
$$
