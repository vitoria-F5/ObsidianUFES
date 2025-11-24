
* **EDO exata: 
	* A forma padrão é $M(x,y)dx + N(x,y)dy = 0$
	* Sempre existe uma função $F(x,y)$ tal que: $dF(x,y) = F_{x}dx + F_{y}dy$;
	* Verificamos que é exata se $\frac{\partial M(x,y)}{\partial y} = \frac{\partial N(x,y)}{\partial x}$;
	* A solução é da forma $F(x,y) = C$ com $C$ sendo uma constante
	* $M(x,y) = F_{x}  \text{ e } N(x,y) =F_{y}$.
---
* **Procedimento de Resolução - EDO's:**
	1. Escrever a EDO na forma padrão: $\text{com }x \text{ como variável independente}\frac{dx}{dy}=F(x,y), \text{ou com } y \text{ como variável independente } \frac{dy}{dx}=F(x,y)$.
	2. Identificar o tipo da EDO (Separável, Linear, Exata ou Homogênea):
		1. É Separável?
			1. Verificar se é da forma padrão separável $\frac{dx}{dy}=f(x)g(y) \text{ ou } \frac{dy}{dx}=f(x)g(y)$.
				1. Se for:
					1. Tornar para o tipo $f(x)dx = g(y)dy$ e integrar em ambos os lados;
					2. Resolver a nova equação para $x \text{ ou } y$.
				2. Se não for: próximo teste.

		2. É Linear?
			1. Verificar se é da forma padrão linear $\frac{dx}{dy} + f(y)x = g(y) \space \text{ ou } \space \frac{dy}{dx} + f(x)y = g(x)$.
				1. Se for:
						1. Calcular o Fator Integrante $\mu(y) = e^{\int f(y)dy} \text{ ou } \mu(x) = e^{\int f(x)dx}$;
						2. Calcular a derivada do Fator Integrante;
						3. Multiplicar o Fator Integrante pela forma padrão linear obtida em (1);
						4. Reescrever o produto de maneira implícita como a derivada do produto como na forma $(x\mu(y))' = x'\mu(y)+x\mu'(y)$;
						5. Resolver para $(x\mu(y))'$ usando igualdades e rearranjos;
						6. Integrar ambos os lados;
						7. Resolver para $x \text{ ou } y$.
				2. Se não for: próximo teste.

		3. É exata?
			1. Escrever na forma padrão $M(x,y)dx + N(x,y)dy = 0$;
				1. Verificar se $\frac{\partial M}{\partial y} = \frac{\partial N}{\partial x}$.
					1. Se for:
						1. Para $M(x,y)dx$:
							1. Integrar em relação a $x$, obtendo $\psi(x,y)$;
							2. Derivar $\psi(x,y)$ em relação a $y$ surgindo um $h'(y)$;
							3. Igualar a $N(x,y)$ e resolver pra $h'(y)$;
							4. Integrar $h'(y)$;
							5. Substituir $h(y)$ em $\psi(x,y)$;
			2. Se não for: 
				1. Testar para encontrar um fator integrante:
					1. Se $\frac{(My - Nx)}{N} = f(x):$  então, usa-se que $μ(x) = e^{\int{f(x)dx}}$;
					2. Se $\frac{(Nx - My)}{M} = g(y):$ então, usa-se que $\mu(y) = e^ {f(y)dy}$;
				2. Multiplicar o Fator Integrante pela EDO padrão;
				3. Integrar em relação a $x$ que é $\psi(x,y)$;
				4. Derivar $\psi(x,y)$ em relação a $y$;
				5. Igualar a $N(x,y)$ e resolver pra $h'(y)$;
				6. Integrar $h'(y)$;
				7. Substituir $h(y)$ em $\psi(x,y)$;

		5. É homogênea?
			1. Escrever a forma padrão da EDO em função de $(\frac{y}{x})$;
			2. Usar que $v = (\frac{y}{x})$ para achar $y = vx$ e $\frac{dy}{dx} =v +xv'$;
			3. Substituir $y = vx$ e $\frac{dy}{dx}$em (1️);
			4. Verificar se é separável:
				1. Se for:
					1. Tornar para o tipo $f(x)dx = g(y)dy$ e integrar em ambos os lados;
					2. Resolver a nova equação para $x \text{ ou } y$.
				2. Se não for: revise.