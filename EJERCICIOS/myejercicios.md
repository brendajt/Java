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
