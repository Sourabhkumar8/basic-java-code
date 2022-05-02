# basic-java-code
table of any number ,  fibonacci series ,factorial of a number, checking prime
import java.util.Scanner;
 public class Basic{
       public static void main(String args[]){
             System.out.println("welcome to java basic code for begginer");
             System.out.println("enter 1 for print table , 2  for factorial , 3 for prime number, 4 for fibonacci series ");
             Scanner sc = new Scanner(System.in);
             int m =sc.nextInt();
             switch(m){
                   case 1:
                   int n,t;
                   System.out.println("enter number you want table for ");
                   Scanner s = new Scanner(System.in);
                   n = s.nextInt();
                   int i=1;
                   while(i<=10){ 
                         t=i*n;                                                                            //sourabh
                         System.out.println(t);
                         i+=1;
                   }
                   break;
                   case 2:
                   int num,fact=1,j=1;
                   System.out.println("enter the number you want factorial for");                           //sourabh
                   num=sc.nextInt();
                   while(j<=num){
                         fact=fact*j;
                     j+=1;
                   }System.out.println(fact);
                   break;
                   case 3:
                   int var;
                   int k=2;
                   int flag =0;
                   System.out.println("entered the number you want to check prime or not");
                   var=sc.nextInt();
                   while(k<=var-1){
                        if(var%k==0){
                               flag+=1;
                         }
                         
                             k+=1;
                   }
                   if(flag==0){
                   System.out.println(" prime");
                   }
                   else{
                         System.out.println(" not  prime");
                   }
                   break;
                   case 4:
                   int n1=0,n2=1,n3,v;
                   Scanner d= new Scanner(System.in);
                   System.out.println("enter the number till you want fibbonecci series");
                   
                   int coun=d.nextInt();
                   System.out.println(n1);
                   System.out.println(n2);
                   for(v=2;v<coun;v++)
                   {
                         n3=n1+n2;
                         System.out.println(""+n3);
                         n1=n2;
                         n2=n3;
                   }                                                                                // sourabh
                   break;
                      
                   default:
                   System.out.println("you have entered wrong value");
             }
       }
 }
