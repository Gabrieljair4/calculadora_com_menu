# calculadora_com_menu
calculadora com menu
import java.util.*;
public class App {
    public static void main(String[] args) throws Exception {
    // System.out.println("Hello, World!");
    int i,t,a,b,c,r,e,v,senha;    
    // char;
    float x1,x2,delta;
    Scanner leia = new Scanner(System.in);
    
    System.out.println(" bem vindos ao meu programa!!! ");
    
    System.out.println("mas para acessar o programa vc precisa da senha: ");
    senha = leia.nextInt();
    
    if(senha == 123){
        
        System.out.print("senha correta vc pode senguir em frente: ");
        
    }
    else 
    
    while(senha !=123){
        System.out.println("senha incorreta: ");
        System.out.println("digite a senha de novo: ");
    }

    
    System.out.println(" digite oque precisa !!! ");
    System.out.println("digite 1 para calcular a temperatura em f para c: ");
    System.out.println("digite 2 para calucular o imposto: ");
    System.out.print("digite 3 para calcular equaçao do segundo grau: ");
    System.out.println("digite 4 para calcular exponeciaçao: ");
    System.out.println("digite 5 para calcular soma ");
    
    System.out.println("informe um numero: ");
    r = leia.nextInt();
    
    switch (r) {
        case 1:
            System.out.print("informe o valor da temperatura em celcios: ");
            t = leia.nextFloat();
            
            t = 5*((f-31)/9);
            System.out.println("valor da temperatura: " + t);
            
            break;
        case 2:
            System.out.print("infomre o valor do mantante: ");
        
            break;
        case 3:
        
        System.out.print("digite o valor de a: ");
        a = leia.nextInt();
        
        System.out.print("digite o valor de b: ");
        b = leia.nextInt();

        System.out.print("digite o valor de c: ");
        c = leia.nextInt();

        delta = (b*b)-4*a*c;
        
        System.out.print("valor de delta: " + delta);
        
        if(delta >1){
            
            x1 = -b+(Math.pow(delta,1/2))/2*a;   
            x2 = -b-(Math.pow(delta,1/2))/2*a; 
            
            System.out.print("valor de x1: " + x1);
            System.out.print("valor de x2: " + x2);
        }else
        System.out.print("para delta igual a 1 ou negativo ,nao a raizes reais: ");
        //System.out.print("");
            break;        
            case 4:
            
            System.out.print("informe o valor da base: ");
        b = leia.nextInt();
        
        System.out.print("informe o valor do expoente: ");
        e = leia.nextInt();
        
        Math.pow(b,e);
        
        System.out.print("valor da expoenciçao: " + b);
        break;
        
        default:
            break;
            System.out.println("fim do programa: ");
    }
    
    
    
    }
}
