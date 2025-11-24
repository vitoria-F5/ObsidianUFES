**2.1 Equações Lineares; Método dos Fatores Integrantes**
* Definições:
	**Solução da Equação Diferencial Ordinária de ordem 1:**
	1. Colocar na Forma Padrão da Equação Linear de Primeira Ordem: $$y'(t)+p(t)y = q(t)$$onde $p(t)$ e $g(t)$ são funções dadas da variável dependente t.
	
	2. Calculamos o *fator integrante* $\mu(t) = e^{\int p(t)  dt}$ 
	3. Solução será dada por: 
$$y(t) = \frac{1}{\mu(t)\left( \int \mu(t)·g(t)dt + c \right)}$$

- [ ] Exemplo 1 do 9

**2.2 Equações Separáveis**
* **Variáveis Separáveis** 
	Se for possível escrever a equação na forma:
	$$\frac{dy}{dx}=f(x)g(y)$$

	neste caso, as soluções são obtidas de $$\int P(x)dx = \int Q(x)dy + C$$
	onde $C$ é uma constante real arbitrária.

	<span style="background:rgba(255, 183, 139, 0.55)">Observação: Toda EDO de variáveis separáveis é exata!</span>
* **EDO do tipo Linear**
	Se for possível escrever a equação na forma:
 $$\frac{dy}{dx} +P(x)y=Q(x) \space \text{ ou do tipo } \space \frac{dx}{dy} + P(y)x = Q(y)$$

* **Foma da EDO exata: $$M(x,y) + N(x,y)y' = 0$$**
	Dizemos que ela é exata se existir uma função diferencial $\psi: u \to IR$ tal que:
	$\psi_{x}(x,y) = M(x,y)$ para todo $(x,y)$ $\in$ $U$ 
	$\psi_{y}(x,y) = N(x,y)$

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
3. Não há funções não-lineares da variável dependente ou suas derivadas (ex: $sin(y), e^y, (y')^2, ln(y)$)

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

---
* **Procedimento de Resolução - EDOS:**
	1. Escrever a EDO na forma padrão: $\text{com }x \text{ como variável independente}\frac{dx}{dy}=F(x,y), \text{ou com } y \text{ como variável independente } \frac{dy}{dx}=F(x,y)$.
	2. Identificar o tipo da EDO;
		1. É separável?
			1. Verificar se é da forma $\frac{dy}{dx}=f(x)g(y) \text{ ou } \frac{dx}{dy}=f(x)g(y)$;
				1. Se for:
					1. Torna para o tipo $dy(y) = dx(x)$ e integra em ambos os lados;
					2. Resolve para $x \text{ ou } y$.
				2. Se não for: próximo passo.
		2. É linear?
			1. Verificar se é da forma padrão linear $\frac{dy}{dx} +P(x)y=Q(x) \space \text{ ou do tipo } \space \frac{dx}{dy} + P(y)x = Q(y)$
				1. Se for:
					1. Calcular o Fator Integrante $\mu(y) = e^{\int P(y)dx} \text{ ou } \mu(x) = e^{\int P(x)dy}$;
					2. Calcular a derivada do Fator Integrante;
					3. Multiplicar o fator integrante pela EDO da forma linear (1);
					4. Reescrever a nova EDO de maneira implícita para a derivada do produto;
					5. Igualar a derivada do produto à correspondencia da EDO em (4);
					6. Integrar ambos os lados;
					7. Resolver para $x \text{ ou } y$.
				2. Se não for: próximo passo.
		3. É exata?
			1. Escrever na forma padrão $M(x,y)dx + N(x,y)dy = 0$;
			2. Verificar se $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$.
				1. Se for:
					1. Para $M(x,y)$:
						1. Integrar em relação a $x$;
						2. Derivar em relação a $y$;
					2. Igualar a $N(x,y)$ e achar $h'(y)$:
					3.  Resolver pra $x$ ou $y$.
				2. Se não for: 
					1. Tentar calcular o Fator Integrante $μ(x) \text{ se } (My - Nx)/N = f(x) \text{ ou } μ(y) \text{ se } (Nx - My)/M = g(y)$
					2. Multiplicar o fator integrante pela EDO padrão;
					3. 
		4. É homogênea?
			1. Escrever a forma padrão da EDO em função de $(\frac{y}{x})$;
			2. Usar que $v = (\frac{y}{x})$ para achar $y = vx$ e o valor de $\frac{dy}{dx}$;
			3. Substituir $y = vx$ e $\frac{dy}{dx}$em 1️⃣;
			4. Verificar se é separável:
				1. Se for: Resolver integrando dos dois lados;
				2. Resolver para $x \text{ ou } y$;
				3. Se não for: Próximo passo.

