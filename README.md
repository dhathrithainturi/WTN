1) Student demo using class and object:

import java.io.*;
import java.util.*;
public class StudentDemo {
	int id =30609;
	String name="kavya";
	public static void main(String args[]){  
		 StudentDemo s1=new StudentDemo();
		 System.out.println(s1.id);
		  System.out.println(s1.name);  
	}

}



2)sum of two numbers using method:

import java.io.*;
import java.util.*;
public class Sum {
	public static void main(String[] args) {          
	      int a = 30000;  
	        int b = 30609;  
	        System.out.println("The sum of a and b is = " + Integer.sum(a, b));  

}
}




3)print employee information using setters and getters method:

import java.io.*;
import java.util.*;
class EmpSetGet
{

private int empId;
	   private String name;
	   private int age;
	   private String dept;

	   public int getEmpId()
	   {
	      return empId;
	   }
	   public String getName()
	   {
	      return name;
	   }
	   public int getAge()
	   {
	      return age;
	   }
	   public String getDept()
	   {
	       return dept;
	   }
	   public void setEmpId( int empId)
	   {
	      this.empId = empId;
	   }
	   public void setName(String name)
	   {
	      this.name = name;
	   }
	   public void setAge( int age)
	   {
	      this.age = age;
	   }
	   public void setDept(String dept)
	   {
	       this.dept = dept;
	   }
	}
public class Emp {
	  public static void main(String args[])
	    {
	      EmpSetGet emp = new EmpSetGet();
	      emp.setEmpId(30609);
	      emp.setName("kavya");
	      emp.setAge(20);
	      emp.setDept("Development");
	      System.out.println("Employee Id : "+emp.getEmpId() + "\nName : " + emp.getName() + "\nAge : " + emp.getAge() + "\nDepartment : "+emp.getDept());
	   }
	
}

#4th program

package com.w3epic.wiprotraining;

public class Assignment4 {

	public static void main(String[] args) {
		char x = 'a';
		char y = 'e';
		
		if (x < y) {
			System.out.println(x + ", " + y);
		} else {
			System.out.println(y + ", " + x);
		}

	}

}

#5th program

package com.w3epic.wiprotraining;

public class Assignment5 {

	public static void main(String[] args) {
		char ch = '*';
		
		//for (int i = 0; i < 128; i++) System.out.printf("%d: %c \n", i, i);
		
		if ((ch >= 65 && ch <= 90) || (ch >= 97 && ch <= 122)) {
			System.out.println("Alphabet");
		} else if (ch >= 48 && ch <= 57) {
			System.out.println("Digit");
		} else {
			System.out.println("Special Character");
		}

	}

}

#6th program

package com.w3epic.wiprotraining;

public class Assignment6 {

	public static void main(String[] args) {
		String gender = args[0];
		int age = Integer.parseInt(args[1]);
		
		if (!gender.equals("Male") && !gender.equals("Female"))
			System.out.println("Invalid gender");
				
		if (age < 1 || age >= 120)
			System.out.println("Invalid age");
		
		
		if (gender.equals("Female") && (age >= 1 && age <= 58)) {
			System.out.println("Interest == 8.2%");
		} else if (gender.equals("Female") && (age >= 59 && age <= 120)) {
			System.out.println("Interest == 7.6%");
		} else if (gender.equals("Male") && (age >= 1 && age <= 60)) {
			System.out.println("Interest == 9.2%");
		} else if (gender.equals("Male") && (age >= 61 && age <= 120)) {
			System.out.println("Interest == 8.3%");
		}
		
	}

}


#7th program

package com.w3epic.wiprotraining;

public class Assignment7 {

	public static void main(String[] args) {
		char ch = 'a';
		
		if (Character.isLowerCase(ch)) 
			System.out.println(ch + "->" + Character.toUpperCase(ch));
		else
			System.out.println(ch + "->" + Character.toLowerCase(ch));

	}


#8th program

package com.w3epic.wiprotraining;

public class Assignment8 {

	public static void main(String[] args) {
		char colorCode = 'Q';
		
		switch (colorCode) {
		case 'R':
			System.out.println("R->Red");
			break;
		case 'G':
			System.out.println("G->Green");
			break;
		case 'B':
			System.out.println("B->Blue");
			break;
		case 'O':
			System.out.println("O->Orange");
			break;
		case 'Y':
			System.out.println("Y->Yellow");
			break;
		case 'W':
			System.out.println("W->White");
			break;
		default:
			System.out.println("Invalid Code");
		}

	}

}

#9th program

package com.w3epic.wiprotraining;

import java.time.Month;

public class Assignment9 {

	public static void main(String[] args) {
		if (args.length == 0) {
			System.out.println("Please enter the month in numbers");
			System.exit(0);
		}
		
		int month = Integer.parseInt(args[0]);
				
			
		if (month < 1 || month > 12) {
			System.out.println("Invalid month");
			System.exit(0);
		}
		
		// toUpperCaseFirst
		String monthStr = Month.of(month).name();
		monthStr = monthStr.substring(0,1).toUpperCase() + monthStr.substring(1).toLowerCase();
		
		System.out.println(monthStr);

	}
	

}

#10th program

package com.w3epic.wiprotraining;

public class Assignment10 {

	public static void main(String[] args) {
		for (int i = 1; i <= 10; i++) {
			System.out.print(i + "\t");
		}

	}

}

#11th program

package com.w3epic.wiprotraining;

public class Assignment11 {

	public static void main(String[] args) {
		for (int i = 23; i <= 57; i++) {
			if (i % 2 == 0)
				System.out.println(i);
		}

	}

}

#12th program

package com.w3epic.wiprotraining;

public class Assignment12 {

	public static void main(String[] args) {
		int no = -4;
		
		if (no < 0) no *= -1;
		
		Boolean isPrime = true;
		
		for (int i = 2; i < no/2+1; i++) {
			if (no % i == 0) {
				isPrime = false;
				break;
			}
		}
		
		if (no == 0 || no == 1) isPrime = false;
		
		if (isPrime) System.out.println("prime");
		else System.out.println("not prime");
	}

}

#13th program

package com.w3epic.wiprotraining;

public class Assignment13 {

	public static void main(String[] args) {
		for (int i = 10; i <= 99; i++) {
			if (isPrime(i)) System.out.println(i);
		}

	}
	
	public static boolean isPrime(int no) {
		if (no < 0) no *= -1;
		
		Boolean isPrime = true;
		
		for (int i = 2; i < no/2+1; i++) {
			if (no % i == 0) {
				isPrime = false;
				break;
			}
		}
		
		if (no == 0 || no == 1) isPrime = false;
		
		return isPrime;
	}

}

#14th program

package com.w3epic.wiprotraining;

public class Assignment14 {

	public static void main(String[] args) {
		if (args.length == 0) {
			System.out.println("Please enter an integer number");
			System.exit(0);
		}

		int number = Integer.parseInt(args[0]);
		
		if (number == 0 || number == 1) {
			System.out.println(number + " is neither prime nor composite");
		} else {
			if (isPrime(number))
				System.out.println(number + " is a prime number");
			else
				System.out.println(number + " is not a prime number");
		}
		
	}
	
	public static boolean isPrime(int no) {
		if (no < 0) no *= -1;
		
		Boolean isPrime = true;
		
		for (int i = 2; i < no/2+1; i++) {
			if (no % i == 0) {
				isPrime = false;
				break;
			}
		}
		
		if (no == 0 || no == 1) isPrime = false;
		
		return isPrime;
	}

}

#15th program

package com.w3epic.wiprotraining;

public class Assignment15 {

	public static void main(String[] args) {
		int number = 1234;
		int sum = 0;
		
		while (number != 0) {
			sum += number % 10;
			number /= 10;
		}
		
		System.out.println(sum);

	}

}

#16th program

package com.w3epic.wiprotraining;

public class Assignment16 {

	public static void main(String[] args) {
		if (args.length == 0) {
			System.out.println("Please enter an integer number");
			System.exit(0);
		}
		
		int rowCount = Integer.parseInt(args[0]);
		
		for (int i = 0; i < rowCount; i++) {
			for (int j = 0; j <= i; j++) {
				System.out.print("*");
			}
			System.out.println();
		}

	}

}

#17th program

package com.w3epic.wiprotraining;

import java.util.Scanner;

public class Assignment17 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		int ip = sc.nextInt(); // 1234
		int op = 0; // 4321
		int i = (int) Math.pow(10, String.valueOf(ip).length() - 1);
		
		while (ip != 0) {
			int digit = ip % 10;
			op += digit * i;
			i /= 10;
			ip /= 10;
		}
		
		System.out.println(op);
		
		sc.close();
	}

}

#18th program

package com.w3epic.wiprotraining;

public class Assignment18 {

	public static void main(String[] args) {
		int number = Integer.parseInt(args[0]);
		
		if (getPalindromeNumber(number) == 2)
			System.out.println(number + " is a palindrome");
		else
			System.out.println(number + "is not a palindrome");
	}
	
	public static int getPalindromeNumber (int input1) {
		String numberStr = String.valueOf(input1);
		int digitCount = numberStr.length();
		boolean isPalindrome = true;
		
		int range = digitCount / 2;
		if (digitCount % 2 == 0) range--;
		
		for (int i = 0; i <= range; i++) {
			if (numberStr.charAt(i) != numberStr.charAt(digitCount - i - 1)) isPalindrome = false;
		}
		
		if (isPalindrome == true) return 2;
		else return 1;
	}

}

#19th program

package com.w3epic.wiprotraining;

public class Assignment19 {

	public static void main(String[] args) {
		
		int counter = 0;
		int i = 0;
		
		while (counter != 5) {
			i++;
			
			if (i % 2 == 0 && i % 3 == 0 && i % 5 == 0) {
				System.out.println(i);
				counter++;
			}
		}
	}

}

#20th program

package com.w3epic.wiprotraining;

import java.util.Scanner;

public class Assignment20 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		System.out.println("1. Add\n2. Sub");
		int choice = sc.nextInt();
		
		int operand1;
		int operand2;
		int result;
		
		if (choice == 1) {
			System.out.println("Enter first operand: ");
			operand1 = sc.nextInt();
			System.out.println("Enter second operand: ");
			operand2 = sc.nextInt();
			result = operand1 + operand2;
		} else {
			System.out.println("Enter first operand: ");
			operand1 = sc.nextInt();
			System.out.println("Enter second operand: ");
			operand2 = sc.nextInt();
			result = operand1 - operand2;
		}
		
		System.out.println("Result: " + result);
		
		System.out.println("Do you want to continue? Y or N");
		
		sc.nextLine();		
		choice = sc.nextLine().charAt(0);
		
		if (choice == 'Y' || choice == 'y') main(args);
		
		sc.close();
	}

}
