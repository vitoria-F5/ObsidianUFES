Atividade 1
1. Importei duas bibliotecas: a math pras funções trigonométricas e raiz quadrada, e a outra pro gráfico

2. Criei listas pra armazenar os valores de tempo e as posições

3. Depois um loop que executa 300 vezes, no caso são 3 segundos que vão aumentando de 0,01 segundos e são armazenados na lista
	1. Para cada instante de tempo, eu calculei as posições usando essa fórmula do MHS e armazenando nas listas

4. Configurei os três sistemas diferentes: primeiro, massa de 2kg com mola de 200N/m; segundo, massa de 3kg com mesma mola de 200N/m; e terceiro, massa de 5kg com mola de 500N/m com um angulo phi de π/2 radianos diferente dos outros pra evitar sobreposição;

5. Por fim, criei uma figura com as três curvas representando cada sistema da questão com título, uma grade padrão e uma legenda.

------

Atividade 2
1. **Importei uma biblioteca** pra criar gráficos e visualizar os resultados.  

2. Pedi quatro valores de aceleração (em m/s²) para simular diferentes cenários de movimento acelerado.  

3. Defini um intervalo de tempo de 0 a 10 segundos, com incrementos de 1 segundo (`tempos = [0, 1, 2, ..., 10]`).  

4. Criei quatro listas (`v1`, `v2`, `v3`, `v4`) para calcular e guardar a velocidade de cada aceleração ao longo do tempo.  

5. Para cada tempo `t` na lista `tempos`, calculei a velocidade usando a fórmula do movimento uniformemente acelerado: armazenei os resultados nas listas de velocidades correspondentes.  

6. 
   - Defini o tamanho da figura (`figsize=(10, 6)`) para melhor visualização.  
   - Plotei quatro curvas, uma para cada aceleração, com cores diferentes e legendas personalizadas (mostrando o valor da aceleração). 

1. Por fim, criei uma figura com as três curvas representando cada sistema da questão com título, uma grade padrão e uma legenda.
   - Título: "Velocidade do Carro ao Longo do Tempo".  
   - Rótulos dos eixos:  
     - Eixo X: "Tempo (s)".  
     - Eixo Y: "Velocidade (m/s)".  
   - Grade (`grid(True)`) para facilitar a leitura.  
   - Legenda (`legend()`) para identificar cada curva.  

8. **Exibi o gráfico**:  
   - Usei `plt.show()` para visualizar o resultado final.  
