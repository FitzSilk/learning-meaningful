##<a name="arrays"></a>Arrays
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