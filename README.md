# faktoriyel
import java.util.Scanner;
public class Main {
   
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);
        int n,r,result,nf=1,rf=1,differancef=1,differance;
        System.out.println("C(n,r) için n sayısını giriniz: ");
        n=reader.nextInt();
        System.out.println("C(n,r) için r sayısını giriniz: ");
        r=reader.nextInt();
        differance=n-r;
        for(int i=1;i<=n;i++){
            nf *= i;
        }
        for(int i=1;i<=r;i++){
            rf*= i;
        }
        for(int i=1;i<=differance;i++){
            differancef*= i;
        }
        result=nf/(rf*differancef);
        System.out.println(result);
    }
}
