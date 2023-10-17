# Fundamentals of Dart :
<br><br>
## Dart :
> * Dart First developed 14, November 2013.
> * It is developed by Google.
> * In 2015, Dart Assembly renamed it Sky.

<br>

## * First Dart Program using DartPad, CMD and VS Code :

<br>

  ### DartPad :
  
  > * `Dartpad is used to run Dart Program in online.`


<br>

  ### CMD : 

  > * `Dart programs can also be run in CMD.`
  > * `First Text File create and save filename.dart extensions and after click path and write cmd.`
  > * `And write the dart filename.dart.` 

<br>

### VS Code : 

> * `VS Code is used to run dart program.`

<br><br>
## * Variables, Datatypes, Constants :

<br>

### * Variable : 

> * Variables are the contener which stores the same value.
> * Where we can store some value.

<br>

### * Datatype :
> * Datatype is simply a type of data.
> * `int`
> * `String`
> * `double`
> * `bool`

<br>

#### New Datatype : 
> * `dynamic`
> * `var` => var is Keyword not datatype.

<br>

#### dynamic Datatype : 
> * when a variable is declared as a dynamic type, it can store any value, such as int and float .
> * Dynamic can access any value. So any datatype can run in it.

<br>

<pre>
  Example: 

 void main() {
  
     dynamic d = "Jaynesh";

     d = 3.14;

     d = true;

     d = 50;
  
 }
</pre>

<br>

#### var Datatype : 
> * when a variable is declared as a var type, it can store any value, such as int and float .
> * var can access any value. So any datatype can run in it.
> * but Create any var variable and only after assigning a value it will run that data.Any other data will not work.

<br>

<pre>
  Example: 

 void main() {
  
     var v = "Jaynesh";

     v = 3.14; // error
  
 }

  void main() {

    var v;

    v = "Jaynesh";
    v = 3.14;
  
  }
</pre>

<br><br>

### * Constants : 

> * `Constant means to fix value of variable.`.
> * `when we make a variable const that time we have to assign value to the variable.`
> * `A final can also be written instead of const.`
> * `final works the same as const. To fix the value.`
> * `When we final the variable we don't need to assign the value to the variable.`

<br>

<pre>
  void main() {
      const PI = 3.14;

      final PI;
      PI = 3.14;
  
  }
</pre>

<br>

### * Operators :

#### 1. Floor Division Operator :
> * `When we do division between int and int then the value comes in by default point. But the value returns to int from the flooor divcon operator.`

<br>

<pre>
  void main() {
  
      int a = 10;
      int b = 3;

      print(a~/b); // floor Division Operator
  
  }
</pre>

<br><br>

### * String Interpolation :

<br>

<pre>
  void main() {
  
      int a = 10;
      int b = 3;

      print("Division of $a and $b : ${a~/b}"); // ${} => String Interpolation.
  
  }
</pre>

<br>

## How to take user input in dart ?

<br>

<pre>
  void main() { 

      int n;

      stdout.write("Enter any Number : ");
      n = int.parse(stdin.readLineSync()!);

      double pi;

      stdout.write("Enter any Real Number : ");
      pi = double.parse(stdin.readLineSync()!);

      String name;

      stdout.write("Enter your Name : ");
      name = stdin.readLineSync();
  
  }
</pre>

## Types of collection datatype : 

> `Primiteve : `
> * int
> * String
> * double
> * bool
> * dynamic.

<br>

> `Collection : `
> * List (Fixed-length, growable)
> * Set
> * Map

<br><br>

### - List (fixed-length & growable) : 
> * `List is collection of multiple values which can have multiple datatype.`
> * List write only for [] (square) bracket.



