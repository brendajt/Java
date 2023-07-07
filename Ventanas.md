## Creación de las ventanas 

    import javax.swing.*; //Traemos todo con el *
    // Vamos a crear la clase heredada
    public class Ventana extends JFrame{
        private JLabel ventana1;
        private JLabel ventana2; // hay que crear uno por cada uno
        // Creamos el método constructor que lleva el nombre de la clase
        public Ventana(){ //los parentesís vacíos nos indican que es un método constructor
            setLayout(null); //No da un tamaño por defaul, yo lo haré
            ventana1 = new JLabel("Ventana 1"); // mi primer lagout
            ventana1.setBounds(0,0,200,100); // le dimos tamaño a la etiqueta que esta dentro
            add(ventana1); // agregar al lagout, arriba lo creamos, aqui lo agregamos
    
            ventana2 = new JLabel("Bienvenido al programa de JAVA");
            ventana2.setBounds(-10,-10,200,100);
            add(ventana2);
        }
    
        public static void main(String args[]){
            // voy a crear una nueva ventana llamada ventana 1
            Ventana ventana1= new Ventana();
            //La ventana tendrá caracteristicas 
            ventana1.setBounds(0,0,300,400); //Para definir tamaño, eje x eje y, anchura, altura
            ventana1.setVisible(true);// Debemos de decir que la ventana es o no visible
            ventana1.setResizable(false); // bloquea al usuario para modificar el tamaño de la ventana
            // Vamos a crear el contenido de adentro de la ventana 
            // Interfaz, lagout, funcionalidad deben tener estas 3 cosas las ventanas
    
    }
    }


## Creación de los botones 

    import javax.swing.*;
    import java.awt.event.*; // escuchar cuando pase algo
    public class Boton extends JFrame implements ActionListener{// implementa ademas la accion de escuchar
        private JButton boton1; //declarando el boton 
    // vamos a crear el metodo constructor
        public Boton(){
            setLayout(null); // no le des tamaño ni posición, yo se la daré
            boton1 = new JButton("Cerrar");
            boton1.setBounds(100,200,100,30);
            add(boton1);
            boton1.addActionListener(this);
        
        }
        public void actionPerformed(ActionEvent evento){
            if(evento.getSource() == boton1){
                System.exit(0); // cierra la ventana si ocurre el evento sobre el boton.
    
            }
        }
    
        public static void main(String args[]){
            Boton boton1 = new Boton();
            boton1.setBounds(50,50,300,400);
            boton1.setVisible(true);
            //add(boton1);
        }
    
    }

## Creación boton 2

    import javax.swing.*;
    import java.awt.event.*;
    public class Boton2 extends JFrame implements ActionListener{
        private JButton boton1,boton2,boton3;
        private JLabel etiqueta1;
    
        public Boton2(){
            setLayout(null);
            boton1=new JButton("Boton 1");
            boton1.setBounds(20,100,90,30);
            add(boton1);
            boton1.addActionListener(this);
    
            boton2=new JButton("Boton 2");
            boton2.setBounds(120,100,90,30);
            add(boton2);
            boton2.addActionListener(this);
    
            boton3=new JButton("Boton 3");
            boton3.setBounds(220,100,90,30);
            add(boton3);
            boton3.addActionListener(this);
    
            etiqueta1=new JLabel("Elige una opción");
            etiqueta1.setBounds(10,10,300,30);
            add(etiqueta1);
        }
    
        // EVENTOS
        public void actionPerformed(ActionEvent evento){
            if(evento.getSource()==boton1){
                etiqueta1.setText("Elegiste el 1");
            }
            if(evento.getSource()==boton2){
                etiqueta1.setText("Elegiste el 2");
            }
            if(evento.getSource()==boton3){
                etiqueta1.setText("Elegiste el 3");
            }
        }
        // Creamos la ventana donde estarán
        public static void main(String args[]){
            Boton2 boton1= new Boton2();
            boton1.setBounds(50,50,350,200);
            boton1.setVisible(true);
            boton1.setResizable(false);
        }
    }
