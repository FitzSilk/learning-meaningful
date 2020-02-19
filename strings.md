##<a name="strings"></a>Strings
A **String** represents a sequence of characters. They are enclosed by **double quotes**.
> ```String myName = "John Doe";```  
> ```String myName = new String("John";```
###Useful String methods
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