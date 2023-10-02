**.NET - OOPS Interview questions**

1\. What are the four pillars of OOPs Concepts?

encapsulation, inheritance, abstraction, polymorphism.

2\. What are the man concepts of OOPs?

Class, object, encapsulation, inheritance, abstraction, polymorphism.

3\. Describe the class and object?

Class is a logical unit or blueprint that contains fields, methods, and
properties.

Constructor is a special method in the class and gets executed When user
created object of a class.

Fields the members of the class and it is a variable of any type. These
holds the data.

Properties meant for getting/setting fields.

Method is an code block that contains series of code statements
/business logic.

Object is an instance of a class.

![A computer screen shot of a program Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image1.png){width="6.5in"
height="2.033333333333333in"}

![A computer screen shot of a computer code Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image2.png){width="6.5in"
height="1.2833333333333334in"}

4\. What are the different types of constructors in a class?

-   A class can have any number of constructors.

-   Constructor doesn't have any return type, not even void.

-   With in class, you can create one static constructor only.

-   Static constructor cannot be parameterized constructor.

**Default constructor**: Constructor without parameters used to called
as **Default constructor**. The drawback of a default constructor is
that every instance of the class will be initialized to the same values,
and it is not possible to initialize each instance of the class with
different values. The default constructor initializes: 

1.  All numeric fields in the class to zero.

2.  All string and object fields to null.

**parameterized constructor**: A constructor with at least one parameter
is called a **parameterized constructor**. The advantage of a
parameterized constructor is that you can initialize each instance of
the class with a different value.

**Copy constructor**: A constructor which creates an object by copying
the values of another object is called as **copy constructor**.

**Static constructor**:

A constructor which can be created with an static keyword called as
**static constructor**.

It will be invoked only once for all the instances of the class.

Static constructor used to initialize the static members of an class.

**Some key points of a static constructor are:** 

1.  A static constructor does not take access modifiers or have
    > parameters.

2.  A static constructor is called automatically to initialize the
    > class before the first instance is created or any static members
    > are referenced.

3.  A static constructor cannot be called directly.

4.  The user has no control over when the static constructor is executed
    > in the program.

5.  A typical use of static constructors is when the class is using a
    > log file and the constructor is used to write entries to this
    > file.

![A screenshot of a computer program Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image3.png){width="6.5in"
height="3.5618055555555554in"}

**Private constructor**:

A constructor can be created with a private specifier called as
**private constructor**.

Other classes won't inherit the properties of class which is having
private constructor.

We can avoid object creation with new keyword by using private
constructor.

Some key points of a private constructor are:

1.  One use of a private constructor is when we have only static
    > members.

2.  It provides an implementation of a singleton class pattern.

3.  Once we provide a constructor that is either private or public or
    > any, the compiler will not add the parameter-less public
    > constructor to the class.

![A screenshot of a computer Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image4.png){width="6.5in"
height="2.3666666666666667in"}

5\. What is Inheritance? Why inheritance is important?

Inheritance is creating/establishing parent-child relationship between
two classes where child classes automatically gets properties and method
of a parent class.

![A close-up of words Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image5.png){width="4.645833333333333in"
height="1.25in"}

![A screenshot of a computer Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image6.png){width="6.21875in"
height="0.8958333333333334in"}

Why important?

Reusability and abstraction

Keypoints :\
We can't inherit child from static class and sealed classes.

6\. What are the different types of inheritance?

Single inheritance:

It is an type of inheritance in which one class derived from its parent.

Multiple inheritance:

Multiple Inheritance was not possible in C#. We can achieve this
multiple inheritance with help of interfaces.\
\
Multi-level inheritance:\
When one class is derived from another, this type of inheritance is
called multilevel inheritance\
\
Hierarchal inheritance:\
This is the type of inheritance in which there are multiple classes
derived from one base class.

The following are some key points about inheritance:

1.  C# does not support multiple inheritances of classes, the same thing
    > can be done using interfaces.

2.  Private members are not accessed in a derived class when one class
    > is derived from another.

![](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image7.png){width="6.5in"
height="3.1444444444444444in"}

7\. How to prevent class from being inherited?\
Make that class as **Sealed** class. Sealed classes cannot be
inherited.\
If the class contains all static members, then make as static class.
Static class cannot be Inherited.

8\. What is abstraction?

It is an process to hide the internal details and show only the required
things/functionality. It will make our programmes more secure.\
In below example client knows only property and **calculateSalary**
method. But he doesn't know any methods which are inside calculate
salary. Abstraction can be achieved with either abstract classes or
interfaces.

![A screenshot of a computer program Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image8.png){width="6.5in"
height="1.8118055555555554in"}

9\. How to prevent instance creation of class?\
We can prevent object creation of class in multiple ways.

1\. Make class static

2\. private / protected constructor

3\. abstract class

10\. What is Encapsulation?

It is an process of wrapping up data and methods/properties into single
unit. Property is the best example for encapsulation concept. Direct
accessing of field member of class was the example of violation of
encapsulation.

![A screenshot of a computer Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image9.png){width="6.5in"
height="2.832638888888889in"}

11\. What is Polymorphism?

Polymorphism means multiple forms. Functions with same name, different
arguments but having multiple forms/behavior.\
\
![A screenshot of a computer code Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image10.png){width="5.197916666666667in"
height="1.9895833333333333in"}

There are two types of polymorphism.

-   Static or Compile Time Polymorphism

-   Dynamic or Runtime Polymorphism

![A diagram of polymorphosis Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image11.png){width="6.5in"
height="3.047222222222222in"}

**Compile time polymorphism:**\
Method overloading is a type of static or compile time polymorphism.
Overloading is the concept of having same name with different arguments/
signatures. It is also known as early binding.

public class TestData

{

public int Add(int a, int b, int c)

{

return a + b + c;

}

public int Add(int a, int b)

{

return a + b;

}

}

class Program

{

static void Main(string\[\] args)

{

TestData dataClass = new TestData();

int add2 = dataClass.Add(45, 34, 67);

int add1 = dataClass.Add(23, 34);

}

}

**Run-time Polymorphism:**

Dynamic/runtime polymorphism is also known as late binding. Here, the
method name and the method signature (the number of parameters and
parameter type must be the same and may have a different
implementation). Method overriding is an example of dynamic
polymorphism.

Method overriding can be done using inheritance. Method overriding
allows us to re-write the base class function/method in derived class.

A method cannot be overriden if:

-   Methods have a different return type.

-   Methods have a different access modifier.

-   Methods have a different parameter type or order.

-   Methods are non virtual or static.

public class Drawing //base class

{

public virtual double Area()

{

return 0;

}

}

public class Circle : Drawing

{

public double Radius { get; set; }

public Circle()

{

Radius = 5;

}

public override double Area()

{

return (3.14) \* Math.Pow(Radius, 2);

}

}

public class Square : Drawing

{

public double Length { get; set; }

public Square()

{

Length = 6;

}

public override double Area()

{

return Math.Pow(Length, 2);

}

}

class Program

{

static void Main(string\[\] args)

{

Drawing circle = new Circle();

Console.WriteLine(\"Area :\" + circle.Area());

Drawing square = new Square();

Console.WriteLine(\"Area :\" + square.Area());

Drawing rectangle = new Rectangle();

Console.WriteLine(\"Area :\" + rectangle.Area());

}

}

12\. What is Method hiding in C#?

Method hiding allows us to hide the implementation methods of base class
from derived class by using new keyword.

We are redefining the behavior of parent class method in a child class
by using new keyword.no connection with parent class.

Method overriding and hiding are both same But there was an major
important differences.

1.  In method overriding, only virtual or abstract methods are allowed
    > to be overridden in child class but in the case of method
    > hiding child class can reimplement any method of parent class
    > regardless of being virtual or abstract.

2.  The keyword override is used for overridden methods where
    > keyword new is used for hiding the method.

13\. What is Method overloading in C#?

Method loading is a type of compile time polymorphism. It is concept of
override the method with different signatures.

**Why is it compile time polymorphism?\
**.NET compiler at the time of compiling C# code into machine code
language knows that method has same name and different signatures.

public class TestData

{

public int Add(int a, int b, int c)

{

return a + b + c;

}

public int Add(int a, int b)

{

return a + b;

}

}

class Program

{

static void Main(string\[\] args)

{

TestData dataClass = new TestData();

int add2 = dataClass.Add(45, 34, 67);

int add1 = dataClass.Add(23, 34);

}

}

14\. What are the difference between method overloading vs method
overriding?

  -----------------------------------------------------------------------
  **Method Overloading**              **Method overriding**
  ----------------------------------- -----------------------------------
  Same name in the same class and all Same name and same signature but in
  methods are working in different    different classes
  way.                                

  Method overloading doesn't use any  It will use virtual or abstract
  special keywords like virtual,      keyword for base class method\
  override.                           override keyword for derived class.

  It won't need Inheritance to        Method overriding needs
  achieve method overloading          inheritance.

  If the number of parameters and     Same signature means the methods
  type doesn\'t match by any method   must have the same name, same
  signatures, then it will give the   number of arguments and same type
  compile time error.                 of arguments.
  -----------------------------------------------------------------------

15\. What are the difference between method overriding vs hiding?

  -----------------------------------------------------------------------
  **Method Overriding**               **Method hiding**
  ----------------------------------- -----------------------------------
  In method overriding,               In method hiding, we can override
  only virtual or abstract methods    any method regardless of being
  are allowed to be overridden        virtual or abstract. (no static)
  in child class                      

  The keyword override is used for    keyword new is used for hiding the
  overridden methods                  method
  -----------------------------------------------------------------------

15\. What are the advantages and limitations of OOPS?

Advantages:

-   **Reuse of code** through inheritance.

-   **Flexibility** through polymorphism. Same method name will do
    different things. So, we have flexibility to use right method in
    your application as per our need.

-   **Security of data** through data hiding/Encapsulation.

-   **Simple to upgrade/scale** from smaller to larger applications.

-   **Modularity** is meant easier for troubleshooting.

Limitations:

-   It is not suitable for small applications.

16\. What is an operator overloading?

Operator overloading is the concept of redefine or overload most of the
built-in operators available in C#.\
\
using System;

using System.Collections.Generic;

using System.Linq;

using System.Text;

using System.Threading.Tasks;

namespace ConsoleApp1

{

internal class OperatorOverloading

{

class Calculator

{

public int number = 0;

// no-argument constructor

public Calculator() { }

// parameterized constructor

public Calculator(int n)

{

number = n;

}

// Overloading of Binary \"+\" operator

public static Calculator operator +(Calculator Calc1,

Calculator Calc2)

{

Calculator Calc3 = new Calculator(0);

Calc3.number = Calc2.number + Calc1.number;

return Calc3;

}

// function to display result

public void display()

{

Console.WriteLine(\"{0}\", number);

}

}

// Driver Code

static void Main(string\[\] args)

{

Calculator num1 = new Calculator(200);

Calculator num2 = new Calculator(40);

Calculator num3 = new Calculator();

num3 = num1 + num2;

num1.display(); // Displays 200

num2.display(); // Displays 40

num3.display(); // Displays 240

}}}}

+---+-------------------------------------------------------------------+
|   | **Operators & Description**                                       |
+===+===================================================================+
| 1 | **+, -, !, \~, ++, \--**                                          |
|   |                                                                   |
|   | These unary operators take one operand and can be overloaded.     |
+---+-------------------------------------------------------------------+
| 2 | **+, -, \*, /, %**                                                |
|   |                                                                   |
|   | These binary operators take one operand and can be overloaded.    |
+---+-------------------------------------------------------------------+
| 3 | **==, !=, \<, \>, \<=, \>=**                                      |
|   |                                                                   |
|   | The comparison operators can be overloaded.                       |
+---+-------------------------------------------------------------------+
| 4 | **&&, \|\|**                                                      |
|   |                                                                   |
|   | The conditional logical operators cannot be overloaded directly.  |
+---+-------------------------------------------------------------------+
| 5 | **+=, -=, \*=, /=, %=**                                           |
|   |                                                                   |
|   | The assignment operators cannot be overloaded.                    |
+---+-------------------------------------------------------------------+
| 6 | **=, ., ?:, -\>, new, is, sizeof, typeof**                        |
|   |                                                                   |
|   | These operators cannot be overloaded.                             |
+---+-------------------------------------------------------------------+

17\. What are different type of classes in C#?

-   Abstract class

-   Sealed class

-   Static class

-   Partial class

18\. What is a static class?

Static class is a class which contains all static member, methods.

**Characteristics of static class in C#**

1.  Static class cannot be instantiated using a new keyword.

2.  Static items can only access other static items. For example, a
    > static class can only contain static members, e.g., variables,
    > methods, etc.

3.  A static method can only contain static variables and can only
    > access other static items.

4.  Static items share the resources between multiple users.

5.  Static cannot be used with indexers, destructors, or types other
    > than classes.

6.  A static constructor in a non-static class runs only once when the
    > class is instantiated for the first time.

7.  A static constructor in a static class runs only once when any of
    > its static members are accessed for the first time.

8.  Static members are allocated in a high-frequency heap area of the
    > memory.

  -----------------------------------------------------------------------
  Static class                        Non-static class
  ----------------------------------- -----------------------------------
  It is defined by using static       It was not defined by using static
  keyword.                            key word.

  We cannot create an object of       We can create an object of sealed
  static class.                       class.

  Static classes cannot be inherited. Non-static classes can be
                                      inherited.

  It can have only static members.    It can have both static and
                                      non-static members.

  We can access static members by     We can access non-static members
  using class name.                   through instance of class.

                                      

                                      
  -----------------------------------------------------------------------

19\. What is a sealed class?

Sealed classes are used to restrict the users from inheriting the class.
A class can be sealed by using the sealed keyword. The keyword tells the
compiler that the class is sealed, and therefore, cannot be extended. No
class can be derived from a sealed class.

**e.g** the "Pens" and "Brushes" classes of the **System.Drawing**
namespace. The Pens class represents the pens for standard colors. This
class has only static members. For example, "Pens.Red" represents a pen
with red color. Similarly, the "Brushes" class represents standard
brushes. "Brushes.Red" represents a brush with red color.

20\. What is a abstract class?

To create an abstract class, we can use abstract keyword before class
definition. This class servers as base class for other classes

**Important Points:** 

-   Generally, we use abstract class at the time of *inheritance*.

-   A user must use the *override* keyword before the method is declared
    > as abstract in the child class, the abstract class is used to
    > inherit in the child class.

-   An abstract class cannot be inherited by structures.

-   It can contain constructors or destructors.

-   It can implement functions with non-Abstract methods.

-   It cannot support multiple inheritances.

-   It can't be static.

-   Cannot create instance of abstract type or Interface.

-   With help of abstract class , we can achieve abstraction.

**Advantages:**

1.  Encapsulation: Abstract classes allow you to define a common set of
    > behaviors or properties that derived classes should have, without

2.  exposing the implementation details of those behaviors or properties
    > to the outside world. This can help you create more maintainable
    > and flexible code.

3.  Code reuse: Abstract classes can be used as a base class for
    > multiple derived classes, which can help reduce code duplication
    > and improve code reuse.

4.  Polymorphism: Abstract classes can be used to achieve polymorphism,
    > which allows you to write code that works with objects of
    > different derived classes, as long as they all inherit from the
    > same abstract base class.

**Disadvantages:**

1.  Tight coupling: Abstract classes can create tight coupling between
    > the base class and derived classes, which can make it harder to
    > modify the base class without affecting the derived classes.

2.  Limited inheritance: C# only allows a class to inherit from a single
    > base class, so if you use an abstract class as a base class, you
    > limit the ability of derived classes to inherit from other
    > classes.

3.  Difficulty in testing: Because abstract classes cannot be
    > instantiated directly, they can be more difficult to test than
    > regular classes. In order to test a derived class, you may need to
    > create a mock or stub of the abstract base class.

4.  Overall, abstract classes can be a powerful tool for creating
    > flexible and maintainable code, but they should be used
    > judiciously, taking into account the specific requirements of your
    > application.

21\. What is an interface?

An interface is an completely abstract class which is contains only
abstract methods and properties with empty bodies.

Notes:

-   By default, members of an interface are abstract and public.\
    you do not have to use the override keyword when implementing an
    interface.

-   Interface methods do not have a body - the body is provided by the
    \"implement\" class.

-   On implementation of an interface, you must override all of its
    methods.

-   Interfaces can contain properties and methods, but not
    fields/variables.

-   Interface members are by default abstract and public.

-   An interface cannot contain a constructor (as it cannot be used to
    create objects)

#### **Why And When To Use Interfaces?**

1\) To achieve security - hide certain details and only show the
important details of an object (interface).

2\) C# does not support \"multiple inheritance\" (a class can only
inherit from one base class). However, it can be achieved with
interfaces, because the class can **implement** multiple
interfaces. **Note:** To implement multiple interfaces, separate them
with a comma .

 Complete Abstraction can be achieved by the implementation of
Interface.

Along with making our code easy to maintain, concept loose coupling can
be achieved.

// Interface

interface IAnimal

{

void animalSound(); // interface method (does not have a body)

}

// Pig \"implements\" the IAnimal interface

class Pig : IAnimal

{

public void animalSound()

{

// The body of animalSound() is provided here

Console.WriteLine(\"The pig says: wee wee\");

}

}

22\. What is an partial class?

It is an special feature in C#. Implement the functionality of single
class into multiple files and all the files are compiled into single
file when application is compiled.

**Advantages :** 

-   With the help of partial classes, multiple developers can work
    > simultaneously in the same class in different files.

-   With the help of a partial class concept, you can split the UI of
    > the design code and the business logic code to read and understand
    > the code.

-   When you were working with automatically generated code, the code
    > can be added to the class without having to recreate the source
    > file like in Visual studio.

-   You can also maintain your application in an efficient manner by
    > compressing large classes into small ones.

23\. What are the difference between method overloading vs overriding?

  -----------------------------------------------------------------------
  **Method Overloading**              **Method overriding**
  ----------------------------------- -----------------------------------
  Multiple methods of same name in    Multiple methods of same name in
  same class                          different classes(base/derived)

  No need of inheritance              Need of inheritance, as it is in
                                      different class.

  All methods have different          All methods have same signature
  signature.                          

  It's compile time polymorphism      It's run time polymorphism

  No special keyword required         Virtual& override keywords
                                      required.
  -----------------------------------------------------------------------

24\. If a method is marked as virtual, do we must have to \"override\"
it from the child class?

No, overriding virtual method is optional.

25\. What are the difference between abstract class vs Interfaces?

  -----------------------------------------------------------------------
  **Abstract class**                  **Interfaces**
  ----------------------------------- -----------------------------------
  Abstract class contain both         Interfaces contains only abstract
  abstract and non-abstract methods.  methods.

  Abstract keyword used for defining  Interface keyword used for define
  class.                              interface.

  Doesn't support multiple            Supports multiple multiple
  inheritance                         inheritance

  Abstract class can have             Interface do not have constructors.
  constructors                        

  No special keyword required         Virtual& override keywords
                                      required.
  -----------------------------------------------------------------------

26.If two methods are same except return type, then methods are
overloaded or what will happen?\
\
No, it will throw a compile error because methods should have same
signature with parameters.

27\. how to prevent instance creation of an class.

We can achieve three different ways. 1. Private constructor 2. static
class 3. Abstract class

28\. Boxing and UnBoxing in C#?\
Converting value types into reference type called boxing. Reverse way we
used call as unboxing.

Int x = 600;

Object t = x //boxing.

Int x = (int) t; //unboxing.

29\. Is Boxing and Unboxing good for performance?\
Converting one type into another type always gives bad performance. Try
to avoid conversions but if necessary, use conversions.

30\. difference between string vs stringbuilder?

String is immutable means we cannot modify it, but it will replace with
new string when you assign new value.

StringBuilder is an mutable means we can modify it, But It won't create
new instance every time.

31\. When to use stringbuilder?

In real time applications, if you want to change string multiple times,
then choose stringbuilder. Because it won't consume extra memory in
everytime.

32.What is string interpolation?

string interpolation provides more readable, convenient syntax to format
strings.

e.g const age = 38;

console.WriteLine("I am Ramesh Bole and {0} years old", age);

console.WriteLine(\$"I am Ramesh Bole and {age} years old");

33.What is the difference between "continue" and "break" statement?

**Continue statement** end the loop iteration and transfer the control
to the beginning of the loop.

**Break statement** end the loop iteration and exit the loop.\
![A screenshot of a computer program Description automatically
generated](vertopal_bf8f2d9e08cf4da298b8926692784191/media/image12.png){width="6.5in"
height="3.3333333333333335in"}

34.How to implement Exception Handling in C#?

Exception handling in object-oriented programming is used to
handle/mange the errors.

**Try** : this is the place where exceptions will throw to catch block.

**Catch Block:** this is the place where we handled the errors. We can
write/define multiple catch blocks, when we run application, any
exception occurs. only one catch block executes based on what type of
error received from try block.

**Finally:** irrespective of exception, each and every time finally
block code executes. This is used in real time applications mostly for
disposing unwanted objects .

