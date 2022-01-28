INTRODUÇÃO A JAVA.

1. Faça um sistema que leia a idade de uma pessoa expressa em anos, meses e
dias e mostre-a expressa apenas em dias.
 */
package ListaExercicios1;

import java.util.Scanner;

public class Exercicio1 {

	public static void main(String[] args) {
		Scanner leia = new Scanner (System.in);

		int idade_anos, idade_meses, idade_dias, diasVida;

		System.out.println("Quantos anos você tem? ");
		idade_anos = leia.nextInt();

		idade_anos = (365*idade_anos);

		System.out.println("Quantos meses faltam para o seu aniverário?Mínimo 1 mês tá :) ");
		idade_meses = leia.nextInt();

		idade_meses = (12-idade_meses);

		System.out.println("Quantos dias faltam para o dia correspondente ao seu aniver ");
		idade_dias = leia.nextInt();

		diasVida = idade_anos+idade_meses+idade_dias;


		System.out.println("A sua idade em dias de vida é:"+diasVida);
		leia.close();
