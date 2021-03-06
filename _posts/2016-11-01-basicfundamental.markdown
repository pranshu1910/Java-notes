---
layout: post
title:  "Basic Fundamental "
date:   2016-10-01 06:08:02 +0530
---
### Binary Number System - Base-2


 Binary numbers uses only 0 and 1 digits.











### Decimal to Binary
Divide repeatedly by 2, keeping track of the remainders


35710 converts to 1011001012.



### Decimal Numeral System - Base-10
 Decimal numbers uses digits from 0..9.
 These are the regular numbers that we use.

  Eg:
       253810 = 2×103+5×102+3×101+8×100


### Hexadecimal Numeral System - Base-16
 Hex numbers uses digits from 0..9 and A..F.
 H denotes hex prefix.

 Eg:
      2816 = 28H = 2×161+8×160 = 40
      2F16 = 2FH = 2×161+15×160 = 47
      BC1216 = BC12H = 11×163+12×162+1×161+2×160= 48146


### Octal Numeral System - Base-8
 Octal numbers uses digits from 0..7.

  Eg:
278 = 2×81+7×80 = 16+7 = 23
308 = 3×81+0×80 = 24
43078 = 4×83+3×82+0×81+7×80= 2247






Java
============
Java is a programming language expressly designed for use in the distributed environment of the Internet. It was designed to have the "look and feel" of the C++ language, but it is simpler to use than C++ and enforces an object-oriented programming model.




Platform Independent:
> With Java, you can compile source code on Windows and the compiled code (bytecode to be precise) can be executed (interpreted) on any platform running a JVM. So yes you need a JVM but the JVM can run any compiled code, the compiled code is platform independent




How java is Secured ?

> The Bytecode which are generated by the compiler will be tested by the JVM on the execution of the program or we can say every Java Program is under the control of the JVM which checks the code on the runtime many times for viruses and any malicious.



Java Version History

Current stable release of Java is Java SE 8.



High level language vs Low level language

> High level programming languages are languages that uses syntax which close to human languages so, it is easy to understanding the languages. while the low languages programming is languages that close to machine languages such as assembler languages.

Compiler

> A compiler is a software program that transforms high-level source code that is written by a developer in a high-level programming language into a low level object code (binary code) in machine language, which can be understood by the processor. The process of converting high-level programming into machine language is known as compilation.

Linker

> Linker is a computer program that takes one or more object files generated by a compiler and combines them into a single executable file, library file, or another object file.





## JDK Vs JRE Vs JVM


JDK (Java Development Kit) :

JDK = JRE + JVM
JDK contains everything that will be required to develop and run Java application.


## JRE (Java Run time Environment) :

> JRE contains everything required to run Java application which has already been compiled. It doesn’t contain the code library required to develop Java application.


JVM (Java Virtual Machine):

> JVM is a virtual machine which work on top of your operating system to provide a recommended environment for your compiled Java code. JVM only works with bytecode. Hence you need to compile your Java application(.java) so that it can be converted to bytecode format (also known as the .class file).
Which then will be used by JVM to run application. JVM only provide the environment It needs the Java code library to run applications.

{% include image.html url="/images/jdk.png" description="Java Development kit" %}

Eclipse IDE
============
Eclipse is an integrated development environment (IDE) used in computer programming, and is the most widely used Java IDE.
Eclipse is mostly written in java.
#### Creating new project on eclipse
The New Java Project Wizard has two pages. On the first page −
* Enter the Project Name
* Select the Java Runtime Environment (JRE) or leave it at the default
* Select the Project Layout which determines whether there would be a separate folder for the source codes and class files. The recommended option is to create separate folders for sources and class files.

{% include image.html url="/images/eclipseNewProject.PNG" description="eclipse project" %}

You can click on the Finish button to create the project or click on the Next button to change the java build settings.

On the second page you can change the Java Build Settings like setting the Project dependency (if there are multiple projects) and adding additional jar files to the build path.
# Java - Basic Datatypes

Based on the data type of a variable, the operating system allocates memory and decides what can be stored in the reserved memory. Therefore, by assigning different data types to variables, you can store integers, decimals, or characters in these variables. There are two data types available in Java:

### Primitive Data Types
There are eight primitive datatypes supported by Java. Primitive datatypes are predefined by the language and named by a keyword. Let us now look into the eight primitive data types in detail.

#### byte
>Byte data type is an 8-bit signed two's complement integer
* Minimum value is -128 (-2^7)
* Maximum value is 127 (inclusive)(2^7 -1)
* Default value is 0
Byte data type is used to save space in large arrays, mainly in place of integers, since a byte is four times smaller than an integer.<br/>
Example: byte a = 100, byte b = -50

#### short
> Short data type is a 16-bit signed two's complement integer
* Minimum value is -32,768 (-2^15)
* Maximum value is 32,767 (inclusive) (2^15 -1)
* Short data type can also be used to save memory as byte data type. A short is 2 times smaller than an integer
* Default value is 0. <br/>
Example: short s = 10000, short r = -20000

#### int
> Integer is generally used as the default data type for integral values unless there is a concern about memory.
* Int data type is a 32-bit signed two's complement integer.
* Minimum value is - 2,147,483,648 (-2^31)
* Maximum value is 2,147,483,647(inclusive) (2^31 -1)
* The default value is 0. <br/>
Example: int a = 100000, int b = -200000

#### long
>Long data type is a 64-bit signed two's complement integer
* Minimum value is -9,223,372,036,854,775,808(-2^63)
* Maximum value is 9,223,372,036,854,775,807 (inclusive)(2^63 -1)
* This type is used when a wider range than int is needed
* Default value is 0L. <br/>
Example: long a = 100000L, long b = -200000L

#### float
> Float data type is a single-precision 32-bit IEEE 754 floating point
* Float is mainly used to save memory in large arrays of floating point numbers
* Default value is 0.0f
* Float data type is never used for precise values such as currency <br/>
Example: float f1 = 234.5f

#### double
> double data type is a double-precision 64-bit IEEE 754 floating point
* This data type is generally used as the default data type for decimal values, generally the default choice
* Double data type should never be used for precise values such as currency
* Default value is 0.0d <br/>
Example: double d1 = 123.4

#### boolean
> boolean data type represents one bit of information
* There are only two possible values: true and false
* This data type is used for simple flags that track true/false conditions
* Default value is false <br/>
Example: boolean one = true

#### char
> char data type is a single 16-bit Unicode character
* Minimum value is '\u0000' (or 0)
* Maximum value is '\uffff' (or 65,535 inclusive)
* Char data type is used to store any character <br/>
Example: char letterA = 'A'

{% include image.html url="/images/primitivetype1.png" description="Primitive Datatypes" %}

{% include image.html url="/images/primitivetype2.png" description="Primitive Datatypes" %}
### Reference/Object Data Types
Reference variables are created using defined constructors of the classes. They are used to access objects. These variables are declared to be of a specific type that cannot be changed. For example, Employee, Puppy, etc.

* Class objects and various type of array variables come under reference datatype.

* Default value of any reference variable is null.

* A reference variable can be used to refer any object of the declared type or any compatible type.

Example: Animal animal = new Animal("giraffe");

>Note: Non primitive data type will be studied later.

#### Integer and Float Conversions  
An arithmetic operation between an integer and integer always yields an integer result.
An operation between a float and float always yields a float result.
An operation between an integer and float always yields a float result. In this operation the integer is first promoted to a float and then the operation is performed. Hence the result is float.

### Writing on console:
System.out.print(): is used to print message to console window.
 E.g:
 ```java
    System.out.print("Hello World");
    System.out.print("My name is" + foo);
    System.out.print("Sum of " + a + "and " + b + "is " + c);
    System.out.print("Total USD is " + usd);
```
a, b, c, usd, foo  are variables of some datatype

# Scanner

There are various ways to read input from the keyboard, the java.util.Scanner class is one of them. The Java Scanner class breaks the input into tokens using a delimiter that is whitespace by default. It provides many methods to read values of various types.

~~~java
Scanner sc = new Scanner(System.in);

System.out.print("Enter Integer value: ");
int x = sc.nextInt();

System.out.print("Enter Float value: ");
float k = sc.nextFloat();

System.out.print("Enter Double value: ");
double y = sc.nextDouble();

System.out.print("Enter String value: ");
String z = sc.next();

System.out.print("Reading Character input : ");
char c = reader.next().charAt(0);

sc.close();//Closes this scanner.
~~~
#### Note
>	Java doesn't have unsigned primitives.
The value 127 is actually represented by '01111111' the first bit being the sign (0 is positive).
An unsigned byte would be able to hold values 0 to 255, but 127 is the maximum for a signed byte. Since a byte has 8 bits, and the signed one consumes one to hold the sign. So if you want to represent values larger than 127 you need to use a bigger type that has a greater number of bits. The greater type also has a reserved bit for sign, but it has at least 8 bits used for the actual values, so you can represent the value 255.

# next() vs nextLine():
> next() can read the input only till the space. It can't read two words separated by space. Also, next() places the cursor in the same line after reading the input.
nextLine() reads input including space between the words (that is, it reads till the end of line \n). Once the input is read, nextLine() positions the cursor in the next line.


## Decision Making
Decision making structures have one or more conditions to be evaluated or tested by the program, along with a statement or statements that are to be executed if the condition is determined to be true, and optionally, other statements to be executed if the condition is determined to be false.
#### if Statement:
The Java if statement tests the condition. It executes the if block if condition is true.
```Java
Syntax:
if(condition){  
//code to be executed  
}
```
#### if-else statement:
The Java if-else statement also tests the condition. It executes the if block if condition is true otherwise else block is executed.
```Java
Syntax:
if(condition){  
//code if condition is true  
}else{  
//code if condition is false  
}  
```
#### else-if ladder statement:
The nested if...else statement allows you to check for multiple test expressions and execute different codes for more than two conditions.
```java
Syntax:
if (testExpression1){
   // statements to be executed if testExpression1 is true
}else if(testExpression2{
   // statements to be executed if testExpression1 is false and testExpression2 is true
}else if (testExpression3){
   // statements to be executed if testExpression1 and testExpression2 is false and testExpression3 is true
}
.
.
else{
   // statements to be executed if all test expressions are false
}
```
#### switch statement:
A switch statement allows a variable to be tested for equality against a list of values. Each value is called a case, and the variable being switched on is checked for each case.
```java
Syntax:
switch(expression) {
   case value :
      // Statements
      break; // optional
   case value :
      // Statements
      break; // optional
   // You can have any number of case statements.
   default : // Optional
      // Statements
}
```
## Loop Control
#### while loop:
The Java while loop is used to iterate a part of the program several times. If the number of iteration is not fixed, it is recommended to use while loop.
```java
Syntax:
while(condition){  
//code to be executed  
}
```
~~~java
public class Test {

   public static void main(String args[]) {
      int x = 10;

      while( x < 20 ) {
         System.out.print("value of x : " + x );
         x++;
         System.out.print("\n");
      }
   }
}
value of x : 10
value of x : 11
value of x : 12
value of x : 13
value of x : 14
value of x : 15
value of x : 16
value of x : 17
value of x : 18
value of x : 19
~~~
#### do while loop
E.g:
~~~java
public class Test {

   public static void main(String args[]){
      int x = 10;

      do{
         System.out.print("value of x : " + x );
         x++;
         System.out.print("\n");
      }while( x < 20 );
   }
}
value of x : 10
value of x : 11
value of x : 12
value of x : 13
value of x : 14
value of x : 15
value of x : 16
value of x : 17
value of x : 18
value of x : 19
~~~
#### for loop:
E.g.
~~~java
public class Test {

   public static void main(String args[]) {

      for(int x = 10; x < 20; x = x+1) {
         System.out.print("value of x : " + x );
         System.out.print("\n");
      }
   }
}
value of x : 10
value of x : 11
value of x : 12
value of x : 13
value of x : 14
value of x : 15
value of x : 16
value of x : 17
value of x : 18
value of x : 19
~~~
## Branching Statements
#### break
The break statement has two forms: labeled and unlabeled. You saw the unlabeled form in the previous discussion of the switch statement. You can also use an unlabeled break to terminate a for, while, or do-while loop [...]

An unlabeled break statement terminates the innermost switch, for, while, or do-while statement, but a labeled break terminates an outer statement.
#### continue
The continue statement skips the current iteration of a for, while , or do-while loop. The unlabeled form skips to the end of the innermost loop's body and evaluates the boolean expression that controls the loop. [...]

A labeled continue statement skips the current iteration of an outer loop marked with the given label.
```java
System.out.println("Break Statement\n....................");

        for(int i=1;i<=5;i++)
        {
            if(i==4) break;
            System.out.print(i+" ");
        }

System.out.println("Continue Statement\n....................");

        for(int i=1;i<=5;i++)
        {
            if(i==1) continue;
            System.out.print(i+" ");
        }

output:
Break Statement
1 2 3
Continue Statement
2 3 4 5
```        
