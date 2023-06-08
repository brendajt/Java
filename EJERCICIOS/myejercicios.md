   ## Este es el código del ejercicio sobre la antigüedad de los trabajadores dependiendo de su área y años de trabajo. 
   
   
         import java.util.Scanner;
          public class Sistema{
              public static void main (String[] args){
                  String nombre;
                  int clave;
                  int antiguedad;
                  Scanner sc= new Scanner(System.in);
                  System.out.println("Bienvenido al sistema");
                  System.out.println("¿Cuál es el nombre del trabajador");
                  nombre = sc.nextLine();
                  System.out.println("¿Cuántos años de servicio tiene el trabajador?");
                  antiguedad = sc.nextInt();
                  System.out.println("¿Cuál es la clave de su departamento?");
                  clave = sc.nextInt();
                  if(clave==1){
                      if(antiguedad==1){
                          System.out.println(nombre + " tiene derecho a 6 días");
                      }else if(antiguedad>=2 && antiguedad<=6){
                          System.out.println(nombre + " tiene derecho a 14 días");
                      }else if(antiguedad==7){
                          System.out.println(nombre + " tiene derecho a 16 días");
                      }else{
                          System.out.println(nombre + " aun no tine derecho a vacaciones");
                      }
                  }else if(clave==2){
                      if(antiguedad==1){
                          System.out.println(nombre + " tiene derecho a 7 días");
                      }else if(antiguedad>=2 && antiguedad<=6){
                          System.out.println(nombre + " tiene derecho a 15 días");
                      }else if(antiguedad==7){
                          System.out.println(nombre + " tiene derecho a 22 días");
                      }else{
                          System.out.println(nombre + " aun no tine derecho a vacaciones");
                      }

                  }else if(clave==3){
                      if(antiguedad==1){
                          System.out.println(nombre + " tiene derecho a 10 días");
                      }else if(antiguedad>=2 && antiguedad<=6){
                          System.out.println(nombre + " tiene derecho a 20 días");
                      }else if(antiguedad==7){
                          System.out.println(nombre + " tiene derecho a 30 días");
                      }else{
                          System.out.println(nombre + " aun no tine derecho a vacaciones");
                      }

                  }else{
                      System.out.println("Error, la clave de departamento no existe");
                  }

              }
          }




## Aquí se hace los ejercicios del 08/06/23

### Programa Vacaciones;

      import java.util.Scanner;

      public class Sistemas {
          public static void main (String[] args){
              String nombre;
              int clave;
              int antiguedad;
              String i="si";
              Scanner sc= new Scanner(System.in);
              System.out.println("Bienvenido al sistema");
              // Empieza el WHILE


              while (i.equals("si")){ // en java usamos en las cadenas = para signación == para medir "tipo" y equals(como si fuera ===) para comparar tipo y contenido
                  System.out.println("¿Cuál es el nombre del trabajador?");
                  nombre = sc.nextLine();
                  System.out.println("¿Cuántos años de servicio tiene el trabajador?");
                  antiguedad = sc.nextInt();
                  sc.nextLine(); // mañana explico esta parte
                  System.out.println("¿Cuál es la clave de su departamento?");
                  clave = sc.nextInt();
                  sc.nextLine(); // mañana explico esta parte

                          // EMPEZAMOS CON LAS CONDICIONALES




                  if(clave==1){
                      if(antiguedad==1){
                          System.out.println(nombre + " tiene derecho a 6 días");
                      }else if(antiguedad>=2 && antiguedad<=6){
                          System.out.println(nombre + " tiene derecho a 14 días");
                      }else if(antiguedad==7){
                          System.out.println(nombre + " tiene derecho a 16 días");
                      }else{
                          System.out.println(nombre + " aun no tine derecho a vacaciones");
                      }
                  }else if(clave==2){
                      if(antiguedad==1){
                          System.out.println(nombre + " tiene derecho a 7 días");
                      }else if(antiguedad>=2 && antiguedad<=6){
                          System.out.println(nombre + " tiene derecho a 15 días");
                      }else if(antiguedad==7){
                          System.out.println(nombre + " tiene derecho a 22 días");
                      }else{
                          System.out.println(nombre + " aun no tine derecho a vacaciones");
                      }

                  }else if(clave==3){
                      if(antiguedad==1){
                          System.out.println(nombre + " tiene derecho a 10 días");
                      }else if(antiguedad>=2 && antiguedad<=6){
                          System.out.println(nombre + " tiene derecho a 20 días");
                      }else if(antiguedad==7){
                          System.out.println(nombre + " tiene derecho a 30 días");
                      }else{
                          System.out.println(nombre + " aun no tine derecho a vacaciones");
                      }

                  }else{
                      System.out.println("Error, la clave de departamento no existe");
                  }


                  System.out.println("Seguimos con el programa si/no");
                  i=sc.nextLine();


              }
          }
      }
      
     
   ### Codigo de los pares e impares 
   
         import java.util.Scanner;
      public class ParesImpares{
          public static void main(String[] args) {
              Scanner sc = new Scanner(System.in);
              System.out.println("Ingrese un numero del 1 al 10");
              int numero=sc.nextInt();
              sc.nextLine();

              for(int i=1; i<=10; i++){
                  if(i==numero){
                      System.out.println(numero + " este es tu número");
                      continue;
                  }
                  if(i>=7){
                      System.out.println("Alcanzo el limite ");
                      break;
                  }
                  // Este capta los primeros 10
                  if(i%2==0){
                      System.out.println(i + " Es un número par");
                  }else{
                      System.out.println(i + " Es un número impar");
                  }
              }
              // System.out.println("ingresa un nombre");
              // String nombre = sc.nextLine();
              // System.out.println("Ingrese edad");
              // int edad = sc.nextInt();
              // sc.nextLine(); // siempre que se pida un numero hay que hacer un salto de linea
              // System.out.println("ingresa apellido");
              // String apellido=sc.nextLine();

              // while (nombre.equals("juan")){  // Evalua el tipo de dato y no de donde viene
              //         System.out.println(nombre);
              //         System.out.println(edad);
              //         System.out.println(apellido);
              //         System.out.println("ingresa otro nombre");
              //         nombre=sc.nextLine();

          }


      }

   

