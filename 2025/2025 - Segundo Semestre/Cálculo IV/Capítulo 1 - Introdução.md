**1.1 Alguns Modelos Matemáticos Básicos; Campos de Direção**

**Definições:**
	**Equação Diferencial:** equações que contém derivadas. A incógnita de uma equação diferencial é uma função
	**Modelo Matemático:** equação diferencial que descreve certo processo físico

<span style="background:rgba(74, 82, 199, 0.2)">(?) A solução real do problema aproximado, serve como solução aproximada do problema real?</span>

* Passos Básicos de Modelagem Matemática:
1. Identificar a variável independente e a variável dependente, atribuindo letras para representá-las;
2. Escolher unidades de medida para cada variável;
3. Usar um princípio básico subjacente ou uma lei que rege o problema investigado;
4. Expressar o princípio/lei do passo 3 em função das variáveis do passo 1;
5. Certificar-se que as parcelas da equação estão nas mesmas unidades;

* Teorema de Existência e Unicidade:
A equação 
$$y'(x)=F(x;y)$$
sempre tem soluções se $F(x;y)$ tiver derivadas parciais contínuas.

Dada a condição inicial $(x_{0};y_{0})$ existe uma única solução $y = y(x)$ de $y'(x) = F(x,y)$ que satisfaz $y(x_{0})=y_{0}$ 

* Variáveis Separáveis 
Se for possível escrever a equação na forma 
$$P(x)dx = Q(y)dy$$
dizemos que $\frac{dy}{dx}(x) = F(x;y)$  é uma equação de variáveis separáveis. 

neste caso, as soluções são obtidas de $$\int P(x)dx = \int Q(x)dy + C$$
onde $C$ é uma constante real arbitrária.

<span style="background:rgba(255, 183, 139, 0.55)">Toda EDO de variáveis separáveis é exata!</span>

- [ ] Fazer exemplos de variáveis separadas no papel.

* Quando vamos resolver uma EDO, primeiro verificamos uma das 3 opções:
1. Ela é linear;
2. É de variáveis separáveis;
3. É exata (geralmente um polinômio, seno ou exponencial).

* Foma da EDO exata: $$M(x,y) + N(x,y)y' = 0$$
Dizemos que ela é exata se existir uma função diferencial $\psi: u \to IR$ tal que:
$\psi_{x}(x,y) = M(x,y)$ para todo $(x,y)$ $\in$ $U$ 
$\psi_{y}(x,y) = N(x,y)$

- [ ] Fazer exemplos de EDO exata no papel.

[(Cálculo IV - Aula 12 - Equações diferenciais ordinárias)](https://youtu.be/mH6GQOtC-KE?si=yItV5juZ6N2R9ZWK)

<span style="background:#d2cbff">Lista Sugerida Seção 1.1: 7-10, 15-20,24</span>

----
<span style="background:#d2cbff">Lista Sugerida seção 1.2: 3,19</span>

---
**1.3 Classificação das Equações Diferenciais**

**Equações Diferenciais Ordinárias:** possuem apenas uma variável independente 
Exemplo: Carga $Q(t)$ em um capacitor em um circuito com capacitância $C$, resistência $R$ e indutância $L$
$$L = d²\frac{Q(t)}{dt²} + R = d\frac{Q(t)}{dt} + \frac{1}{C} Q(t) = E(t)$$
**Equações Diferenciais Parciais:** possuem mais de uma variável independente
Exemplo: Equação de Onda

**Sistema de Equações Diferenciais**:

**Ordem:** a ordem da derivada de maior ordem que aparece na equação.

**Linearidade:** 
* A forma geral da equação diferencial linear:
$$
a_n(x) \frac{d^n y}{dx^n} + a_{n-1}(x) \frac{d^{n-1} y}{dx^{n-1}} + \cdots + a_1(x) \frac{dy}{dx} + a_0(x) y = g(x)
$$

* É linear se:
1. A função desconhecida e todas suas derivadas aparecem na primeira potência;
2. Não há produtos entre $y$ e suas derivadas (ex: $y \cdot \frac{dy}{dx})$
3. Não há funções não-lineares de $y$ ou suas derivadas (ex: $sin(y), e^y, (y')^2, ln(y)$)

onde:
- $a_n(x), a_{n-1}(x), \dots, a_0(x)$ são funções que dependem apenas de $x$;
- $g(x)$ depende apenas de $x$;

Exemplos de Equações Diferenciais Lineares:
$\frac{dy}{dx} + 2y = e^x$
$x^2y'' + xy' + y = 0 \quad$
$y''' - 3y' + 2y = \cos(x)$

Exemplos de Equações Diferenciais Não-Lineares:
$\frac{dy}{dx} + y^2 = 0 \quad \text{(termo } y^2 \text{)}$
$y \cdot y' + y = x \quad \text{(produto } y \cdot y' \text{)}$
$y'' + \sin(y) = 0 \quad \text{(função não-linear de } y \text{)}$

* Linearização: produto do pêndulo.

<span style="background:#d2cbff">Lista Sugerida seção 1.3: 1-6, 15-18,28,31</span>

---
