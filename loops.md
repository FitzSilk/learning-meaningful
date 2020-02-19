##<a name="loops"></a>Loops
Use to execute statements multiple times.
###<a name="while"></a>While loop
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

###<a name="dowhile"></a>Do...While loop
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
   
###<a name="for"></a>For loop
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

###<a name="foreach"></a>For each loop
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