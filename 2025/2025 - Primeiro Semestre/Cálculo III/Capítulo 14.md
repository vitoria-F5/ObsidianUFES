**14.2) Limites e Continuidade** (Questão 5)

Calcule o limite: 
$\lim_{(x,y)\to(0,0)} \frac{x^{2}+y^{2}}{x^{2}+y^{4}}$

**Estratégia**
1. Caminho 1:
$\frac{x^{2}+0}{x^{2}+0} = \frac{x^{2}}{x^{2}} = 1.$
Logo, pelo eixo x, o limite tende a 1.

2. Caminho 2:
$\frac{0+y^{2}}{0+y^{4}} = \frac{y^{2}}{y^{4}} = \frac{1}{y^{2}} \to +\infty \quad (y\to 0).$
Logo, pelo eixo y, o limite tende a 0
---
**14.4) Planos Tangentes e Aproximações Lineares** (Questão 1)
Suponha que $f$ tenha derivadas parciais contínuas. Uma equação do plano tangente à superfície $z = f(x,y)$ no ponto $P(x_{0},y_{0},z_{0})$ é dada por 
$$z - z_{0} = f_{x}(x_{0},y_{0})(x - x_{0} + f_{x}(x_{0},y_{0}))$$

**Estratégia**
Encontrar a equação do plano tangente à superfície $S$ onde $f(x,y,z)= x²+3y²+xz² = 12$ no ponto $(2,0,2)$
4. Calcular $\nabla f$ e  $\nabla f(x_{0},y_{0},z_{0})$
5. Produto $\nabla f(x_{0},y_{0},z_{0})((x,y,z)-(x_{0},y_{0},z_{0}))$
---
**14.5) Regra da Cadeia** (Questão 4)
$$\frac{\partial f}{\partial s}=fx· xs + fy·ys$$
$$\frac{\partial f}{\partial t}=fx· xt + fy·yt$$
-----
**14.7) Valores Máximo e Mínimo** (Questão 3)
Condições para que existam pontos máximos e mínimos
* Gradiente de $f$ precisa ser anular em algum ponto diferente de zero.

**Estratégia**
Determinar valores máximo e mínimo absolutos de uma função contínua $f$ em um conjunto fechado limitado em $D$:
1. Determinar os valores de $f$ nos pontos críticos de $f$ em $D$;
2. Determinar os valores extremos de $f$ na fronteira de $D$;
3. O maior dos valores dos passos 1 e 2 é o valor máximo absoluto e o menor é o valor mínimo absoluto.
---
**14.8) Multiplicadores de Lagrange** (Questão 2)
* Equações de Lagrange
$$\nabla f(x,y,z) = \lambda \nabla G(x,y,z)$$

**Estratégia**
1. Encontrar ambos os lados da equação $\nabla f(x,y,z) = \lambda \nabla G(x,y,z)$;
2. Igualar num sistema;
3. Encontrar $\lambda$,$y$²,$z²$ e $x$
4. Substituir o valor de $x$ em cada equação de $y$ e $z$;
5. Valor mínimo da distância: $Fmin = x²+y²+z²$ → substitui por $x$

