# Java_Exemplos - NetBeans

CALCULADORA

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package calculadora;

import java.util.Scanner;

/**
 *
 * @author aluno
 */
public class Calculadora {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        /* Declaração do objeto leitor para leitura de dados
           do teclado
        */
        Scanner leitor = new Scanner(System.in);
        
        /* Declaração das variáveis para os números e para o resultado */
        int num1, num2, resultado = 0;
        /* Declaração da variável op que armazenará a operação a ser realizada */
        String op;
        
        /* Solicita que o usuário digite o primeiro número */
        System.out.println("Digite o primeiro numero:");
        /* Lê o primeiro número */
        num1 = leitor.nextInt();
        
        /* Solicita que o usuário digite o segundo número */
        System.out.println("Digite o segundo numero:");
        /* Lê o segundo número */
        num2 = leitor.nextInt();
        
        /* Exibe menu para o usuário escolher a operação a ser realizada */
        System.out.println("Digite a operação desejada:\n" +
                           "+ para adição \n" +
                           "- para subtração \n" +
                           "* para multiplicação \n" +
                           "/ para divisão \n" +
                           "% para módulo (resto)");
        /* Leitura da operação */
        op = leitor.next();
        
        /* Uso do switch case para verificar qual a operação desejada e efetuar
           a operação correspondente
        */
        switch (op) {
            case "+": resultado = num1 + num2;
                      System.out.println("Adição");
                      break;
            case "-": resultado = num1 - num2;
                      System.out.println("Subtração");
                      break;
            case "*": resultado = num1 * num2;
                      System.out.println("Multiplicação");
                      break;
            case "/": resultado = num1 / num2;
                      System.out.println("Divisão");
                      break;
            case "%": resultado = num1 % num2;
                      System.out.println("Módulo (Resto da divisão)");
                      break;
            default:  System.out.println("Operador inválido");
                      break;
        }
        /* Exibe o resultado da operação */
        System.out.println("Resultado = " + resultado);
    }
    
}

xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

CALCULADORA COM LOOP

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package calculadora;

import java.util.Scanner;

/**
 *
 * @author aluno
 */
public class CalculadoraComLoop {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        /* Declaração do objeto leitor para leitura de dados
           do teclado
        */
        Scanner leitor = new Scanner(System.in);
        
        /* Declaração das variáveis para os números e para o resultado */
        int num1, num2, resultado = 0;
       
        /* Declaração da variável op que armazenará a operação a ser realizada */
        String op;
        
        /* Declaração da variável resp que armazenará a resposta se o usuário
           deseja ou não continuar
        */
        String resp;
        
        do {  /* Fica em loop até o usuário escolher parar */

            /* Solicita que o usuário digite o primeiro número */
        System.out.println("Digite o primeiro numero:");
        /* Lê o primeiro número */
        num1 = leitor.nextInt();
        
        /* Solicita que o usuário digite o segundo número */
        System.out.println("Digite o segundo numero:");
        /* Lê o segundo número */
        num2 = leitor.nextInt();
        
        /* Exibe menu para o usuário escolher a operação a ser realizada */
        System.out.println("Digite a operação desejada:\n" +
                           "+ para adição \n" +
                           "- para subtração \n" +
                           "* para multiplicação \n" +
                           "/ para divisão \n" +
                           "% para módulo (resto)");
        /* Leitura da operação */
        op = leitor.next();
        
        /* Uso do switch case para verificar qual a operação desejada e efetuar
           a operação correspondente
        */
        switch (op) {
            case "+": resultado = num1 + num2;
                      System.out.println("Adição");
                      break;
            case "-": resultado = num1 - num2;
                      System.out.println("Subtração");
                      break;
            case "*": resultado = num1 * num2;
                      System.out.println("Multiplicação");
                      break;
            case "/": resultado = num1 / num2;
                      System.out.println("Divisão");
                      break;
            case "%": resultado = num1 % num2;
                      System.out.println("Módulo (Resto da divisão)");
                      break;
            default:  System.out.println("Operador inválido");
                      break;
        }
        /* Exibe o resultado da operação */
        System.out.println("Resultado = " + resultado);
        
        /* Pergunta ao usuário se deseja continuar a executar */
            System.out.println("Deseja executar novamente (S/N) ?");
            
            /* Leitura da resposta */
            resp = leitor.next();
            
        } while (resp.equals("S") || resp.equals("s"));
           // while (resp.equalsIgnoreCase("S"));
        
    }
    
}

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

ESTRUTURA DE REPETIÇÃO

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package estruturarepeticao;

/**
 *
 * @author aluno
 */
public class EstruturaRepeticao {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {

        /* Uso do for para exibir os números de 0 a 9 */
        
        for (int i = 0; i < 10; i++) {
            System.out.println(i);
        }
        System.out.println("");

        /* Uso do while para exibir os números de 0 a 9 */
        int i =0;
        while (i < 10) {
            System.out.println(i);
            i++;
        }
        System.out.println("");
        
        /* Uso do do/while para exibir os números de 0 a 9 */
        i= 0;
        do{
            System.out.println(i++);
        } while (i < 10);
        

    }
    
}

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

LEITURA DE NUMEROS

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package leituranumeros;

import java.util.Scanner;

/**
 *
 * @author aluno
 */
public class LeituraNumeros {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        /* Programa que solicita que o usuário digite 10 números,
           lê os números e exibe a soma desses 10 números.
        */
        int num, soma = 0;
        
        Scanner leitor = new Scanner(System.in);
        
        for (int i = 0; i < 10; i++) {
            /* Solicita que o usuário digite o número */
            System.out.println("Digite um número");
            /* Lê o número digitado */
            num= leitor.nextInt();
            
             /* Soma o número lido à variável soma */
             soma += num;
        }
 
        /* Exibe a soma dos números */
        System.out.println("A soma dos números é " + soma);
    }
    
}

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

MEDIA DE NUMEROS

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package medianumeros;

import java.util.Scanner;

/**
 *
 * @author aluno
 */
public class MediaNumeros {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
        /* Programa que solicita que o usuário digite vários números,
           até que ele digite um número negativo.
           O programa lê os números digitados e exibe a média dos números
           positivos.
        */
        Scanner leitor = new Scanner(System.in);
        
        int num, soma=0, cont= 0;
        float media;
        
        do {
            /* Solicita que o usuário digite um número */
            System.out.println("Digite um número");
            /* Lê o número digitado e armazena em num */
            num= leitor.nextInt();
            
            if (num > 0) {      /* Se o número digitado for positivo */
                soma += num;    /* soma o número à variável soma */
                cont++;         /* e incrementa cont */
            }
        } while (num > 0);      /* Repete o loop enquanto num for positivo */
        
        /* Calcula a média dos números */
        media = (float) soma / (float)cont;
        
        System.out.println("A soma dos números lidos positivos é " + soma);
        System.out.println("A média dos números lidos positivos é " + media);
        
        
        
    }
    
}

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

VETOR

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package vetor;

import java.util.Scanner;

/**
 *
 * @author aluno
 */
public class Vetor {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
       /* Declaração de um vetor para armazenar 5 valores
          do tipo float
        */
       float[] vetor = new float[5];
       
       /* exemplo de declaração de matriz de inteiros
          de 2 linhas e 3 colunas 
       */
       int[][] matriz = new int[2][3];
       
       Scanner leitor = new Scanner(System.in);
       
       /* Leitura de 5 valores para armazenar no vetor */
        for (int i = 0; i < vetor.length; i++) {
            System.out.println("Digite a nota " + (i + 1));
            vetor[i] = leitor.nextFloat();
        }
       
        /* Exibição dos valores do vetor */
        for (int i = 0; i < vetor.length; i++) {
            System.out.print(String.format("%.2f \t", vetor[i]));
        }
        System.out.println("");
        
        /* Leitura dos valores da matriz */
        for (int linha = 0; linha < matriz.length; linha++) {
            for (int coluna = 0; coluna < matriz[0].length; coluna++) {
                System.out.println("Digite um valor para matriz linha " + linha +
                                   " e coluna " + coluna);
                matriz[linha][coluna] = leitor.nextInt();
            }
        }

        /* Exibição dos valores da matriz */
        for (int linha = 0; linha < matriz.length; linha++) {
            for (int coluna = 0; coluna < matriz[0].length; coluna++) {
                System.out.print(matriz[linha][coluna] + "\t");
            }
            System.out.println("");
        }
        
        
        
       
    }
    
}
                
