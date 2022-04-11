# -genin-evresini-ve-alan-n-hesaplama
Java 101_3 Kenar uzunlukları alınan üçgenin çevresini ve alanını hesaplayan program

/* Ödev -Patika.dev
Üç kenar uzunluğunu kullanıcıdan aldığınız üçgenin alanını hesaplayan programı yazınız. */

import java.util.Scanner ;

public class Main {
    public static void main (String[] args) {
        int a, b, c ;
        double alan, u ;
    
        Scanner kenar=new Scanner(System.in);
        System.out.print("a kenarının uzunluğunu giriniz : ");
        a=kenar.nextInt();
        System.out.print("b kenarının uzunluğunu giriniz : ");
        b=kenar.nextInt();
        System.out.print("c kenarının uzunluğunu giriniz : ");
        c=kenar.nextInt();
        
        u=(a+b+c)/2 ;
        System.out.println("Üçgenin çevresi :"+ (2*u));
        alan=Math.sqrt(u*(u-a)*(u-b)*(u-c));
        System.out.print("Üçgenin alanı :"+ alan);
        
    }    
    
    
}
