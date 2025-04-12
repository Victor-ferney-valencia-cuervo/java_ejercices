# ejercicio 1

import java.util.Scanner;

public class OperacionesBasicas {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Introduce el primer numero: ");
        double num1 = sc.nextDouble();

        System.out.print("Introduce el segundo numero: ");
        double num2 = sc.nextDouble();

        double suma = num1 + num2;
        double resta = num1 - num2;
        double multiplicacion = num1 * num2;
        double division = (num2 != 0) ? num1 / num2 : Double.NaN;
        double modulo = (num2 != 0) ? num1 % num2 : Double.NaN;

        System.out.println("\nResultados:");
        System.out.println("Suma: " + suma);
        System.out.println("Resta: " + resta);
        System.out.println("Multiplicacion: " + multiplicacion);
        System.out.println("Division: " + (num2 != 0 ? division : "No se puede dividir por cero"));
        System.out.println("Modulo: " + (num2 != 0 ? modulo : "No se puede calcular el módulo con divisor cero"));

        sc.close();
    }
}


