# NetBeans_Java_
//Para crear un nuevo proyecto va hasta File>New Project>Debe estar seleccionado es Categories:Java, y en Projects:Java Application,>Next>Pone el nombre del archivo, luego>Finish
package prueba;
import java.util.Scanner;//Esta biblioteca es necesaria para poder solicitar un dato al usuario
public class Prueba {

    
    public static void main(String[] args)//Como no van a usar aún la programación orientada a objetos, todo lo escribe en el main
    {
        int a=1;
        double b=Math.pow(4,2);//Math.pow es para hacer una potencia, en este caso 4,2
        double c=3.4;
        int d=0;
        //-----Tabla de multiplicar
        Scanner cualquierNombre=new Scanner(System.in);//Esta línea es para poder pedir los datos al usuario
        System.out.println("Ingrese el número del que desea obtener la tabla");//Esto equivale al cout en c
        d=cualquierNombre.nextInt();//Al igual que en ruby, debe especificar entero, string, double, con la diferencia de que en java, no puede hacer la conversión directamente; nextInt() es para recibir un entero, para recibir un double, es nextDouble, y un string, es nextLine();
        
        while (a<=10)
        {   
            System.out.println(d+"x"+a+"="+d*a);//En c sería cout<<d<<"x"<<a<<"="<<d*a<<endl;
            a++;//Esto equivale a (a=a+1;)
        }
        //Para ejecutar, en el panel izquierdo sale su proyecto, lo extiende, luego extiende la carpeta Source Packages, da click derecho sobre el proyecto, y da click en Run File.
    }
    
}
