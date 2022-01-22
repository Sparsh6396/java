//java
//user defined array : in which user can input values and size of array..
//also find maximum amd minimum number.
import java.util.*;
public class Array1{
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number which you want to size of array");
        int n=sc.nextInt();
        int a[]=new int[n+1];
        for (int i=0;i<n+1;i++){
            System.out.println("Enter the value of"+i+""+"number "+":-");
            a[i]=sc.nextInt();
            

        }
        int smallest=a[0];
        int largest=a[0];
        for(int i=0;i<n+1;i++)
        if(a[i]>largest)
        largest=a[i];
        else if(a[i]<smallest)
        smallest=a[i];

        System.out.println("your largest no.is in array is:-"+""+largest );
        System.out.println("your smallest no.is in array is:-"+""+smallest );


    }
}
