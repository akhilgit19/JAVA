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
7)HelloWorld.java----------->HelloWorld.class (bytecode)------------> JVM Input which reads code line by line and converst to machine understandable


INPUT TO JVM---->CLASSLOADER---METHOD AREA,HEAP AREA,Stack Memory,Program Counter

METHOD AREA - contains class data
HEAP AREA-- contains objects
STACK MEMORY- Local variables are stores in stack memory
Program Counter- cuurent execution next execution status
Native Method- 
