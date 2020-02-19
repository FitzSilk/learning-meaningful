##<a name="methods"></a>Methods
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

###<a name="overloading"></a>Method overloading
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