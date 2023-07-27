#calculator App

import java.util.Scanner;
public class Main {
	public static void main(String[] args) {
		int withdraw; int deposit; int balance =5000 ;
		while(true)
		{
		Scanner sc=new Scanner(System.in);
		System.out.println("select option 1 for withdraw");  
		   System.out.println("select option 2 for deposit");
		System.out.println("select option 3 for balance");
		System.out.println( " select option 4 for exit");
		System.out.println("select an option");
		int s = sc.nextInt(); 
		switch(s)
		{
		
		  case 1 :
		  
		  System.out.println("Please collect your money");
		  withdraw = sc.nextInt();
		  if(balance>=withdraw)
		  {
		  	balance = balance-withdraw ;
		  
		  }
		  
		  else
		  {
		      System.out.println(" insufficient balance");
		  }
		  
		  break;
		  
		  case 2 :
		  
		  System.out.println("Enter money to be deposited" );
		  deposit = sc.nextInt();
		  balance = balance + deposit;
		  System.out.println("Your money has been deposited successfully");
		  break ;
		  
		     case 3 :
		     
		     System.out.println(balance);
		     break;
		     
		     case 4 :
		     System.out.println(" transaction completed successfully");
		     
		     System.exit(0);
		     
		}

	}
	
	}
}
