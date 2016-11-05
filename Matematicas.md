...Java
import java.util.Scanner;

public class Matematicas {
   public static void main(String[] args)
   {
      Scanner input = new Scanner(System.in);
      
      int a, b;
      double x1, x2, y1, y2, distancia, r, r1, m;
      double medio_x, medio_y;
      
      System.out.println("Escoga:\n" + "\n1 - Calcular distancia");
      System.out.println("2 - Coordenadas de un punto medio");
      System.out.println("3 - Pendiente de una linea");
      System.out.println("4 - Centro y radio de un circulo\n");
      System.out.print("Entre un numero: ");
      a = input.nextInt();
      
      switch (a){
         case 1: System.out.println("Entre la primera coordenada (x1, y1)" + "\n");
                 System.out.print("Entre el valor x1 = ");
                 x1 = input.nextDouble();
                 System.out.print("Entre el valor y1 = ");
                 y1 = input.nextDouble();
                 System.out.println("La primera coordenada es: (" + (x1) + ", " + (y1) + ")" + "\n"); 
                 
                 System.out.println("Entre la segunda coordenada (x2, y2)" + "\n");
                 System.out.print("Entre el valor de x2 = ");
                 x2 = input.nextDouble();
                 System.out.print("Entre el valor y2 = ");
                 y2 = input.nextDouble();
                 System.out.println("La segunda coordenada es: (" + (x2) + ", " + (y2) + ")" + "\n"); 
                 
                 distancia = Math.sqrt(Math.pow( (x2 - x1), 2) + Math.pow( (y2 - y1), 2) );
                 System.out.println("La distancia entre los puntos: (" + (x1) + ", " + (y1) + "), (" + (x2) + ", " + (y2) + ") = " + (distancia));
                 break;
                 
         case 2: System.out.println("Para calcular la coordenada del punto medio:" + "\n" + "(a) de x es (x2 + x1)/2" + "\n" + "(b) de y es (y2 + y1)/2" + "\n");
                 System.out.println("Entre la primera coordenada (x1, y1)" + "\n" );
                 System.out.print("Entre el valor x1 = ");
                 x1 = input.nextDouble();
                 System.out.print("Entre el valor y1 = ");
                 y1 = input.nextDouble();
                 System.out.println("La primera coordenada es: (" + (x1) + ", " + (y1) + ")" + "\n"); 
                 
                 System.out.println("Entre la segunda coordenada (x2, y2)" + "\n" );
                 System.out.print("Entre el valor x2 = ");
                 x2 = input.nextDouble();
                 System.out.print("Entre el valor y2 = ");
                 y2 = input.nextDouble();
                 System.out.println("La segunda coordenada es: (" + (x2) + ", " + (y2) + ")" + "\n"); 
                 
                 medio_x = (x2 + x1) / 2;
                 System.out.println("El punto medio de x es: " + (medio_x));
                 medio_y = (y2 + y1) / 2;
                 System.out.println("El punto medio de y es: " + (medio_y));
                 break;
                 
         case 3: System.out.println("La ecuacion de la pendiente es: Elevacion / Recorrido" + "\n" + "m = (y2 - y1) / (x2 - x1)" + "\n");
                 System.out.println("Entra P1 = (x1, y1)");
                 System.out.print("x1 = ");
                 x1 = input.nextDouble();
                 System.out.print("y1 = ");
                 y1 = input.nextDouble();
                 System.out.println("Entra P2 = (x2, y2)");
                 System.out.print("x2 = ");
                 x2 = input.nextDouble();
                 System.out.print("y2 = ");
                 y2 = input.nextDouble();
                 m = (y2 - y1) / (x2 - x1);
                 System.out.println("La pendiente de (" + (y2) + " - " + (y1) + ") / (" + (x2) + " - " + (x1) + ") es = " + (m)); 
                 break;
                 
                      
                 
         case 4: System.out.println("La ecuacion del circulo es: (x - h)^2 + (y - k)^2 = r^2" + "\n");
                 System.out.println("Escriba la ecuacion del circulo");
                 System.out.print("x = ");
                 x1 = input.nextDouble();
                 System.out.print("h = ");
                 x2 = input.nextDouble();
                 System.out.print("y = ");
                 y1 = input.nextDouble();
                 System.out.print("k = ");
                 y2 = input.nextDouble();
                 System.out.print("r = ");
                 r = input.nextDouble();
                 System.out.println("La ecuacion del circulo que escribio es: (" + (x1) + " - " + (x2) + ")^2 + (" + (y1) + " - " + (y2) + ")^2 = " + (r) + "\n");
                 System.out.println("El centro del circulo es (h, k) = (" + (x2) + ", " + (y2) + ")" );
                 r1 = Math.sqrt(r);
                 System.out.println("El radio del circulo es = " + (r1));
                 break;        
        
      }      
      
      input.close();
   }
}
...
