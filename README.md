# Java

1)WHO WILL TRANSLATE SYSTEM TO MACHINE LEVEL?
  -COMPILER + INTERPRETER.

2)HELLO.JAVA ----COMPILIER-->HELLO.CLASS(BYTE  code which is neither machine or understandable code)-- Machine-- interpreter intepretes line by   line in the machine.



3)public class HelloWorld{

public static void main(String[] args) {
   System.out.println("Hello World!!!");
}
}
akhilpagadapoola@Akhils-MacBook-Air Documents % ls
HelloWorld.java			aws
Hibernate error doc.txt		git.txt
Hibernate new error doc.txt	ias.txt
Pay Slips
akhilpagadapoola@Akhils-MacBook-Air Documents % javac HelloWorld.java
akhilpagadapoola@Akhils-MacBook-Air Documents % java HelloWorld
Hello World!!!


4) JDK- JAVA DEVELOPMENT KIT- JDK is combinatioon of JRE and Dev tools-java compilier, java debugger, java doc
5) JRE- JAVA RUNTIME ENVIRONMENT- JRE is combination of JVM + Runtime libraries
6) JVM- JAVA VIRTUAL MACHINE

                 (jdk --compiler)                         JVM+JRE
7)HelloWorld.java----------->HelloWorld.class (bytecode)------------> INPUT TO JVM---->CLASSLOADER---METHOD AREA,HEAP AREA,Stack Memory,Program Counter------------>(Execution Engine)--->interpreter(reads code line by line--> JIT (Just in time compiler) IF repeated methods it quickly compile-- Garbage collector----JNI(Java Native interface).

METHOD AREA - contains class data
HEAP AREA-- contains objects
STACK MEMORY- Local variables are stores in stack memory
Program Counter- cuurent execution next execution status
Native Method- We can run other programing langagues 


InterviewQuestion Note:
=========================
1.You can compile a java code without a main method.
2.You cannot run a java code without a main method.


package com; //optional

import ...;// on demand

class HelloWorld {
//var
//methods: set of instructions
//constructor
//blocks

}



public static void main(String args []){
}

public- Access specifier
static- keyword
void- return type
main- method name
String args[] - Array of string type


Identifiers:
==============
package com.flm.identifiersdemo;

public class IdentifiersDemo {

	public static void main(String[] args) {
		
		int x=10;
		
		int a2=250;
		System.out.println(a2);
	}
}

Datatypes:
============

package com.flm.identifiersdemo;

public class DataTypesDemo {

	public static void main(String[] args) {
		
		//integral data types
		byte b =127;
		short s =12999;
		int i =1299999999; //preferred
		long l=899999999; 
		
		//decimal values
		float f=12.3888888888888888888888888f;
		double d =123.458687677777777777777777777;//preferred
		
		//boolean
		
		boolean k =true;
		boolean k2=false;
		
		
		//char
		char c='A';
		char c1=65;
		
		
		
		System.out.println("Byte value is "+b);
		System.out.println("Short value is "+s);
		System.out.println("int  value is "+i);
		System.out.println("long value is "+l);
		System.out.println("float value is "+f);
		System.out.println("double value is "+d);
		
		System.out.println("boolean value is "+k);
		System.out.println("boolean value is "+k2);
		
		System.out.println("character value is "+c+c1);
	}
	
}

Scanner
=========

package com.flm.identifiersdemo;

import java.util.Scanner;

public class ScannerDemo {

	public static void main(String[] args) {
		
		
		   Scanner so = new Scanner(System.in);
	        System.out.println("Please enter byte value");
	        byte b = so.nextByte();

	        System.out.println("Please enter short value");
	        short s = so.nextShort();

	        System.out.println("Please enter int value");
	        int i = so.nextInt();

	        System.out.println("Please enter long value");
	        long l = so.nextLong();

	        System.out.println("Please enter double value");
	        double d = so.nextDouble();

	        System.out.println("Please enter float value");
	        float f = so.nextFloat();

	        System.out.println("Please enter boolean value");
	        boolean bool = so.nextBoolean();
	        
	        // Consume the newline character
	        so.nextLine();

	        System.out.println("Please enter char value");
	        char c = so.nextLine().charAt(0);

	        System.out.println("Please enter string value");
	        String str = so.nextLine();

	        System.out.println("Byte value is " + b);
	        System.out.println("Short value is " + s);
	        System.out.println("Int value is " + i);
	        System.out.println("Long value is " + l);
	        System.out.println("Float value is " + f);
	        System.out.println("Boolean value is " + bool);

	        System.out.println("Char value is " + c);
	        System.out.println("String value is " + str);

	        scannerFunction();
	}

	private static void scannerFunction() {
		//Java is a object oriented language OOP
		
		Scanner s = new Scanner(System.in);
		
		System.out.println("Welcome to MIT Solutions");
	    System.out.println("Please enter a value");
        int a =s.nextInt();
        System.out.println("Please enter b value");
        int b = s.nextInt();
        
        int result = a+ b;
        System.out.println(result);
		
		helloWorld();
	}

	private static void helloWorld() {
		System.out.println("Hello World");
	}
}





LOGICAL OPERATORS
====================

package com.flm.identifiersdemo;

import java.util.Scanner;
public class OperatorsDemo {

	public static void main(String[] args) {
		
	
		boolean b1=false;
		boolean b2=true;
		
		System.out.println(b1 || b2); //true
		System.out.println(!b1); //true
		System.out.println((b1 && b2) || (b2 || b1));//true
 	
	}
PredIncrement and PostIncrement:
=====================================
	private static void preIncrementAndPostIncrement() {
		// pre increment and post increment 
		
		int a=10;
		
		System.out.println(++a);//11
		System.out.println(a++);//11
		System.out.println(a);//12
		System.out.println(--a);//11
		System.out.println(a--);//11
		System.out.println(a);//10
	}

Swapping of Two Numbers:
===========================
	private static void swappingOfTwoNumbers() {
		Scanner s = new Scanner(System.in);
		
//		int a=10;
//		int b=20;
//		
//		a+=b; //a=a+b
//		a-=b; //a=a-b
//		System.out.println("Res "+a);
		
		//swapping of two variables first logic
//	int a=10;
//	int b=20;
//	int c=a;
//	a=b;
//	b=c;
//	System.out.println(a);
//	System.out.println(b);
	
	// second logic for swapping of two variables first logic
		int a=10;
		int b=20;
	
     a=a+b;
     b=a-b;
     a=a-b;
     
 	System.out.println(a);
 	System.out.println(b);
	}

Arthimetic Operators:
======================

	private static void arthOperators() {
		Scanner sc = new Scanner(System.in);
		//+ - * / %
		
		System.out.println("Enter your first no: ");
		int a=sc.nextInt();
		System.out.println("Enter your second no: ");
		int b=sc.nextInt();
		
		int sum = a+b;
		
		System.out.println("Sum of two numbers "+sum);
		System.out.println("Sub of two number "+(a-b));
		System.out.println("mul of two numbers "+ (a*b));
		System.out.println("div of two numbers "+(a/b));
	}
}


Relation Operators:
======================

package com.flm.identifiersdemo;

import java.util.Scanner;
public class OperatorsDemo {

	public static void main(String[] args) {
		
	
		relationOperators();
			
		
 	
	}

	private static void relationOperators() {
		int a=10;
		int b=20;
		
		boolean r1 = !(a==b);// true
		System.out.println(r1);
				
		boolean r2 = (a!=b);//true
		System.out.println(r2);
		
		boolean r3 = (a>b);//false
		System.out.println(r3);
		
		boolean r4 = (a<b);//true
		System.out.println(r4);
		
		boolean r5 = (a>=b);//false
		System.out.println(r5);
		
		boolean r6 = (a<=b);//true
		System.out.println(r6);
	}


Terinary Operators:
====================


package com.flm.identifiersdemo;

import java.util.Scanner;
public class OperatorsDemo {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Enter your first no : ");
		int a = sc.nextInt();
		
		System.out.println("Enter your second no : ");
		int b = sc.nextInt();
		
		System.out.println("Enter your third no : ");
		int c = sc.nextInt();
		
//		int a=100;
//		int b=20;
		
	   int highestNumber = (a>b)? ((a>c)? a:c):((b>c)? b:c);
	   
//	   int highestNumber = (a>b) && (a>c)? a: (b>c)? b:c;
	   
	   System.out.println("highestNumber "+ highestNumber);
	   
		
 	
	}
