# LED-em-JAVA

/*
*   Faça um programa onde ocorre o calculo de quantas LEDS a pessoa vai usar dependendo do número que ela digitar
*   Exemplo: Ela escolhe o número 18
*   esse número tem 9 Leds.
*   O valor de cada Led será informado abaixo para ajudar no desenvolvimento do projeto
*
*   Valores de cada Led;
*   1 = 2;
*   2 = 5;
*   3 = 5;
*   4 = 4;
*   5 = 5;
*   6 = 6;
*   7 = 3;
*   8 = 7;
*   9 = 6;
*   0 = 6;
 */

package br.com.abc.introducao;

import java.util.Scanner;

public class TesteLED {
    public static void main(String[] args){

        Scanner leitor = new Scanner(System.in);
        int val = Integer.parseInt(leitor.nextLine());/*Quantidade de vezes*/
        int cota = 0;


        String[] vetor = new String[val];

        /*Preenchimento do meu vetor*/
        for(int i = 0; i < val; i++){
        cota = 0;
            System.out.println("Digite o " + (i + 1) + "º numero: ");

            vetor[i] = leitor.nextLine();

                /*
                * Usar charAt(j)
                * Usar Integer
                * Usar parseInt
                *
                */

                for(int j = 0; j < vetor[i].length(); j++)

                if (vetor[i].charAt(j) == '1') {
                    cota = cota + 2;
                } else if (vetor[i].charAt(j) == '2') {
                    cota = cota + 5;
                } else if (vetor[i].charAt(j) == '3') {
                    cota = cota + 5;
                } else if (vetor[i].charAt(j) == '4') {
                    cota = cota + 4;
                } else if (vetor[i].charAt(j) == '5') {
                    cota = cota + 5;
                } else if (vetor[i].charAt(j) == '6') {
                    cota = cota + 6;
                } else if (vetor[i].charAt(j) == '7') {
                    cota = cota + 3;
                } else if (vetor[i].charAt(j) == '8') {
                    cota = cota + 7;
                } else if (vetor[i].charAt(j) == '9') {
                    cota = cota + 6;
                } else if (vetor[i].charAt(j) == '0') {
                    cota = cota + 6;
                }
            System.out.println("Numero de Leds = "+cota);
        }

    }
}


