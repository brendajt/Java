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


   ## Este es el ejercicio del día 13/06/2023
   Se vieron los unicase, asi como la diferencia entre un println y un print, el primero hace un salto de línea y el ultimo solo sigue sobre la misma. 
   Vimos también para que sirve equalsIgnoreCase que ignora las mayusculas.
   También se vio para que sirven los Switch y cada uno tiene sus Case que deben terminar con un break.
   Vimos "default" para el caso en que el usuario no ponga los casos que consideramos. 


               import java.util.Scanner;
               public class Case{
                   public static void main(String[] args){
                       //int a\u00f1o=2023;  // Se utilizo el unicode de la "ñ" que es \u00f1 
                       //System.out.println("Estamos en el año " + año);
                       Scanner sc= new Scanner(System.in);
                       int mes, a\u00f1o;
                       String palabra_secreta="PILARES";
                       System.out.print("Ingresa la palabra secreta para acceder ");
                       String palabra_usuario=sc.nextLine();
                       if(palabra_secreta.equalsIgnoreCase(palabra_usuario)){
                           System.out.println("Bienvenido al Case");
                           int numero_aleatorio=(int)(Math.random()*3+1);
                           System.out.println("Tu numero aleatorio es:" + numero_aleatorio);
                           switch(numero_aleatorio){
                               case 1:
                                   System.out.println("Programa que dice numero de días de un mes seleccionado");
                                   System.out.println("¿Que año es?");
                                   a\u00f1o=sc.nextInt();
                                   System.out.println("Ingresa el numero del mes del 1 al 12: ");
                                   mes=sc.nextInt();
                                   sc.nextLine();
                                   switch(mes){
                                       case 1: case 3: case 5: case 7: case 8: case 10: case 12:
                                           System.out.print("El mes " + mes + " tiene 31 días");
                                           break;
                                       case 4: case 6: case 9: case 11:
                                           System.out.print("El mes " + mes + " tiene 30 días");
                                           break;
                                       case 2:
                                           if(a\u00f1o%4==0 && a\u00f1o%100!=0){
                                               System.out.print("El mes tiene 29 días");
                                           }else{
                                               System.out.print("El mes solo tiene 28 días");
                                           }
                                           break;
                                       default:
                                           System.out.println("No es valido este dato");
                           
                               
                                   }
                                   break;
                               case 2:
                                   System.out.println("Programa que te dice si tu año es bisiesto");
                                   System.out.println("Ingresa el año: ");
                                   a\u00f1o=sc.nextInt();
                                   sc.nextLine();
                                   break;
                               case 3:
                                   System.out.println("Programa que dice numero de mes ingresado");
                                   break;    
                           }
                       }else{
                           System.out.println("No es correcta la palabra");
                       }
                   }
               }   




### Se realizo el Código de la evaluación del moodle del 16/06/2023

         import java.util.Scanner;
         public class Instrucciones{
             public static void main(String[] args){
                 Scanner sc=new Scanner(System.in);
                 System.out.println("Inroduce un número del 1 al 7 para conocer el día de la semana");
                 int dia=sc.nextInt();
                 sc.nextLine();
                 switch(dia){
                     case 1:
                         System.out.print("El día es Lunes");
                         break;
                     case 2:
                         System.out.print("El día es Martes");
                         break;
                     case 3:
                         System.out.print("El día es Miércoles");
                         break;
                     case 4:
                         System.out.print("El día es Jueves");
                         break;
                     case 5:
                         System.out.print("El día es Viernes");
                         break;
                     case 6:
                         System.out.print("El día es Sabado");
                         break;
                     case 7:
                         System.out.print("El días es Domingo");
                         break;
                     default:
                         System.out.println("No es valido este dato");                    
                 }
             }
         }


### Se termino el programa Case.java

            import java.util.Scanner;
            public class Case{
                public static void main(String[] args){
                    //int a\u00f1o=2023;  // Se utilizo el unicode de la "ñ" que es \u00f1 
                    //System.out.println("Estamos en el año " + año);
                    Scanner sc= new Scanner(System.in);
                    int mes, a\u00f1o;
                    String palabra_secreta="PILARES";
                    System.out.print("Ingresa la palabra secreta para acceder ");
                    String palabra_usuario=sc.nextLine();
                    if(palabra_secreta.equalsIgnoreCase(palabra_usuario)){
                        System.out.println("Bienvenido al Case");
                        int numero_aleatorio=(int)(Math.random()*3+1);
                        System.out.println("Tu numero aleatorio es:" + numero_aleatorio);
                        switch(numero_aleatorio){
                            case 1:
                                System.out.println("Programa que dice numero de días de un mes seleccionado");
                                System.out.println("¿Que año es?");
                                a\u00f1o=sc.nextInt();
                                System.out.println("Ingresa el numero del mes del 1 al 12: ");
                                mes=sc.nextInt();
                                sc.nextLine();
                                
                                switch(mes){
                                    case 1: case 3: case 5: case 7: case 8: case 10: case 12:
                                        System.out.print("El mes " + mes + " tiene 31 días");
                                        break;
                                    case 4: case 6: case 9: case 11:
                                        System.out.print("El mes " + mes + " tiene 30 días");
                                        break;
                                    case 2:
                                        if(a\u00f1o%4==0 && a\u00f1o%100!=0){
                                            System.out.print("El mes tiene 29 días");
                                        }else{
                                            System.out.print("El mes solo tiene 28 días");
                                        }
                                        break;
                                    default:
                                        System.out.println("No es valido este dato");
                        
                            
                                }
                                break;
                            case 2:
                                System.out.println("Programa que te dice si tu año es bisiesto");
                                System.out.println("Ingresa el año: ");
                                a\u00f1o=sc.nextInt();
                                sc.nextLine();
                                if(a\u00f1o%4==0 && a\u00f1o%100!=0){
                                    System.out.println("El año "  + a\u00f1o  +  " SI es bisiesto");
                                }else{
                                    System.out.println("El año "  + a\u00f1o  +  " NO es bisiesto");
                                }
                                break;
                            case 3:
                                // Para el caso 3 haremos un arreglo 
                                System.out.println("Programa que dice número de mes ingresado del 1 al 12");
                                String[] meses={"enero","febrero","marzo","abril","mayo","junio","julio","agosto","septiembre","octubre","noviembre","diciembre"};
                                System.out.println("Ingresa un mes:");
                                String mes_ingresado=sc.nextLine();
                                int posicion=1;
                                for(int i= 0; i<meses.length;i++){
                                    if(meses[i].equals(mes_ingresado)){
                                        System.out.println("Para el mes "+ mes_ingresado + " le corresponde el número: " + posicion);
                                    }else{
                                        posicion++;
                                    }
                                }
                                    
                                
                            break;    
                        }
                    }else{
                        System.out.println("No es correcta la palabra");
                    }
                }
            }
