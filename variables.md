## <a name="variables"></a>Variables

Primitive type & reference type

###<a name="primitive"></a>Primitive types:
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

###<a name="reference"></a>Reference types:

A reference type holds a reference, a **pointer** to the object in the heap.
> ```Cat myCat = new Cat("Garfield");```  
>```myCat``` is a pointer (#ref) to the cat Garfield in the heap.