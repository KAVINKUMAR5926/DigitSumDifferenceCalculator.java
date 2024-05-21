# DigitSumDifferenceCalculator.java
import java.util.Scanner;
public class Main
{
    public static void main(String arg[]){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int esum=0, osum=0, rem;
        while(n>0){
           rem = n%10;
           if(rem%2==0){
                esum += rem;
        }
        else{
           osum += rem; 
        }
        n/=10;
       }
       System.out.print((esum>osum)?esum-osum:osum-esum);
    }
}
