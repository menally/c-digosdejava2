# import java.util.Scanner;
public class Main {
    public static void main (String[] args) {
        Scanner scanner = new Scanner(System.in);
    System.out.println("Ingresa un numero del 1 al 5 para conocer tu calificacion:");
    int calificacion = scanner.nextInt();
    switch (calificacion){
        case 1:
        System.out.println("Excelente trabajo, Tu calificacion es A , Sigue asi");
        break;
        case 2:
        System.out.println("Muy bien hecho, Tu calificacion es B, ");
        break;
        case 3:
        System.out.println("Buen esfuerzo, Tu calificacion es C");
        break;
        case 4:
            System.out.println("Aprobaste peor tienes una calificacion D, NO te rindas");
            break;
        case 5:
            System.out.println("Tu calificacion es F,Esta vez no se logro");
            break;
    }

    System.out.println("------------------");

    System.out.println("Ingresa el nombre de un mes en minusculas:");
    String mes = scanner.next() ;
    switch (mes) {
        case "diciembre":
        case "enero":
        case "febrero":
            System.out.println("La estacion es: invierno");
            break;
        case "marzo":
        case "abril":
        case "mayo":
            System.out.println("La estacion es: primavera");
            break;
        case "junio":
        case "julio":
        case "agosto":
            System.out.println("La estacion es: verano");
            break;
        case "septiembre":
        case "octubre":
        case "noviembre":
            System.out.println("La estacion es: otoño");
            break;
        default:
            System.out.println("Error:El texto ingresado no es un mes valido en minusculas ");
            break;
    }
           System.out.println("----------------------");
            System.out.println("Ingresa un numero del 1 al 3 para el nivel de videojuegos:");
            int nivel = scanner.nextInt();
            switch (nivel){
                case 1 -> System.out.println("Nivel elegido:Facil, Ideal para empezar");
                case 2 -> System.out.println("Nivel elegido: Intermedio, Preparate para un reto");
                case 3 -> System.out.println("Nivel elegido: Dificil, Solo paar expertos");
                default -> System.out.println("Error: numero de nivel incorrecto");
    }
    System.out.println("---------------------");
            System.out.println("Ingresa una letra minuscula: ");
            String letra = scanner.next();
            switch (letra){
                case "a","e","i","o","u" -> System.out.println("Es una vocal");
                default -> System.out.println("Es una consonante o caracter invalido");
            }
            System.out.println("------------------");
            System.out.println("Ingresa un numero entero:");
            int numero = scanner.nextInt();

            if (numero > 0 && numero % 2 == 0) {
                System.out.println("El numero es positivo y ademas es par");
            } else {
                System.out.println("El numero no cumple ambas condiciones, no es posotivo,par o ninguno");
            }
            System.out.println("---------------------");

            System.out.println("Ingresa tu edad:");
            int edad = scanner.nextInt();

            System.out.println("Ingrese sus años de experiencia laboral:");
            int experiencia = scanner.nextInt();

            if (edad > 21 && experiencia >=2) {
                System.out.println("Resultado: Usted es APTO para el puesto");
            } else {
                    System.out.println("Resultado: No cumple con los requisitos minimos para el puesto");
            }

    scanner.close();
    }
}