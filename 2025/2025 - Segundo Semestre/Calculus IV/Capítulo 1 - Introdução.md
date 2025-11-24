**Equações Diferenciais Ordinárias Homogêneas**
* **Definições:**
	* **Função Homogênea:**  é da forma $f(\lambda x, \lambda y) = \lambda^n  ·f(x,y)$ para algum valor real de $n$.
		* Exemplo: $f(x,y) = x² +2xy - y²$.
			1. Transformar $x$ em $\lambda x$ e $y$ em $\lambda y$;
			2. Verificar se o resultado é equivalente a forma geral.
	* **Equações Diferenciais Ordinárias Homogêneas:** dada a EDO $M(x,y)·dx + N(x,y)·dy = 0$, ela é homogênea se $M(x,y)$ e $N(x,y)$ forem funções homogêneas de mesmo grau. 
		* **Método de Resolução:**
			1. (TRANSFORMAR EM EDO SEPARÁVEL) 
				1. Verificar entre $M(x,y)$ e $N(x,y)$ qual função é mais simples;
					1. Se $dx$ = $x = v·y$
					2. Se $dy$ = $y = u·x$
					3. Se não houver diferença significativa → Qualquer uma 
1. 

-----
**Equações Ordinárias de Segunda Ordem**
**Forma Geral:**
$$\frac{d²y}{dt²}=f(t,y,\frac{dy}{dt})$$
**Problema de Valor Inicial:** É o conjunto da equação diferencial com uma condição inicial.
* **Definições:**
	* Ao resolver a equação diferencial, se obtem a **solução geral;**
	* Ao aplicar a condição inicial, se obtem a **solução particular;**

* **Método para Encontrar a Solução Explícita:**
	1. Escrever a EDO na forma padrão;
1. 
**1.3 Classificação das Equações Diferenciais**

**Equações Diferenciais Ordinárias:** possuem apenas uma variável independente 
Exemplo: Carga $Q(t)$ em um capacitor em um circuito com capacitância $C$, resistência $R$ e indutância $L$
$$L = d²\frac{Q(t)}{dt²} + R = d\frac{Q(t)}{dt} + \frac{1}{C} Q(t) = E(t)$$
**Equações Diferenciais Parciais:** possuem mais de uma variável independente
Exemplo: Equação de Onda

**Sistema de Equações Diferenciais**:

**Ordem da EDO:** a ordem da derivada de maior ordem que aparece na equação.

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
