**3.3 Determinante**
* **Definições**
	* **Permutação:** dados $n$ objetos distintos $a_{1},\dots,a_{n},$ uma permutação destes objetos consiste em dispô-los em uma determinada ordem. <font color="#de7802">Exemplo: (1 2 3) e (3 2 1) é uma permutação dos números 1, 2 e 3</font>.
		* **Inversão de Permutação:** quando dada uma permutação dos inteiros 1, 2, …., n, um inteiro maior vai na frente do menor.
	* **Determinante |A|:** número de inversões da permutação.
		- **Propriedades:**
			1. Permutação com Número Par de Inversões: somatória positiva;
			2. Permutação com Número Ímpar de Inversões: somatória negativa;
			3. Se Todos os Elementos de uma Linha (coluna) de uma Matriz $A$ são Nulos: $det A = 0$
			4. $\det A = \det A'$
			5. Matriz Multiplicada por Constante: $\det$ multiplicado por constante.
			6. Duas Linhas Trocadas: troca sinal de $\det$;
			7. Determinante de Matriz com 2 Linhas (colunas) Iguais: zero
			8. $\det(A·B) = \det A · \det B$ 
			9. Matriz Triangular: O produto de sua diagonal equivale ao $determinante$

* **Cálculo do Determinante (Regra de Sarrus):**
![[Pasted image 20251028103531.png]]
**3.4 Desenvolvimento de Laplace**
* **Desenvolvimento de Laplace:** permite calcular o determinante de uma matriz de ordem $n$, a partir dos determinantes das submatrizes quadradas de ordem $n - 1$.
1. Escolher uma linha ou coluna (fila) padrão, de preferência que tenha um ou mais zeros;
2. Descrever a fórmula: $a_{ij}C_{ij} + a_{ij}C_{ij} + a_{ij}C_{ij} \dots = \dots$ 
3. Calcular cofatores: $C_{ij}= (-1)^{i+j}\det M_{ij}$
4. Substituir na Fórmula
 
**3.6 Regra de Cramer**
5. Verificar se o determinante é diferente de zero;
6. Encontrar $x,y,z..$:
	1. Substituir na matriz dos coeficiente o resultado exatamente na coluna do coeficiente desejado;
	2. Calcular o determinante da nova matriz;
	3. Dividir o determinante da nova matriz pelo determinante geral;

**3.9 Procedimento para a Inversão de Matrizes**
1. Verificar se o $determinante$ é diferente de zero;
2. Colocar matriz lado a lado da identidade e transformar a inicial em identidade (a da direita será a inversa)