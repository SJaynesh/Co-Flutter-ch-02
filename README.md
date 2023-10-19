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

#### var Keyword : 
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
> * `When we do division between int and int then the value comes in by default point. But the value returns to int from the floor division operator.`

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

<br><br>

## Types of collection datatype : 

<br>

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
> * List is an ordered collection of values, which contains index values to access it's inner attributes.
> * List have indexes like arrays.
> * List can be created using '[]'.

<br>

### How to declration List :

<br>

> `Syntax : ` List variableName = [Values];

<br>

<pre>

  void main() {
  
    List name = ["Jaynesh", "A", "B", "C"];

    print(name[0]);
}

  
</pre>

<br>

#### To add up :

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    name.add(50);
  
    print(name);
}

</pre>

<br>

### To add Multiple values :

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    name.addAll(['Akhil', 40, 90]);
  
    print(name);
}

</pre>

<br>

### To Insert to value :

<br>

<pre>
  void main() {
  List name = ["Jaynesh", "A", "B", "C"];

  print(name[0]);

  name.insert(2, 50);

  print(name);
}

</pre>

<br>

### To Insert multiple value :

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    name.insertAll(2, [1, 2, 3, 4]);
  
    print(name);
}

</pre>

<br>

### To know the index of the list Value :

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    int i = name.indexOf("Jaynesh");
  
    print(i);
}

</pre>

<br>

### To Remove a Value : 

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    name.remove("B");
  
    print(name);
}

</pre>

<br>

### To Remove a value for Index :

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    name.removeAt(3);
  
    print(name);
}

</pre>

<br>


### To Reverse a List :

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    print(name.reversed.toList());
}

</pre>

<br>

### To Show Datatype : 

<br>

<pre>
  void main() {
    List name = ["Jaynesh", "A", "B", "C"];
  
    print(name[0]);
  
    print(name.runtimeType);
}

</pre>

<br><br>

## * Generics : 
> * Generics will be used to fix the datatype in the list.
> * fix any one data type in the collection data types.
> * it can be applied to either data types, value or both.
>   `List <int> number = [10,20,30,40,50];` 

<br>

<pre>
  import 'dart:io';

void main() {
  List name = [];

  print("Enter number of Name : ");
  int n = int.parse(stdin.readLineSync()!);

  for (int i = 0; i < n; i++) {
    print("Enter Name : ");
    String val = stdin.readLineSync()!;
    name.add(val);
  }

  print(name);
}

</pre>

<br>


## * Types of List :
> 1. `growable` (default)
> 2. `fixed length`

<br><br>

### 1. growable :
#### Syntax :
> `List a = List.generate(length, (index) => element);`

<pre>
  void main() {

    List a = List.generate(10, (index) => index + 1);

    print(a);
}

</pre>

## 2. Fixed Length :
  > * List.generate(length, (index) => element,growable: true);
  > * List.unmodifiable([]);
  > * List.empty(growabl;e: false)


### How to Fixed length in list ? 
> * To write growable : false.

<pre>
  void main() {
    List a = List.generate(10, (index) => index + 1, growable: false);

    a.add("11");

    print(a); // exception
}

</pre>

### To Fix length or Values :
> ` List a = List.unmodifiable([Values]);`

<pre>
  void main() {
  
     List a = List.unmodifiable([10, 20, 30, 40, 50]);

     a[3] = 80; // exception

     print(a);
  
  }
</pre>


### How to User Input in List :

#### Type : 01
<pre>
import 'dart:io';

void main() {
  int n;

  stdout.write("Enter length in list : ");
  n = int.parse(stdin.readLineSync()!);

  List a = List.generate(n, (index) => null);

  for (int i = 0; i < n; i++) {
    stdout.write("Enter any Value : ");
    a[i] = stdin.readLineSync()!;
  }

  print(a);
}

</pre>





