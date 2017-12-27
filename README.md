# Empresa-corier
package empresa_courier;

import java.util.Scanner;

public class Empresa_courier {
    
    public static void Clases_de_camion(){
    
    System.out.println("Camion Grande [1]");
    System.out.println("Camion Pequeño[2]");
    }
    
    public static void tipo_camion(int carga, int volumen){
    int camion=0; 
        
        Scanner entrada = new Scanner (System.in);
        
        if (carga>500 || volumen>1){
            System.out.println("Utilizara un camion grande");
            camion=entrada.nextInt();
           
        }else if(carga<500 || volumen<1){
            System.out.println("Utilizara un camion pequeño");
            
        }
    }
    
    public static void  Rendimiento (int carga, int tipo_camion){
        if (carga==0){
            System.out.println("15km/litro");
        }else if (carga<500)
            System.out.println("20% menor al rendimiento sin carga");
    
    }
    public static void Despacho(int mercancia, int volumen){
    int ciudad=0;
    int aux=3;
            
        for (int i =0;i<aux;i++){
            ciudad++;
            for(int j=0;j<aux;j++){
                for(int k=0;k<aux;k++){
                    
                
                }
            }
        }
    }

    public static void main(String[] args) {
    
    int carga =0;
    int volumen=0;
        
        
        Scanner entrada = new Scanner (System.in);
      
       do{
            System.out.print("Ingrese la carga en kg");
            carga=entrada.nextInt();
            
            if (carga>750) 
                System.out.println("valor ingresado incorrecto");
	
        }while(carga>750);
           
        do{
            System.out.println("Ingrese el volumen en m3");
            volumen=entrada.nextInt();
            
            if (volumen<2)
                System.out.println("Valor incorrecto");
            
        }while (volumen<2);
        
        Clases_de_camion();
        tipo_camion(carga, volumen);
        Rendimiento(carga, volumen);
    }
}
