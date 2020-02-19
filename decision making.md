##<a name="decision"></a>Decision making
 
 Execute a block of statements under a **certain condition**.
 
 ###<a name="ifelse"></a>If... else statements
 
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

###<a name="switch"></a>Switch statements
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