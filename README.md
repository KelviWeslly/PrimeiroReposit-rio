package lista6exercicio;

import java.util.Scanner;

public class questão1matrizes {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

//		Questão 1. Dada uma matriz de ordem 4x3 contendo valores numéricos reais. Faça um 
//		algoritmo que calcule e exiba a soma dos números positivos e a soma dos números 
//		negativos.
		
		

		 		Scanner scan = new Scanner(System.in);

		       
		        double[][] matriz = new double[4][3];

		        
		        double somadosPositivos = 0;
		        double somadosNegativos = 0;

		     
		        for (int i = 0; i < 4; i++) {
		            for (int j = 0; j < 3; j++) {
		                System.out.print("Digite o valor da posição [" + i + "][" + j + "]: ");
		                matriz[i][j] = scan.nextDouble();
		            }
		        }

		  
		        for (int i = 0; i < 4; i++) {
		            for (int j = 0; j < 3; j++) {

		                if (matriz[i][j] > 0) {
		                    somadosPositivos += matriz[i][j];
		                } else if (matriz[i][j] < 0) {
		                    somadosNegativos += matriz[i][j];
		                }
		            }
		        }

		      
		        System.out.println("\nSoma dos numeros positivos: " + somadosPositivos);
		        System.out.println("Soma dos numeros negativos: " + somadosNegativos);

		        scan.close();
	}

}
