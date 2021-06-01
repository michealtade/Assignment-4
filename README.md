# Assignment-4
Prime Number
//COURSE TITLE:OPERATING SYSTEM &NETWORK SECURITY
//Assignment 4

import java.util.Scanner;

public class Assignment4
{
 public static void main(String args[])
 {		
	int temp;
	boolean isPrime=true;
	Scanner scan= new Scanner(System.in);
	System.out.println("Input any Prime number:");
	//capture the input in an integer
	int num=scan.nextInt();
      scan.close();
	for(int i=2;i<=num/2;i++)
	{
		while(num%i == 0) {
            System.out.println(i+" ");
            num = num/i;
         }
      }
         temp=num%num;
	
	   {
		   if(num >2) {
		         System.out.println(num);
	      isPrime=false;
	     
	
	   }
	
	//If isPrime is true then the number is prime else not
	if(isPrime)
	   System.out.println(num + " is a Prime Number and the factors are:" + num);
	else
	   System.out.println(num + " is a composite factor and the factors are:" + num);
 }
}
}
