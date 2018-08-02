//Revise the program to randomly generate an addition question with two integers less than 100.

# Extra_Ex3_10

package com.personal.Ex3_10;



	import java.util.Scanner; 

	public class EX_10  {
	  public static void main(String[] args) {
	    int number1 = (int)(Math.random() * 10);
	    int number2 = (int)(Math.random() * 10);

	    if (number1 < number2) {
	      int temp = number1;
	      number1 = number2;
	      number2 = temp;
	    }

	    System.out.print
	      ("What is " + number1 + " - " + number2 + "? ");
	    Scanner input = new Scanner(System.in);
	    int answer = input.nextInt();

	    if (number1 - number2 == answer)
	      System.out.println("You are correct!");
	    else
	      System.out.println("Your answer is wrong.\n" + number1 + " - "
	        + number2 + " should be " + (number1 - number2)); 
	  }
	}

