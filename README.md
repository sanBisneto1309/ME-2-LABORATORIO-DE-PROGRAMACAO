# ME-2-LABORATORIO-DE-PROGRAMACAO
Repositório da atividade de fixação sobre repetições em Java
------------------------------------------------------------------
1-
import java.util.Scanner;

public class SenhaCorreta {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
        final int senhaCorreta = 2002;
        int senha;
        do {
            System.out.print("Digite a senha: ");
            senha = scanner.nextInt();
            if (senha != senhaCorreta) {
                System.out.println("Senha Invalida");
            } else {
                System.out.println("Acesso Permitido");
            }
        } while (senha != senhaCorreta);
        scanner.close();
	}
}
-------------------------------------------------------------------
2-
import java.util.Scanner;

public class Quadrantes {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
        int x, y;
        while (true) {
            System.out.print("Digite a coordenada X: ");
            x = scanner.nextInt();
            System.out.print("Digite a coordenada Y: ");
            y = scanner.nextInt();
            if (x == 0 || y == 0) {
                break;
            }
            if (x > 0 && y > 0) {
                System.out.println("Primeiro quadrante");
            } else if (x < 0 && y > 0) {
                System.out.println("Segundo quadrante");
            } else if (x < 0 && y < 0) {
                System.out.println("Terceiro quadrante");
            } else if (x > 0 && y < 0) {
                System.out.println("Quarto quadrante");
            }
        }
        scanner.close();
    }
}
-----------------------------------------------------------------------
3-
import java.util.Scanner;
public class Combustível {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
        int alcool = 0;
        int gasolina = 0;
        int diesel = 0;  
        while (true) {
            System.out.println("Informe o código do combustível (1.Álcool, 2.Gasolina, 3.Diesel, 4.Fim): ");
            int codigo = scanner.nextInt();
            if (codigo == 1) {
                alcool++;
            } else if (codigo == 2) {
                gasolina++;
            } else if (codigo == 3) {
                diesel++;
            } else if (codigo == 4) {
                break;
            } else {
                System.out.println("Código inválido! Tente novamente.");
            }
        }  
        System.out.println("MUITO OBRIGADO");
        System.out.println("Álcool: " + alcool);
        System.out.println("Gasolina: " + gasolina);
        System.out.println("Diesel: " + diesel);
        scanner.close();
    }
}
------------------------------------------------------------------------------------------------------------------
4-
import java.util.Scanner;

public class ValorInteiro {
	public static void main(String[] args) {
  Scanner scanner = new Scanner(System.in);
        System.out.print("Digite um valor inteiro X (1 <= X <= 1000): ");
        int x = scanner.nextInt(); 
        if (x >= 1 && x <= 1000) {
            for (int i = 1; i <= x; i += 2) {
                System.out.println(i);
            }
        } else {
            System.out.println("O valor deve estar entre 1 e 1000.");
        }
        scanner.close();
	   }
 }
 -----------------------------------------------------------------------------------
5-
import java.util.Scanner;

public class Inteiro {
	public static void main(String[] args) {
	        Scanner scanner = new Scanner(System.in);
	        System.out.print("Digite a quantidade de valores inteiros a serem lidos (N): ");
	        int n = scanner.nextInt();
	        int in = 0;
	        int out = 0;
	        for (int i = 0; i < n; i++) {
	            System.out.print("Digite o valor inteiro X: ");
	            int x = scanner.nextInt();
	            if (x >= 10 && x <= 20) {
	                in++;
	            } else {
	                out++;
	            }
	        }
	        System.out.println(in + " in");
	        System.out.println(out + " out");
	        scanner.close();
	}
}
-----------------------------------------------------------------------------------------------
6-
import java.util.Scanner;

public class eaicumparssa {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite o número de casos de teste: ");
        int n = scanner.nextInt();
        for (int i = 0; i < n; i++) {
            System.out.print("Digite o primeiro valor (com peso 2): ");
            double valor1 = scanner.nextDouble();
            System.out.print("Digite o segundo valor (com peso 3): ");
            double valor2 = scanner.nextDouble();
            System.out.print("Digite o terceiro valor (com peso 5): ");
            double valor3 = scanner.nextDouble();
            double mediaPonderada = (valor1 * 2 + valor2 * 3 + valor3 * 5) / 10.0;
            System.out.printf("Média ponderada: %.1f%n", mediaPonderada);
        }
        scanner.close();
    }
}
