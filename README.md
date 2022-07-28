# Preenchendo-e-somando-vetores-codigo-Java


Damares Costa de Souza 
Moodle - IFRS

Programação Básica com Java III - Turma 2022B
Painel Meus cursos  PBJIII2022B 2. Vetores  Teste seus conhecimentos 2
Iniciado em	quinta, 28 jul 2022, 17:08
Estado	Finalizada
Concluída em	quinta, 28 jul 2022, 17:37
Tempo empregado	29 minutos 10 segundos
Avaliar	9,00 de um máximo de 10,00(90%)
Questão 1
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Complete o programa abaixo de forma que leia um vetor de 20 números inteiros e gere um segundo vetor cujas posições pares são o dobro do vetor original e as ímpares o triplo.



public class ModificaVetor {
	public static void main(String[] args) {
		int[] vetor = new int[20];
		
		// Leitura
		for(int cont = 0; cont < vetor.length; cont++) {
			System.out.printf("vetor[%d]: ", cont);
			vetor[cont] = Integer.parseInt(System.console().readLine());
		}
		
		// Processamento
		for(int cont = 0; cont < vetor.length; cont++) {
			if(________________________)
				vetor[cont] *= 2;
			else
				vetor[cont] *= 3;
		}
		
		// Saida
		System.out.println("\n----------------- NOVO VETOR -----------------");
		for(int cont = 0; cont < vetor.length; cont++) {
			System.out.printf("vetor[%d] = %d\n", cont, vetor[cont]);
		}
	}
}

Escolha uma opção:

a.
cont % 2 == 0


b.
cont % 2 != 0


c.
vetor[cont] % 2 == 0


d.
vetor % 2 == 0


e.
vetor[cont] % 2 != 0

Feedback
Sua resposta está correta.
A resposta correta é: cont % 2 == 0
Questão 2
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Complete o programa Java abaixo de forma que leia um vetor de tamanho 15 e mostre os números das posições que contém o valor 30.



public class Mostra30 {
	public static void main(String[] args) {
		int[] vetor = new int[15];
		
		// Leitura
		for(int cont = 0; cont < vetor.length; cont++) {
			System.out.printf("vetor[%d]: ", cont);
			vetor[cont] = Integer.parseInt(System.console().readLine());
		}
		
		// Processamento e Saída
		boolean achou = false;
		System.out.println("\nPosicoes do vetor com elementos iguais a 30: ");
		for(int cont = 0; cont < vetor.length; cont++) {
			if(vetor[cont] == 30) {
				achou = true;
				System.out.printf("%d ", ____________________________);
			}
		}
		System.out.println();
		
		if(!achou)
			System.out.println("Nenhuma posicao do vetor contem o valor 30!");
	}
}

Escolha uma opção:

a.
cont


b.
vetor[cont]


c.
cont[vetor]

d.
vetor

e.
achou

Feedback
Sua resposta está correta.
A resposta correta é: cont
Questão 3
Incorreto
Atingiu 0,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Complete o trecho de código abaixo, de forma que a estrutura for passe por todas as posições do vetor nome.



                for(int cont = 0; cont < Resposta
Media.length
; cont++) {
			if(media[cont] < 7)
				System.out.println(nome[cont]);
			if(cont == 0 || media[cont] > maiorMedia) {
				maiorMedia = media[cont];
				nomeMaior = nome[cont];
	  		}
		}



Feedback
A resposta correta é: nome.length
Questão 4
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Escreva um programa que leia a pontuação de 20 times de um campeonato de futebol. O programa deve mostrar, ao final, qual a pontuação dos campeões, bem como mostrar quantos times dividiram o título.

Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.



public class VerificaCampeoes {
	public static void main(String[] args) {
		int[] pontos = new int[20]; 
		
		// Leitura
		for(int cont = 0; cont < pontos.length; cont++) {
			System.out.printf("Pontuacao do time %d: ", cont+1);
			pontos[cont] = Integer.parseInt(System.console().readLine()); 
		}
		
		// Processamento
		int maior = pontos[0]; 
		for(int cont = 1; cont < pontos.length; cont++) {
			if(maior < pontos[cont]) 
				maior = pontos[cont]; 
		}
		
		int campeoes = 0;
		for(int cont = 0; cont < pontos.length; cont++) {
			if(pontos[cont] == maior) 
				campeoes++;
		}
		
		// Saida
		System.out.printf("\nNUMERO DE CAMPEOES = %d\n", campeoes);
	}
}

     
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o seguinte problema:

Escreva um programa que leia a pontuação de 20 times de um campeonato de futebol. O programa deve mostrar, ao final, qual a pontuação dos campeões, bem como mostrar quantos times dividiram o título.

Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.



public class VerificaCampeoes {
	public static void main(String[] args) {
		[int[] pontos = new int[20];]
		
		// Leitura
		for(int cont = 0; cont < pontos.length; cont++) {
			System.out.printf("Pontuacao do time %d: ", cont+1);
			[pontos[cont] = Integer.parseInt(System.console().readLine());]
		}
		
		// Processamento
		[int maior = pontos[0];]
		for(int cont = 1; cont < pontos.length; cont++) {
			[if(maior < pontos[cont])]
				[maior = pontos[cont];]
		}
		
		int campeoes = 0;
		for(int cont = 0; cont < pontos.length; cont++) {
			[if(pontos[cont] == maior)]
				campeoes++;
		}
		
		// Saida
		System.out.printf("\nNUMERO DE CAMPEOES = %d\n", campeoes);
	}
}

Questão 5
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o problema abaixo:

Faça um programa para controlar o estoque de mercadorias de uma empresa. Inicialmente, o programa deverá preencher dois vetores com dez posições cada, onde o primeiro corresponde ao código do produto e o segundo ao total desse produto em estoque. Logo após, o programa deverá ler o código de um produto comprado por um cliente juntamente com a quantidade. O programa deverá verificar:

se o código do produto solicitado existe. Se existir, tentar atender ao pedido; caso contrário, exibir mensagem “Código inexistente”;
cada pedido feito por um cliente só pode ser atendido integralmente. Caso isso não seja possível, mostrar a mensagem “Não temos estoque suficiente desta mercadoria”. Se puder atende-lo, mostrar a mensagem “Pedido atendido!”;
efetuar a atualização do estoque (subtrair de seu valor a quantidade) somente se o pedido for atendido integralmente;
no final do programa, escrever os códigos dos produtos com seus respectivos estoques já atualizados.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.

public class GerenciaEstoque {
	public static void main(String[] args) {
		int[] codigos = new int[10];
		int[] estoque = new int[10]; 
		
		// Leitura
		for(int cont = 0; cont < codigos.length; cont++) {
			System.out.printf("-------------------------- PRODUTO %02d --------------------------\n", cont+1);
			System.out.print("Codigo: ");
			codigos[cont] = Integer.parseInt(System.console().readLine()); 
			System.out.print("Quant. em estoque: ");
			 em branco 
		}
		
		System.out.println("\n----------------------------- COMPRA -----------------------------");
		System.out.print("Codigo do produto: ");
		int codProd = Integer.parseInt(System.console().readLine()); 
		System.out.print("Quantidade comprada: ");
		int quant = Integer.parseInt(System.console().readLine()); 
		
		// Processamento e Saída
		boolean achou = false;
		for(int cont = 0; cont < codigos.length; cont++) {
			if(codigos[cont] == codProd ) {
				achou = true; 
				if(quant <= estoque[cont] ) {
					System.out.println("\nPedido atendido!");
					estoque[cont] ‑= quant; 
				} else {
					System.out.println("\nNao temos estoque suficiente desta mercadoria.");
				}
			}
		}
		
		if(!achou)
			System.out.println("\nCodigo inexistente!");
		
		System.out.println();
		for(int cont = 0; cont < codigos.length; cont++) {
			System.out.printf("-------------------------- PRODUTO %02d --------------------------\n", cont+1);
			System.out.printf("Codigo: %d\n", codigos[cont]);
			System.out.printf("Quant. em estoque: %d\n", estoque[cont]);
		}
	}
}

    estoque[cont] = Integer.parseInt(System.console().readLine());    
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o problema abaixo:

Faça um programa para controlar o estoque de mercadorias de uma empresa. Inicialmente, o programa deverá preencher dois vetores com dez posições cada, onde o primeiro corresponde ao código do produto e o segundo ao total desse produto em estoque. Logo após, o programa deverá ler o código de um produto comprado por um cliente juntamente com a quantidade. O programa deverá verificar:

se o código do produto solicitado existe. Se existir, tentar atender ao pedido; caso contrário, exibir mensagem “Código inexistente”;
cada pedido feito por um cliente só pode ser atendido integralmente. Caso isso não seja possível, mostrar a mensagem “Não temos estoque suficiente desta mercadoria”. Se puder atende-lo, mostrar a mensagem “Pedido atendido!”;
efetuar a atualização do estoque (subtrair de seu valor a quantidade) somente se o pedido for atendido integralmente;
no final do programa, escrever os códigos dos produtos com seus respectivos estoques já atualizados.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.

public class GerenciaEstoque {
	public static void main(String[] args) {
		int[] codigos = new int[10];
		[int[] estoque = new int[10];]
		
		// Leitura
		for(int cont = 0; cont < codigos.length; cont++) {
			System.out.printf("-------------------------- PRODUTO %02d --------------------------\n", cont+1);
			System.out.print("Codigo: ");
			[codigos[cont] = Integer.parseInt(System.console().readLine());]
			System.out.print("Quant. em estoque: ");
			[estoque[cont] = Integer.parseInt(System.console().readLine());]
		}
		
		System.out.println("\n----------------------------- COMPRA -----------------------------");
		System.out.print("Codigo do produto: ");
		[int codProd = Integer.parseInt(System.console().readLine());]
		System.out.print("Quantidade comprada: ");
		[int quant = Integer.parseInt(System.console().readLine());]
		
		// Processamento e Saída
		boolean achou = false;
		for(int cont = 0; cont < codigos.length; cont++) {
			if([codigos[cont] == codProd]) {
				[achou = true;]
				if([quant <= estoque[cont]]) {
					System.out.println("\nPedido atendido!");
					[estoque[cont] ‑= quant;]
				} else {
					System.out.println("\nNao temos estoque suficiente desta mercadoria.");
				}
			}
		}
		
		if(!achou)
			System.out.println("\nCodigo inexistente!");
		
		System.out.println();
		for(int cont = 0; cont < codigos.length; cont++) {
			System.out.printf("-------------------------- PRODUTO %02d --------------------------\n", cont+1);
			System.out.printf("Codigo: %d\n", codigos[cont]);
			System.out.printf("Quant. em estoque: %d\n", estoque[cont]);
		}
	}
}

Questão 6
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Faça um algoritmo que leia o nome, o custo e o preço de 20 produtos. Ao final deverá relacionar os produtos que:

Tem lucro menor que 10%;
Tem lucro entre 10% e 30%;
Tem lucro maior que 30%.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.

public class VerificaLucros {
	public static void main(String[] args) {
		String[] nomes = new String[20];
		double[] custos = new double[20];
		double[] precos = new double[20];
		
		// Leitura
		for(int cont = 0; cont < nomes.length ; cont++) {
			System.out.printf("-------------------------- PRODUTO %02d --------------------------\n", cont+1);
			System.out.print("Nome: ");
			nomes[cont] = System.console().readLine();
			System.out.print("Custo: ");
			custos[cont] = Double.parseDouble(System.console().readLine());
			System.out.print("Preco: ");
			precos[cont] = Double.parseDouble(System.console().readLine()); 
		}
		
		// Processamento e Saída (produtos com lucro menor do que 10%)
		System.out.println("Produtos com menos de 10% de lucro:");
		for(int cont = 0; cont < nomes.length; cont++) {
			double lucro = precos[cont] - custos[cont];
			if(lucro < precos[cont] * 0.10) 
				System.out.println(nomes[cont]);
		}
		
		// Processamento e Saída (produtos com lucro entre 10% e 30%)
		System.out.println("Produtos com lucro entre 10% e 30%:");
		for(int cont = 0; cont < nomes.length; cont++) {
			double lucro = precos[cont] - custos[cont];
			if(lucro <= precos[cont] * 0.30 && lucro >=  precos[cont] * 0.10) 
				System.out.println(nomes[cont]);
		}
		
		// Processamento e Saída (produtos com lucro maior do que 30%)
		System.out.println("Produtos com lucro maior que 30%:");
		for(int cont = 0; cont < nomes.length; cont++) {
			double lucro = precos[cont] - custos[cont];
			if(lucro > precos[cont] * 0.30) 
				System.out.println(nomes[cont]);
		}
	}
}

    
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o seguinte problema:

Faça um algoritmo que leia o nome, o custo e o preço de 20 produtos. Ao final deverá relacionar os produtos que:

Tem lucro menor que 10%;
Tem lucro entre 10% e 30%;
Tem lucro maior que 30%.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.

public class VerificaLucros {
	public static void main(String[] args) {
		String[] nomes = new String[20];
		double[] custos = new double[20];
		double[] precos = new double[20];
		
		// Leitura
		for(int cont = 0; cont < [nomes.length]; cont++) {
			System.out.printf("-------------------------- PRODUTO %02d --------------------------\n", cont+1);
			System.out.print("Nome: ");
			nomes[cont] = System.console().readLine();
			System.out.print("Custo: ");
			custos[cont] = Double.parseDouble(System.console().readLine());
			System.out.print("Preco: ");
			[precos[cont] = Double.parseDouble(System.console().readLine());]
		}
		
		// Processamento e Saída (produtos com lucro menor do que 10%)
		System.out.println("Produtos com menos de 10% de lucro:");
		for(int cont = 0; cont < nomes.length; cont++) {
			double lucro = precos[cont] - custos[cont];
			[if(lucro < precos[cont] * 0.10)]
				System.out.println(nomes[cont]);
		}
		
		// Processamento e Saída (produtos com lucro entre 10% e 30%)
		System.out.println("Produtos com lucro entre 10% e 30%:");
		for(int cont = 0; cont < nomes.length; cont++) {
			double lucro = precos[cont] - custos[cont];
			[if(lucro <= precos[cont] * 0.30 && lucro >= precos[cont] * 0.10)]
				System.out.println(nomes[cont]);
		}
		
		// Processamento e Saída (produtos com lucro maior do que 30%)
		System.out.println("Produtos com lucro maior que 30%:");
		for(int cont = 0; cont < nomes.length; cont++) {
			double lucro = precos[cont] - custos[cont];
			[if(lucro > precos[cont] * 0.30)]
				System.out.println(nomes[cont]);
		}
	}
}

Questão 7
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Escreva um programa que leia dois vetores contendo números reais com 10 posições e preenche um terceiro vetor de 10 posições, contendo a multiplicação dos números presentes em cada um dos dois primeiros vetores. Por exemplo, a posição 1 do terceiro vetor conterá a multiplicação dos valores armazenados na posição 1 dos dois primeiros vetores. O programa deve mostrar então a soma dos valores de todas as posições do terceiro vetor.

Complete o programa abaixo arrastando e soltando os trechos de código nos espaços em branco, de forma que o programa implemente corretamente o problema acima.



public class ProdutoEscalar {
	public static void main(String[] args) {
		double[] vetorA = new double[10];
		double[] vetorB = new double[10];
		double[] resultados = new double[10]; 
		
		// Leitura
		for(int cont = 0; cont < vetorA.length; cont++) {
			System.out.printf("Vetor A posicao %d: ", cont);
			vetorA[cont] = Double.parseDouble(System.console().readLine()); 
		}
		for(int cont = 0; cont < vetorB.length; cont++) {
			System.out.printf("Vetor B posicao %d: ", cont);
			vetorB[cont] = Double.parseDouble(System.console().readLine()); 
		}
		
		// Processamento
		for(int cont = 0; cont < vetorA.length; cont++) {
			resultados[cont] = vetorA[cont] * vetorB[cont]; 
		}
		
		double soma = 0;
		for(int cont = 0; cont < resultados.length; cont++) {
			soma += resultados[cont]; 
		}
		
		// Saida
		System.out.printf("\nSOMA DOS PRODUTOS DOS ELEMENTOS DOS VETORES (PRODUTO ESCALAR) = %f\n", soma);
	}
}

    
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o seguinte problema:

Escreva um programa que leia dois vetores contendo números reais com 10 posições e preenche um terceiro vetor de 10 posições, contendo a multiplicação dos números presentes em cada um dos dois primeiros vetores. Por exemplo, a posição 1 do terceiro vetor conterá a multiplicação dos valores armazenados na posição 1 dos dois primeiros vetores. O programa deve mostrar então a soma dos valores de todas as posições do terceiro vetor.

Complete o programa abaixo arrastando e soltando os trechos de código nos espaços em branco, de forma que o programa implemente corretamente o problema acima.



public class ProdutoEscalar {
	public static void main(String[] args) {
		double[] vetorA = new double[10];
		double[] vetorB = new double[10];
		[double[] resultados = new double[10];]
		
		// Leitura
		for(int cont = 0; cont < vetorA.length; cont++) {
			System.out.printf("Vetor A posicao %d: ", cont);
			[vetorA[cont] = Double.parseDouble(System.console().readLine());]
		}
		for(int cont = 0; cont < vetorB.length; cont++) {
			System.out.printf("Vetor B posicao %d: ", cont);
			[vetorB[cont] = Double.parseDouble(System.console().readLine());]
		}
		
		// Processamento
		for(int cont = 0; cont < vetorA.length; cont++) {
			[resultados[cont] = vetorA[cont] * vetorB[cont];]
		}
		
		double soma = 0;
		for(int cont = 0; cont < resultados.length; cont++) {
			[soma += resultados[cont];]
		}
		
		// Saida
		System.out.printf("\nSOMA DOS PRODUTOS DOS ELEMENTOS DOS VETORES (PRODUTO ESCALAR) = %f\n", soma);
	}
}

Questão 8
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Faça um programa que preencha um vetor com seis elementos numéricos inteiros, e após calcule e mostre:

todos os números pares;
a quantidade de números pares;
todos os números ímpares;
a quantidade de números ímpares.
Complete o seguinte programa em Java, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema seja corretamente implementado.

public class VetorNumeros {
	public static void main(String[] args) {
		int[] vetor = new int[6];
		
		// Leitura
		for(int cont = 0; cont < vetor.length; cont++) {
			System.out.printf("Posicao %d: ", cont); 
			vetor[cont] = Integer.parseInt(System.console().readLine()); 
		}
		
		// Numeros pares
		int quantPares = 0;
		System.out.print("Numeros pares:");
		for(int cont = 0; cont < vetor.length ; cont++) {
			if(vetor[cont] % 2 == 0) {
				System.out.printf(" %d", vetor[cont]); 
				quantPares++;
			}
		}
		System.out.printf("\nQuantidade de numeros pares = %d\n", quantPares);
		
		// Numeros impares
		int quantImpares = 0;
		System.out.print("Numeros impares:");
		for(int cont = 0; cont < vetor.length; cont++) {
			if(vetor[cont] % 2 != 0) {
				System.out.printf(" %d", vetor[cont]);
				quantImpares++; 
			}
		}
		System.out.printf("\nQuantidade de numeros impares = %d\n", quantImpares);
	}
}

    
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o seguinte problema:

Faça um programa que preencha um vetor com seis elementos numéricos inteiros, e após calcule e mostre:

todos os números pares;
a quantidade de números pares;
todos os números ímpares;
a quantidade de números ímpares.
Complete o seguinte programa em Java, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema seja corretamente implementado.

public class VetorNumeros {
	public static void main(String[] args) {
		int[] vetor = new int[6];
		
		// Leitura
		for(int cont = 0; cont < vetor.length; cont++) {
			[System.out.printf("Posicao %d: ", cont);]
			[vetor[cont] = Integer.parseInt(System.console().readLine());]
		}
		
		// Numeros pares
		int quantPares = 0;
		System.out.print("Numeros pares:");
		for(int cont = 0; cont < [vetor.length]; cont++) {
			if(vetor[cont] % 2 == 0) {
				[System.out.printf(" %d", vetor[cont]);]
				quantPares++;
			}
		}
		System.out.printf("\nQuantidade de numeros pares = %d\n", quantPares);
		
		// Numeros impares
		int quantImpares = 0;
		System.out.print("Numeros impares:");
		for(int cont = 0; cont < vetor.length; cont++) {
			if(vetor[cont] % 2 != 0) {
				System.out.printf(" %d", vetor[cont]);
				[quantImpares++;]
			}
		}
		System.out.printf("\nQuantidade de numeros impares = %d\n", quantImpares);
	}
}
