**16.1) Campos Vetoriais**

* O que é um campo vetorial? Dê três exemplos com significado físico.
	* **Campo Vetorial:** Seja D um conjunto em R² (região plana). Campo vetorial em $R²$ é uma função $F$ que associa a cada ponto $(x,y)$ em D um vetor bidimensional $f(x,y)$.
	* Ex.:  Campo Vetorial de Velocidade que mostra aspectos do vento em determinada região, correntes oceânicas e escoamento do ar.
* O que é um campo vetorial conservativo?
	* **Campo Vetorial Conservativo:** Um campo o qual é gradiente de alguma função escalar → Se existir uma função $f$ tal que $F = \nabla{f}$. Ex.: Campo Gravitacional.
* O que é uma função potencial?
	* **Função Potencial:** A função $f$ para o caso anterior.

**16.2) Integrais de Linha**
(Inventadas para resolver problemas relacionados a escoamento de fluídos e magnetismo)

**Definições**
* Integral de Linha de $f$ sobre $C$ 
$$\int_{C} f(x,y)ds = \int_{a}^{b}f(x(t),y(t))\sqrt{(\frac{dx}{dt})²+(\frac{dy}{dt})²}\space dt
$$
$$\int_{C} f(x,y,z)ds = \int_{a}^{b}f(x(t),y(t),z(t))\sqrt{(\frac{dx}{dt})²+(\frac{dy}{dt})²+ (\frac{dz}{dt})²}\space dt
$$
**TIPO**
* $\int_{C} xds$ é o arco de parábola $y = x²$ de $(0,0)$ a $(1.1)$
* $\int_{C}yz\cos xds$, $C: x = t, y =3\cos t,z=3sent$ e $0 \leq t\leq\pi$

**Estratégia**
1. Identificar em relação a quem o arco C está em função:
2. Parametrizar em relação a quem o arco C está em função;
3. Derivar quem não está em função;
4. Substituir.

* Parametrização do Seguimento de Reta
$$r(t)=(1-t)r_{0}+tr_{1}$$
$$0\leq t\leq 1$$
**TIPO**
Provavelmente fala que é um segmento de reta

**Estratégia**
1. $r(t)=(1-t)<1,0,-1> + \space t<3,4,2>\space =\space <1-t,0-1,-1+t>+<3t,4t,2t>=<1+2t,4t,-1+3t>$
2. separa cada termo em x,y,z
3. Deriva cada termo
4. Substitui

* Integral de Linha com Relação ao Comprimento de Arco em Função de $x$ e $y$ 
$$\int_C f(x,y) \, ds = \int_{a}^{b} f(x(t), y(t))x'(t)dt$$
$$\int_C f (x, y) \, ds = \int_{a}^{b} f (x (t), y (t)) y'(t)dt$$
**TIPO**
* $\int_{C}y³dx+x²dy$ onde $C$ é o arco da parábola $x = 1 - y²$ de $(0,-1)$ a $(0,1)$.

**Estratégia**
1. Identificar em relação a quem o arco C está em função:
	1. x = y + 1 (em função de y, usa-se o tipo 2)
	2. y = x + 1 (em função de x, usa-se o tipo 1)
2. Parametrizar em relação a quem o arco C está em função;
3. Derivar quem não está em função;
4. Substituir.

* Centro de Massa
$$\overline{x} = \frac{1}{m}\int_C x\rho(x,y)ds \space \space e \space \space\overline{y} = \frac{1}{m}\int_C y\rho (x, y) ds$$

* Integral de Linha sobre $C$ de uma função escalar $f$ (em relação a $x,y$ e $z$)

* Integral de linha do campo vetorial $F$ ao longo da curva suave $C$ dada pela função vetorial $r(t)$
$$
\int_C \vec F · d\vec r = \int_a^b \vec F (\vec r(t)) · \vec r'(t)dt = \int_C \vec F · T ds
$$
$$W = \int_{C} F·dr = \int_{a}^{b}F(r(t))·r'(t)dt = \int_{C}F·Tds$$
**TIPO**
* $\int_{C}F·dr$, onde $F(x,y,z) = e²i + xyj +(x+y)k$ e $C$ é dado por $r(t) = t²i + t³j - tk$, $0\leq t\leq 1$ 

**Estratégia**
1. Parametrizar a curva C (F(x,y,z)) em função de t;
2. Derivada da parametrização;
3. Substituir r(t) em F(x,y,z) resultando em F(r(t));
4. Calcular o produto;
5. Definir os limites;
6. Calcular a integral

----
**16.3) O Teorema Fundamental das Integrais de Linha**

> <u>Relembre...</u>
> Teorema Fundamental do *Cálculo*
>$$\int_a^bF'(x)dx = F(b) = F(a)$$

* Teorema Fundamental das Integrais de Linha
	Sendo $C$ uma curva suave dada pela função vetorial $\mathbf r(t)$, $a \leq t \leq b$. Seja $f$ uma função diferenciável de duas ou três variáveis cujo vetor gradiente $\nabla f$ é contínuo em $C$. Então:
$$\int_C \nabla f·d \mathbf r = f(\mathbf r(b) - f(\mathbf r(a))$$
* O que significa dizer que $\int_C \mathbf F · d \mathbf r$ é independente do caminho?
	* que a integral de linha de um campo vetorial conservativo depende somente das extremidades da curva.
* Se você souber que $\int_C \mathbf F · d \mathbf r$ é independente do caminho, o que poderia dizer sobre $\mathbf F$?
	* que as integrais de linha de campos vetoriais são conservativos

* Teorema
	Se $F(x,y)= P(x,y)i + Q(x,y)j$ é um campo vetorial conservativo, onde $P$ e $Q$ têm derivadas parciais de primeira ordem contínuas em um domínio $D$, então em todos os pontos de $D$ temos:
$$\frac{\partial P}{\partial y} = \frac{\partial Q}{\partial x}$$
**Estratégias**
Mostrar que $F$ é conservativo
1. Explicitar: componentes $P(x,y)$ e $Q(x,y)$;
2. Derivar: $P$ em função de $y$ e $Q$ em função de $x$;
3. Comparar: os resultados
	1. Se forem iguais - $F$ é conservativo;
	2. Se forem diferentes - $F$ não é conservativo

Determinar uma função $f$ tal que $F = \nabla f$ sendo $F(x,y) = f_{x}(x,y) = (1 + xy)e⁵i + f_{y}(x,y) = (5 + xy)e⁶j$
1. Sabendo que $f$ é conservativo, existe:
	1. $f_{x}(x,y) = (1 + xy)e⁵$
	2. $f_{y}(x,y) = (5 + xy)e⁶$
2. Integrar $f_{x}$ em relação a $x$ obtendo $f(x,y)$;
3. Derivar $f(x,y)$ em relação a $y$;
4. Comparar $f_{y}(x,y)$ e $f'_{y}(x,y)$ para achar $g'(x)$
5. Integrar para achar $g(x)$

Calcular $\int_{C}F·dr$ ao longo da curva dada a partir da conservação de $F$
1. Conhecer: pontos final e inicial de $C$;
2. Encontrar: uma função $f$ tal que $F = \nabla f$;
3. Substituir os pontos final e inicial de $C$ em $\int_{C} F · dr = \int_{C} \nabla f·dr = f(r(b)-r(a))$.

**16.4) Teorema de Green**
é relação do delimitador, a integral de linha, com a região interna

correspondente ao Teorema Fundamental do Cálculo para integrais duplas e fornece uma relação entre uma integral de linha ao redor de uma curva fechada simples $C$ e uma integral dupla sobre a região do plano $D$ delimitada por $C$.

convenção: a orientação positiva de uma curva fechada simples $C$ refere-se ao <font color="#ff0000">sentido anti-horário</font> de $C$, percorrido uma só vez.

* Teorema de Green: Seja $C$ uma curva plana simples, fechada, contínua por partes, orientada positivamente, e seja $D$ a região delimitada por $C$. Se $P$ e $Q$ têm derivadas parciais de primeira ordem contínuas sobre uma região aberta que contenha $D$, então:
$$\int\int_{C}P\space dx + Q \space dy = \int \int_{D} (\frac {\partial Q}{\partial x} - \frac{\partial P}{\partial y})\space dA$$
**Estratégias**
1. Identificar $P(x,y)$ e $Q(x,y)$
2. Derivadas Parciais
3. Substituir

**16.5) Rotacional e Divergente**

* **Rotacional de F:** se $F = Pi + Qj + Kr$ é um campo vetorial em $R³$ e as derivadas parciais de $P, Q$ e $R$ existem, então o rotacional de $F$ é o campo vetorial em $R³$ definido por:

$$rot \space F =
\vec{\nabla} \times \vec{F} = 
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\
P & Q & R \\
\end{vmatrix}
= \left( \frac{\partial R}{\partial y} - \frac{\partial Q}{\partial z} \right)\hat{i} - \left( \frac{\partial R}{\partial x} - \frac{\partial P}{\partial z} \right)\hat{j} + \left( \frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} \right)\hat{k}
$$

$$rot \space F = (\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z})i + (\frac{\partial P}{\partial z}-\frac{\partial R}{\partial x})j + (\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y})k$$
* Se $$F = Pi + Qj + rK$$ é uma função de 3 variáveis que tem derivadas parciais de segunda ordem contínuas, então: $$rot (\nabla f) = 0$$
	* Se isso ocorre, *F* é um campo vetorial conservativo.

* **Divergente de F:** Se $F = Pi + Qj + Kr$$ é um campo vetorial é um campo vetorial em $R³$ e $\frac {\partial P}{\partial x}$, $\frac {\partial Q}{\partial y}$, $\frac {\partial R}{\partial z}$ existem, então o divergente de $F$ é a função de 3 variáveis definida por:
$$div F = \frac {\partial P}{\partial x} + \frac {\partial Q}{\partial y} + \frac {\partial R}{\partial z}$$

**16.6) Superfícies Parametrizadas e suas Áreas**
usar funções vetoriais para descrever superfícies parametrizadas e calcular as áreas.

* **Superfícies Parametrizadas**
Suponhamos que $r(u,v) = x(u,v)i + y(u,v)j + z(u,v)k$ seja uma função de valores vetoriais definida sobre uma região $D$ do plano $uv$. Então $x, y$ e $z$ , os componentes de funções de r, são funções de duas variáveis $u$ e $v$ com domínio $D$. 

O conjunto de todos os pontos $(x,y,z)$ em $R³$ tal que:
$$x = x(u,v) \space y = y(u,v) \space z = z(u,v) \ space $$
são as superfícies parametrizadas

* Superfícies de Revolução
* Planos Tangentes
* Área de Superfície
$$r(u,v) = x(u,v)\mathbf{i} + y(u,v)\mathbf{j} + z(u,v)\mathbf{k}$$
$$(u,v) \in D$$
<div align="center">(Superfície Parametrizada suave S)</div>

$$A(S) = \int\int_D|\mathbf{r_u}\times \mathbf{r_v}|dA$$
Onde, 

$$\mathbf{r_u}=\frac{\partial{x}}{\partial{u}}\mathbf{i}+\frac{\partial{y}}{\partial{u}}\mathbf{j}+\frac{\partial{z}}{\partial{u}}\mathbf{k} ,\mathbf{r_v}=\frac{\partial{x}}{\partial{v}}\mathbf{i}+\frac{\partial{y}}{\partial{v}}\mathbf{j}+\frac{\partial{z}}{\partial{v}}\mathbf{k}$$

* Área de Superfície do Gráfico de uma Função
$$A(S) = \int _{D}\int \sqrt{1 +(\frac{\partial z}{\partial x})²+(\frac{\partial z}{\partial y})²}\space dA$$

**16.7) Integrais de Superfície**
-

**16.8) Teorema de Stokes**
generalização do Teorema de Green

Enquanto o Teorema de Green relaciona uma integral dupla sobre uma região plana $D$ com uma integral de linha em torno de sua curva limite plana, o Teorema de Stokes relaciona uma integral de superfície $S$ com uma integral em torno da curva da fronteira $S$ (que é uma curva no espaço).

* Teorema de Stokes
	* Seja $S$ uma superfície orientada, suave por partes, cuja fronteira é formada por uma curva $C$ fechada, simples, suave por partes, com orientação positiva;
	* Seja $F$ um campo vetorial cujas componentes têm derivadas parciais contínuas em uma região aberta de $R³$ que contém $S$:
$$\int_{C}F·dr =\int_{a}^{b}F(r(t))·r'(t)= \int _{S}\int rot\space F·dS$$

O Teorema de Stokes diz que a integral de linha em torno da curva fronteira de $S$ da componente tangencial de $F$ é igual à integral de superfície sobre $S$ da componente normal do rotacional de $F$.

**Estratégias**
Cálculo do Rotacional 
1. Identificar $P, Q$ e $R$;
2. Calcular o produtor vetorial $\nabla \times F$;
3. Calcular as derivadas parciais do produto vetorial
4. Substituir.

**16.9) Teorema do Divergente**
Seja $E$ uma região sólida simples e seja $S$ a superfície fronteira de $E$, orientada positivamente (para fora). Seja $F$ um campo vetorial cujas funções componentes tenham derivadas parciais contínuas em uma região aberta que contenha $E$. Então
$$\int \int _{S} F·ds = \int \int \int _{E} div \space F \space dV$$
Questão B
1. Aplicar o teorema do divergente
2. A região $V$ é o cilindro elíptico entre $z = 0$ e $z=5$ com base $B = (x,y):x²+ \frac{y²}{4}\leq_ {1}$ 
3. Transformação Linear em B (u,v);
4. Determinante Jacobiano;
5. Substituir na integração original
6. Passar para coordenadas polares  

Questão 3:
1. Normal unitária da esfera $||r|| = R$, a normal externa é $n = \frac{(x,y,z)}{R²}$
2. O valor de F na esfera: $F = \frac{(x,y,z)}{R²}$
3. Produto escalar constante: $F · n$
4. Integrar $\int \int FndS$ → dS = $4\pi R²$