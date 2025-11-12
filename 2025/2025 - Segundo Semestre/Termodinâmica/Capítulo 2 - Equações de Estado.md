* **Seção 2.2 Equação de Estado de um Gás Ideal**
	**Tópico:** Constante Universal dos Gases
	**O que diz:** É o **limite comum** da razão $\frac{Pv}{T}$ quando $P \to 0$, onde $v$ é o **volume molar**.
	**Por que:**  No limite de **pressão zero**, todos os gases reais comportam-se como gases ideais, e a razão $\frac{Pv}{T}$ torna-se **a mesma para qualquer gás**, definindo assim a constante universal $R$.
	**Fórmula:** $R = \lim_{P \to 0} \frac{Pv}{T} \simeq 8314 \ \text{J·mol}^{-1}\text{·K}^{-1}$
	
	* **Equação de Estado de um Gás Ideal:** $Pv = nRT$ ou $PV = nRT$

* **Seção 2.3 Superfície P-v-T para um Gás Ideal**
	**Tópico:** Processo Isotérmico (Lei de Boyle)
	**O que diz:**  Em um processo isotérmico com massa fixa de um gás ideal, o produto da pressão pelo volume é constante.
	**Por que:**  
	**Fórmula:**  $Pv = RT$
	**Mini exemplo:**  

	**Tópico:** Processo Isocórico
	**O que diz:**  Em um processo isocórico com massa fixa de um gás ideal, a pressão é uma função linear da temperatura
	**Por que:**
	**Fórmula:**  $P=(\frac{nR}{V})T = \text{constante} \times T$
	**Mini exemplo:**  
	
	**Tópico:** Processo Isobárico
	**O que diz:**  Em um processo isobárico com massa fixa de um gás ideal, o volume é uma função linear da temperatura.
	**Fórmula:**  $V = (\frac{nR}{P})T = \text{constante} \times T$
	**Mini exemplo:**  
	
	* **Processo Adiabático:** sem troca de calor

* **Seção 2.4 Equações de Estado de Gases Reais**

$$\text{Van der Walls em 1873:}$$
$$(P + \frac{a}{v²})(v-b) = RT$$


$$\text{Forma Expandida em Série de Potências de v:}$$
$$Pv³-(Pb + RT)v² + av - ab = 0$$


$$\text{Outra forma:}$$
$$Pv = A + \frac{B}{v} + \frac{C}{v²}+\dots,$$
$$\text{Forma Virial:}$$$$Pv = RT(1 - \frac{b}{v})⁻^1 -\frac{a}{v}$$$$\text{(pelo teorema binomial, segue que:)}$$
$$(1 - \frac{b}{v})⁻^1 = 1 + \frac{b}{v} + \frac{b²}{v} + \dots$$

* **2.7 Derivadas Parciais, Expansibilidade e Compressibilidade**
	* **Inclinação da Tangente de PT:** $(\frac{\partial P}{\partial T})$
	* **Coeficiênte de Dilatação Volumétrica:** $\beta = \frac{1}{V}(\frac{\partial V}{\partial T})_{P}$ 
	* **Coeficiênte de Compressão Isotérmica:** $k = - \frac{1}{V}(\frac{\partial V}{\partial P})_{T}$

* **2.8 Constantes Críticas de um Gás de Van der Waals**
	* Como calcular as constantes críticas $P_{c}, v_{c} \space \text{e} \space T_{c}$ dado uma equação de Van de Walls:
		1. Resolver a equação de Van der Walls para P;
		2. Derivar P em relação a $v$ com $T$ constante;
		3. Considerar que no ponto crítico $(\frac{\partial P}{\partial v})_{T}=0$ e chegar em uma relação pras constantes críticas
		4. Derivar P em relação a $v$ com $T$ constante;
		5. Considerar que no ponto crítico $(\frac{\partial² P}{\partial v²})_{T}=0$ e chegar em uma nova relação pras constantes críticas
		6. Resolver o sistema das duas relações encontras e achar $P_{c}, v_{c} \space \text{e} \space T_{c}$    bgv 


* **Seção 2.10 Diferenciais Exatas**
	* **Diferencial Exata do Volume:** $dV = (\frac{\partial V}{\partial T})_{P}\space dT + (\frac{\partial V}{\partial P})_{T} \space dP$

-----

**Outras equações não especificamente citadas no livro:**
* **Lei de Boyle-Mariotte:** $P_{0}V_{0}=P_{f}V_{f}$
* **Volume em Seção Reta Uniforme:** $V = AH$ 
* **Ley de Gay-Lussac*:** $\frac{P_{1}}{T_{1}} = \frac{P_{2}}{T_{2}}$  
