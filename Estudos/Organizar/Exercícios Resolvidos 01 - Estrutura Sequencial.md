# Exercícios Resolvidos: 01 - Estrutura Sequencial
#Licenciatura/Algoritmos/FundamentosDaProgramaçãoDeComputadores

1. Faça um programa que
	* Receba quatro números inteiros,
	* Calcule a soma destes números,
	* Mostre a soma.

```portugol
	LEIA numero1
	LEIA numero2
	LEIA numero3
	LEIA numero4

	soma_dos_numeros = numero1 + numero2 + numero3 + numero4

	ESCREVA soma_dos_numeros
```

2. Faça um programa que:
	* Receba três notas,
	* Calcule a média aritmética das notas,
	* Mostre a média aritmética.
   
```portugol
   LEIA noa1
   LEIA nota2
   LEIA nota3

   NUMERO_DE_NOTAS_LIDAS = 3

   media_aritmetica = (nota1 + nota2 + nota3) / NUMERO_DE_NOTAS_LIDAS

   ESCREVA media_aritmetica
```

3. Faça um programa que:
	* Receba três notas e seus respectivos pesos,
	* Calcule a média ponderada,
	* Mostre a média ponderada.

```portugol
LEIA nota1
LEIA nota2
LEIA nota3

LEIA peso1
LEIA peso2
LEIA peso3

soma_das_notas_vezes_os_pesos = nota1 * peso1 + nota2 * peso2 + nota3 * peso3
soma_dos_pesos = peso1 + peso2 + peso3
media_poderada = soma_das_notas_vezes_os_pesos / soma_dos_pesos

ESCREVA media_ponderada
```

4. Faça um programa que:
	* Receba o salário de um funcionário,
	* Calcule o valor do aumento de 25% do salário,
	* Calcule o novo salário com o aumento,
	* Mostre o valores do aumento,
	* Mostre o novo salário.

```portugol
PORCENTAGEM_DE_AUMENTO = 25 / 100

LEIA salario

valor_do_aumento = salario * PORCENTAGEM_DE_AUMENTO
valor_do_novo_salario = salario + valor_do_aumento

ESCREVA valor_do_aumento
ESCREVA valor_do_novo_salario
```

5. Faça um programa que:
	* Receba o salário de um funcionário,
	* Receba o percentual de aumento do salário,
	* Calcule o valor do aumento,
	* Mostre o valor do aumento,
	* Mostre o valor do novo salário.

```portugol
LEIA salario
LEIA percentual_de_aumento

valor_do_aumento = salario * percentual_de_aumento
valor_do_novo_salario = salario + aumento_valor_do_aumento

ESCREVA valor_do_aumento
ESCREVA valor_do_novo_salario
```

6.  Faça um programa que:
	* Receba o salário base de um funcionário,
	* Calcule o valor da gratificação de 5% sobre o salário base,
	* Calcule o valor do imposto de 7% sobre o salário base,
	* Mostre o salário a receber.

```portugol
PORCENTAGEM_DA_GRATIFICACAO = 5 / 100
PORCENTAGEM_DO_IMPOSTO = 7 / 100

LEIA salario_base

valor_da_gratificacao = salario_base * PORCENTAGEM_DA_GRATIFICACAO
valor_do_imposto = salario_base * PORCENTAGEM_DO_IMPOSTO
salario_a_receber = salario_base + valor_da_gratificacao − valor_do_imposto

ESCREVA salrario_a_receber
```

7. Faça um programa que:
	* Receba o salário base de um funcionário,
	* Calcule o valor do imposto de 10% sobre o salário base,
	* Adicione a gratificação de 50,00 ao salário base
	* Mostre o valor do salario base

```portugol
VALOR_DA_GRATIFICACAO = 50
PORCENTAGEM_DO_IMPOSTO = 10 / 100

LEIA salario_base

valor_do_imposto = salario_base * PORCENTAGEM_DO_IMPOSTO
salario_a_receber = salario_base + VALOR_DA_GRATIFICACAO - valor_do_imposto

ESCREVA salario_a_receber
```

8. Faça um programa que:
	* Receba o valor de um depósito,
	* Receba a taxa de juros em porcentagem, que será aplicada ao depósito,
	* Calcule o valor do rendimento,
	* Mostre o valor depositado
	* Mostre o valor atual, disponível após o rendimento.

```portugol
LEIA deposito
LEIA taxa

valor_do_rendimento = deposito * taxa / 100
valor_atual_apos_rendimento = deposito + valor_do_rendimento

ESCREVA valor_do_rendimento
ESCREVA valor_atual_apos_rendimento
```

9. Faça um programa que:
	* Receba a base e a altura de um triângulo
	* Calcule a área de um triângulo.
	* Mostre a área do triângulo
	
	*Sabe-se que: Área = (base * altura) / 2*.

```portugol
LEIA base_do_triangulo
LEIA altura_do_triangulo

area_do_triangulo = (base_do_triangulo * altura_do_triangulo) / 2

ESCREVA area_do_triangulo
```

10. Faça um programa que:
	* calcule a área de um círculo,
	* mostre a área do círculo.

::Sabe-se que: Área = pi * R².::

```portugol
PI = 3.1415

LEIA raio_do_circulo
area_do_circulo = 3.1415 * raio_do_circulo ** 2

ESCREVA area_do_circulo
```

11. Faça um programa que:
	* Receba um número positivo maior que zero,
	* Calcule e mostre:
		* O número digitado ao quadrado,
		* O número digitado ao cubo,
		* A raiz do número digitado,
		* A raiz cúbica do número digitado.

```portugol
LEIA numero

numero_ao_quadrado = numero ** 2
numero_ao_cubo = numero ** 3
raiz_quadrada_do_numero = RAIZ(numero, 2)
raiz_cubica_do_mumero = RAIZ(numero, 3)

ESCREVA numero_ao_quadrado
ESCREVA numero_ao_cubo
ESCREVA raiz_quadrado_do_numero
ESCREVA raiz_cubica_do_numero
```

12. Faça um programa que:
	* receba dois números maiores que zero,
	* calcule um elevado ao outro,
	* mostre o resultado.

```portugol
LEIA um_numero
LEIA outro_numero

um_numero_elevado_ao_outro_numero = um_numero ** outro_numero

ESCREVA um_numero_elevado_ao_outro_numero
```

13. Faça um programa que:
	* Receba uma medida em pés, faça as devidas conversões e mostre os resultados em:
		* Polegadas;
		* Jardas;
		* Milhas.

::Sabe-se que: 1 pé = 12 polegadas,  3 pés = 1 jarda e 1,760 jardas = 1 milha::

```portugol
PES_PARA_POLEGADAS = 12
PES_PARA_JARDAS = 1 / 3
JARDAS_PARA_MILHAS = 1 / 1.760

LEIA pes

medida_em_polegadas = pes * PES_PARA_POLEGADAS
medida_em_jardas = pes * PES_PARA_JARDAS
medida_em_milhas = jardas * JARDAS_PARA_MILHAS

ESCREVA medida_em_polegadas
ESCREVA medida_em_jardas
ESCREVA medida_em_milhas
```

14. Faça um programa que:
	* Receba:
		* O ano atual,
		* O ano de nascimento de uma pessoa,
	* Calcule e mostre:
		*  A idade atual dessa pessoa,
		* Quantos anos ela terá em 2050,
	
```portugol
LEIA ano_atual
LEIA ano_de_nascimento

idade_atual = ano_atual − ano_de_nascimento
idade_em_2050 = 2050 − ano_nascimento

ESCREVA idade_atual
ESCREVA idade_em_2050
```

15. Faça um programa que:
	* Receba:
		* O preço de fábrica de um veículo,
		* O percentual de lucro do distribuidor,
		* Receba o percentual de impostos,
	* Calcule e mostre:
		* O valor correspondente ao lucro do distribuidor;
		* O valor correspondente aos impostos;
		* O preço final do veículo.

```portugol
LEIA preco_de_fabrica
LEIA percentual_de_lucro_do_distribuidr
LEIA percentual_do_imposto

lucro_do_distribuidor = preco_de_fabrica * percentual_de_lucro_do_distribuido / 100
valor_do_imposto = preco_de_fabrica * percentual_de_imposto / 100
preco_final =  preco_de_fabrica + lucro_do_distribuidor + valor_do_imposto

ESCREVA lucro_do_distribuidor
ESCREVA valor_do_imposto
ESCREVA preco_final
```

16. Faça um programa que:
	- Receba:
		* o número de horas trabalhadas,
		*  o valor do salário mínimo,
	* calcule o salário a receber, seguindo estas regras:
		* a hora trabalhada vale a metade do salário mínimo.
		* o imposto equivale a 3% do salário bruto.
		* o salário bruto equivale ao número de horas trabalhadas multiplicado pelo valor da hora trabalhada.
		* o salário a receber equivale ao salário bruto menos o imposto.
	* Mostre o salário a receber

```portugol
LEIA quantidade_de_horas_trabalhadas
LEIA valor_do_salario_minimo

VALOR_DA_HORA_TRABALHADA = valor_do_salario_minimo / 2
PORCENTAGEM_DO_IMPOSTO = 3 / 100

valor_salario_bruto = quantidade_de_horas_trabalhadas * VALOR_DA_HORA_TRABALHADA
valor_do_imposto = valor_salario_bruto * PORCENTAGEM_DO_IMPOSTO
valor_salario_liquido =  valor_salario_bruto - valor_do_imposto

ESCREVA valor_salario_liquido
```

17. Um trabalhador recebeu seu salário e o depositou em sua conta bancária. Esse trabalhador emitiu dois cheques e agora deseja saber seu saldo atual. 

::Sabe-se que cada operação bancária de retirada paga CPMF de 0,38% e o saldo inicial da conta está zerado.::

```portugol
PORCENTAGEM_DA_CPMF = 0.38 / 100
saldo_da_conta = 0

LEIA valor_do_salario_depositado
LEIA valor_cheque1
LEIA valor_cheque2

saldo_da_conta = saldo_da_conta + valor_do_salario_depositado

cpmf_cheque1 = valor_cheque1 * PORCENTAGEM_DA_CPMF
saque1 = valor_cheque1 + cpmf_cheque1
saldo_da_conta = saldo_da_conta - saque1

cpmf_cheque2 = cheque2 * PORCENTAGEM_DA_CPMF
saque2 = valor_cheque2 + cpmf_cheque2
saldo_da_conta = saldo_da_conta -  saque2

ESCREVA saldo
```

18. Pedro comprou um saco de ração com peso em quilos. Ele possui dois gatos, para os quais fornece a quantidade de ração em gramas. A quantidade diária de ração fornecida para cada gato é sempre a mesma. Faça um programa que:
	* receba o peso do saco de ração
	* a quantidade de ração fornecida para cada gato
Calcule e mostre:
	* quanto restará de ração no saco após cinco dias.

```portugol
DIAS_DE_CONSUMO = 5

LEIA peso_saco_em_quilos
LEIA quantidade_de_racao_consumida_em_gramas_pelo_gato1_por_dia
LEIA quantidade_de_racao_consumida_em_gramas_pelo_gato2_por_dia

peso_do_saco_em_gramas = peso_saco_em_quilos * 1000

consumo_em_gramas_do_gato1_em_5_dias = quantidade_de_racao_consumida_em_gramas_pelo_gato1_por_dia * DIAS_DE_CONSUMO
consumo_em_gramas_do_gato2_em_5_dias = quantidade_de_racao_consumida_em_gramas_pelo_gato2_por_dia * DIAS_DE_CONSUMO

total_consumido_pelos_gatos_em_5_dias_em_gramas = consumo_em_gramas_do_gato1_em_5_dias + consumo_em_gramas_do_gato2_em_5_dias

resto_no_saco_de_racao_apos_5_dias_em_gramas = peso_do_saco_em_gramas - total_consumido_pelos_gatos_em_5_dias_em_gramas

ESCREVA resto_no_saco_de_racao_apos_5_dias_em_gramas
```

19. Observe a imagem abaixo.

![](Exerc%C3%ADcios%20Resolvidos%2001%20-%20Estrutura%20Sequencial/2fe1952e-88d2-4b36-a8d7-0529f6140e86.png)

Faça um programa que receba:
	* A altura X do degrau
	* A altura que o usuário deseja alcançar subindo a escada
Calcule e mostre:
	* quantos degraus ele deverá subir para atingir seu objetivo.

::Sem se preocupar com a altura do usuário.::
::Todas as medidas fornecidas devem estar em metros.::

```portugol
LEIA altura_do_degrau, altura_desejada
quantidade_de_degraus = altura_desejada // altura_do_degrau
ESCREVA quantidade_de_degraus
```

20. Observe a imagem abaixo:

![](Exerc%C3%ADcios%20Resolvidos%2001%20-%20Estrutura%20Sequencial/c29be6ea-3394-4263-a730-2708977980ff.png)

Faça um programa que receba:
	* a medida do ângulo (em graus) formado por uma escada apoiada no chão e encostada na parede
	* altura da parede onde está a ponta da escada.

Calcule e mostre:
	* a medida dessa escada.

::Observação: as funções trigonométricas implementadas nas linguagens  de programação trabalham com medidas de ângulos em radianos.::

```portugol
LEIA angulo, altura
radiano = angulo * 3.14 / 180
escada = altura / seno(radiano)
ESCREVA escada
```

21. Observe a imagem abaixo.

![](Exerc%C3%ADcios%20Resolvidos%2001%20-%20Estrutura%20Sequencial/7550aabf-b4b1-4594-861f-f183e5ca2d0a.png)

Uma pessoa deseja pregar um quadro em uma parede. 
Faça um programa para calcular e mostrar:
	* A que distância a escada deve estar da parede.
	
A pessoa deve fornecer:
	* O tamanho da escada
	* A altura em que deseja pregar o quadro.

::Lembre-se de que o tamanho da escada deve ser maior que a altura que se deseja alcançar.::

```portugol
LEIA Z, X
Y = Z ** 2 - X ** 2
Y = Y ** 1 / 2
ESCREVA Y
```

22. Sabe-se que o quilowatt de energia custa um quinto do salário mínimo. Faça um programa que receba:
	* o valor do salário mínimo.
	* a quantidade de quilowatts consumida por uma residência.

Calcule e mostre:
	* o valor de cada quilowatt;
	* o valor a ser pago por essa residência;
	* o valor a ser pago com desconto de 15%.

```portugol
LEIA valor_do_salario, quantidade_de_quilowatt
valor_do_quilowatt = valor_do_salario / 5
valor_em_reais = valor_do_quilowatt * qquantidade_de_quilowatt
valor_do_desconto = valor_em_reais * 15 / 100
valor_com_desconto =  valor_em_reais − valor_do_desconto
ESCREVA valor_do_quilowatt, valor_em_reais, valor_com_desconto
```

23. Faça um programa que receba:
	* um número real.

Encontre e mostre:
	* a parte inteira desse número;
	* a parte fracionária desse número;
	* o arredondamento desse número.

```portugol
LEIA numero
parte_inteira_do_numero = int(numero)
parte_fracionaria = numero - parte_inteira_do_numero
numero_aredondado = arredonda(numero)
ESCREVA parte_inteira, parte_fracionada, numero_arredondado
```

24. Faça um programa que receba:
	* uma hora formada por hora e minutos (um número real), 

Calcule e mostre:
	* a hora digitada apenas em minutos.

::Lembre-se de que: para quatro e meia, deve-se digitar 4.30. Os minutos vão de 0 a 59.::

```portugol
LEIA hora
horas = pegar a parte inteira da variável hora
minutos = hora − h
conversao = (horas * 60) + (minutos * 100)
```

25. Faça um programa que receba:
	* o custo de um espetáculo teatral.
	* o preço do convite desse espetáculo.

Esse programa deverá calcular e mostrar:
	* a quantidade de convites que devem ser vendidos para que, pelo menos, o custo do espetáculo seja alcançado.

```portugol
LEIA custo, convite
quantidade = custo / convite
ESCREVA quantidade
```