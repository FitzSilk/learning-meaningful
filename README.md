# Java Basics Summary

## Summary
- [Variables](#a-namevariablesavariables)
    - [Primitive types](#a-nameprimitiveaprimitive-types)
    - [Reference types](#a-namereferenceareference-types)
- [Expressions](#a-nameexpressionsaexpressions)
    - [Arithmetical operators](#a-namearithmeticalaarithmetical-operators)
    - [Relational operators](#a-namelogicalalogical-operators)
    - [Logical operators](#a-namelogicalalogical-operators)
- [Methods](#a-namemethodsamethods)
    - [Method overloading](#a-nameoverloadingamethod-overloading)
- [Strings](#a-namestringsastrings)
- [Decision making](#a-namedecisionadecision-making)
    - [If... Else statements](#a-nameifelseaif-else-statements)
    - [Switch statements](#a-nameswitchaswitch-statements)
- [Arrays](#a-namearraysaarrays)
- [Loops](#a-nameloopsaloops)
    - [While Loop](#a-namewhileawhile-loop)
    - [Do...While Loop](#a-namedowhileadowhile-loop)
    - [For Loop](#a-nameforafor-loop)
    - [For Each Loop](#a-nameforeachafor-each-loop)
- [Objects](#a-nameobjectsaobjects)
    

## <a name="variables"></a>Variables

Primitive type & reference type

### <a name="primitive"></a>Primitive types:
- Integer
    - **byte** (-128 -> 127) 
        >```byte myAge = 5;```
    - **short** (-32 768 -> 32 767)
        >```short cold = -15;```
    - **int** (-2 147 483 648 -> 2 174 483 647)
        >```int size = 128;```
    - **long** (put a L after the value)
        >```long someVal = 650L;```
- Floating point
    - **float** (up to 7 digit precision) (put a f after the value)
        >```float height = 1.76f;```
    - **double** (up to 16 digit precision)
        >```double pi = 3.14159265;```
- Boolean
    - **true** or **false**
        >```boolean isComplex = false;```
- Character
    - a **single character**. It's enclosed by **single quotes**.
        >```char initial = 'A';```

### <a name="reference"></a>Reference types:

A reference type holds a reference, a **pointer** to the object in the heap.
> ```Cat myCat = new Cat("Garfield");```  
>```myCat``` is a pointer (#ref) to the cat Garfield in the heap.

## <a name="expressions"></a>Expressions:

### <a name="arithmetical"></a>Arithmetical operators

- Addition ```+``` 
>```int addition = 5 + 10;```
- Subtraction ```-``` 
>```int subtraction = 3 - 2;```
- Multiplication ```*``` 
>```int multiplication = 3 * 2;```
- Division ```/``` 
>```int division = 6 / 2;```
- Modulus / Remainder ```%```
>```int modulus = 5 % 2;```
- Post-increment ```++```
>```addition++;```
- Post-decrement ```--```
>```addition--;```
- Pre-increment ```++```
>```++addition;```
- Pre-decrement ```--```
>```--addition;```
- Compound assignement ```+=, -=, %=, *=, /=```
>```addition += 3;```

### <a name="relational"></a>Relational operators

- Equal to ```==```
>```boolean isEqual = 5 == 10;```
- Not equal to ```!=```
>```boolean isNotEqual = 5 != 10;```
- Greater than ```>```
>```boolean isGreaterThan = 5 > 4;```
- Less than ```<```
>```boolean isLessThan = 5 < 4;```
- Greater than or equal to ```>=```
>```boolean isGreaterOrEqual = 5 >= 5;```
- Less than or equal to ```<=```
>```boolean isLessOrEqual = 5 <= 4;```

### <a name="logical"></a>Logical operators

- Logical AND : both are true ```&&```
>```boolean and = true && false;```
- Logical OR : one of them is true ```||```
>```boolean or = true || true```;
- Logical NOT : true if operand is false ```!```
>```boolean not = !false;```
- Logical XOR : true if only one is true ```^```
>```boolean xor = true ^ true;```

**You can combine these operators :**
> **```((5 >= 3) && true) && (((2+4) > 5) || (3 < 2)) && !(3!=3) == true```**

## <a name="methods"></a>Methods
```
public void doSomething(){
    System.out.println("I do!");
}
```
>```public``` is the **access modifier**.  
>```void``` is the **return type**. **void** means nothing will be returned, otherwhise you've to **return** something at the end of the method.  
>```doSomething``` is the **name** of the method. We use **camelCasing** convetions.  
>Between the ```()``` you define the **parameters** of the method.  
>Between the ```{}``` (inside the **body**) is the implementation of what the method will do.  
>You call the method with ```doSomething();``` on your main application.

### <a name="overloading"></a>Method overloading
You can **overload** a method and using it to have only one method that will act on differents types of parameters.  
The combination of the **method’s name** and the **method’s parameter types** is called the **signature** of the method.  
**A method’s signature needs to be unique**
```
public int sum(int n1, int n2){
    return n1 + n2;
}

public double sum(double n1, double n2){
    return n1 + n2;
}
public float sum(float n1, float n2){
    return n1 + n2;
}
```

## <a name="strings"></a>Strings
A **String** represents a sequence of characters. They are enclosed by **double quotes**.
> ```String myName = "John Doe";```  
> ```String myName = new String("John";```
### Useful String methods
- **substring** method
    ```
    String myName = "John Doe";
    String firstName = myName.substring(0, 4); // will hold "John"
  ```
  Get a part of a string. Start at index 0. (n-1)
- **length** method
  ```
  String myNickname = "Coolio";
  int numberOfChars = myNickname.length(); // will hold 6
  ```
  Find the length of a String instance.
- **concat** method
   ```
  String firstName = "John";
  String lastName = "Johnson";
  String fullName = firstName.concat(" "+lastname); // will hold "John Johnson"
  ```
  Concatenate two different string objects together.
- **indexOf** method
    ```
  String myName = "John Doe";
  int indexOfN = myName.indexOf('n'); // will hold 3.
  ```
  Find the index of a character (or a string).
 
 - **equals** method
    ```
    boolean isEqual = aName.equals(anotherName);
   ```
   Validates whether or not two String objects are equal (can be override).
   
 ## <a name="decision"></a>Decision making
 
 Execute a block of statements under a **certain condition**.
 
 ### <a name="ifelse"></a>If... else statements
 
 ```
if(<conditional expression>){
    // code to execute if condition is met
}
```
>```
>public void yawn(int currentHour){
>    if(currentHour > 22){
>        System.out.println("Yawn");
>    }
>    else if(currentHour < 8){
>        System.out.println("Zzz");
>    }
>    else{
>       System.out.println("Working");
>    }
>}
You can execute condition for several conditions.
>```
>public void yawn(int currentHour){
>    if(currentHour > 8 && currentHour < 22){
>        System.out.println("Working!");
>    }
>}
You can combine expressions in one condition.

### <a name="switch"></a>Switch statements
The **switch** statement is use to **operates on values**.
```
switch(expression){
    case value:
        // statement
        break;
    // extra cases
    default:
        // default statement
        break;
}
```
>```
>public void tellMyAge(int age){
>    switch(age){
>        case 0:
>            System.out.print("0 years, just born!");
>            break;
>        case 1:
>            System.out.print("1 year old!");
>            break;
>        default:
>            System.out.print("Getting older...");
>            break;
>    }
>}
>```
>```
>public void tellMyAge(int age){
>    switch(age){
>        case 0:
>        case 1:
>        case 2:
>        case 3:
>            System.out.print("Not old");
>            break;
>        default:
>            System.out.print("Getting older...");
>            break;
>    }
>}
You **need** the ```break;``` statement otherwise the system will continue to execute your code until it finds a break int it.  
You can put several cases before the break in order to give the same execution for these cases.

## <a name="arrays"></a>Arrays
An **array** is a type of **data structure** that stores a **group of variables of the same type**.  
The **length** of an array is **fixed**. It is set **upon initialization**, **required** and can **never be altered** for that array.  
**Declaring** an array is done by using the ```[]``` behind is type.
>```type[] name;```
```
String[] games = new String[3];
String[] games = {"Half-Life 3", "Doom", "Morrowind");
```
As with the substring method, you can access a specific value by using his index (who is n-1).
```
String bestGame = games[2]; // will hold "Morrowind"
```
You can also use methods to it.
```
int amountOfGames = games.length; /// will hold 3
```
**Be aware** that the ```.length``` method here doesn't use ```()```

## <a name="loops"></a>Loops
Use to execute statements multiple times.
### <a name="while"></a>While loop
```
while(<conditional expression">{
    //code to execute
}
```
>```
>public void sayHello(int amount){
>    while(amount > 0){
>        System.out.println("Hello");
>        amount--;
>    }
>}

### <a name="dowhile"></a>Do...While loop
```
do{
    //code to execute
}while(<conditional expression">;
```
The **Do... While** loop will go through the code **once no matter what** and then will check for the conditional expression.
>```
>public void sayHello int amount) {
>   do{
>       System.out.println("Hello");
>       amount--;
>   } while(amount > 0);
>}
   
### <a name="for"></a>For loop
```
for(<Initialization>; <Condition>; <Increment){
    //code to execute
}
```
The **For** loop will iterate **over a range of values**.
>```
>public void sayHello(int amount){
>   for(int i=0; i < amount; i++){
>       System.out.println("Hello");
>   }
>}

### <a name="foreach"></a>For each loop
```
for(<Declaration> : <array|collection>){
    //code to execute
}
```
The **For each** loop will iterate **over a collection of values** (even without knowing the range of values).
>```
>for(int number : numbers){
>   System.out.println(number);
>}
>```
>```
>for(Cat[] cat : cats){
>   cat.feed();
>}

## <a name="objects"></a>Objects
