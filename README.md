# josebarrera
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package josebarrera1;

import javax.swing.JOptionPane;

/**
 *
 * @author willi
 */
public class Josebarrera1 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
   
        int opcion=0;
        String nombre="";
        String direccion="";
        double edad=0;
        double sueldo=0;
        double descuento=0;
        double prestamo=0;
        double total;
        int x =0,y = 0,z = 0,m = 0,n = 0,p = 0;
        double r;
        
        
        do{
           opcion=Byte.parseByte(JOptionPane.showInputDialog(
                   "MENU PRINCIPAL\n"
            + "1. Programa de Serie\n"
            + "2. Programa de Sueldo Liquido\n"
            + "3. Salir\n"
            + "ELIJA SU OPCION"));
            switch(opcion){
                case 1:
                    for ( x = 1; x < 100; x ++ ){
                    y = (x + 2);
                    z = (y * 2);
                    n = (z + 2);
                    m = (n + 2);
                    p = (m * 2);       
                };
                 r = Double.parseDouble(JOptionPane.showInputDialog(null, x +"-"+ x + "-" + y + "-" + z + "-" + n + "-" + n + "-" + m + "-" + p));
                    break;
                case 2:
                    nombre = JOptionPane.showInputDialog(null, "Ingrese Nombre");
                    direccion = JOptionPane.showInputDialog(null, "Ingrese Direción");
                    edad = Double.parseDouble(JOptionPane.showInputDialog(null, "Ingrese Edad"));
                    sueldo = Double.parseDouble(JOptionPane.showInputDialog(null, "Ingrese Sueldo"));
                    descuento = sueldo*0.10;
                    prestamo = sueldo*0.02;
                    total = sueldo -(descuento + prestamo);
                    JOptionPane.showInputDialog(null, "Nombre del Empleado: "+nombre+"\n"+"Dirección del Empleado: "+direccion+"\n"+"Edad del Empleado:  "+edad+"\n"
                                                +"Su Sueldo Total: $"+total);
                    
                    break;
                case 3:
                    opcion=3;
                    break;
                default:
                    JOptionPane.showMessageDialog(null, "salir");
            }
        }
        while(opcion!=3);
        System.exit(0);
        
    }
    
}
