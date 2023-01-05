//# count-of-positive-or-negative
//Write a program to enter the number till the user wants and at the end it should display the count of positive, negative and zero entered.
import java.util.*;
class countpnz{
    public static void main(String[] args){
        Scanner sc= new Scanner(System.in);
        int p=0;
        int m=0;
        int z=0;
        char u;
        do{
            System.out.print("Enter a number:");
            int n=sc.nextInt();
        if(n>1){
            p++;
        }
        else if(n<0){
            m++;
        }
        else if(n==0){
            z++;
        }
        else {
            System.out.println("word dosn't exist");
        }
        System.out.println("if you want to continue type 'c' or don't type'n':");
        u=sc.next().charAt(0);
    }while(u=='c'||u=='C');
        System.out.println("The Total positive numbers you entered:"+p);
        System.out.println("The Total negitive numbers you entered:"+m);
        System.out.println("The Total zeros you entered:"+z);
    }
}
