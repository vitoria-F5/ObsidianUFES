**2.4 Forma Escada**
* Condição
	1. O 1° elemento não nulo de uma linha não nula é 1;
	2. Cada coluna que contém o 1° elemento não nulo de alguma linha tem todos os seus outros elementos iguais a zero;
	3. Toda linha nula ocorre abaixo de todas as linhas não nulas;
	4. Se as linhas 1, …,r são as linhas não nulas, e se o primeiro elemento não nulo de linha i ocorre na coluna na $k_{1} < k_{2} < \dots < k_{r}$.

**2.4.4 Posto e Nulidade**
* **Definição de Posto:** Linhas não nulas da matriz, podendo ser:
	* $\rho_{c}:$ posto da matriz dos coeficientes;
	* $\rho_{a}:$ posto da matriz ampliada.
* **Definição de Nulidade/grau de liberdade:** É o número do número de equações menos o posto (denominado por apenas $\rho$ se $\rho_{c}$ e $\rho_{a}$ são iguais) $n - \rho$.

**2.5 Soluções de um Sistema de Equações Lineares**
**2.5.1 Sistema de uma equação e uma incógnita**
$$ax = b$$
existirão três possibilidades:
i) $a ≠ 0$ e $b\neq 0$ → solução única: $x = \frac{b}{a}$;
ii) $a = 0$ e $b = 0$ → soluções infinitas: $0x = 0$ e qualquer número real será solução;
iii) $a = 0$ e $b \neq 0$ → soluções impossíveis: $0x = b$ 

**2.5.3 Caso Geral**

**2.5.4 Teorema**
* **Discussão de Soluções:**
	* $\rho_{c}$ $\neq$ $\rho_{a}$ → Solução Impossível;
	* $\rho_{c}=\rho_{a}:$
		* $\rho_{c} = \rho_{a} = n$ → Solução Única;
		* $\rho_{c} = \rho_{a}$ $\neq$ $n$ → Soluções Infinitas;