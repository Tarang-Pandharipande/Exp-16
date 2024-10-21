# Experiment 16

**Aim:**  
To explore and apply the concept of Exception Handling.  
<br>
**Theory:**  
In C++, exception handling is a technique that allows programs to manage unexpected events or errors that occur during runtime. It provides a way to handle such situations without crashing the program. Exception handling in C++ revolves around three key keywords, as described below:  
<br>
Keywords of Exception Handling:  
&#8594; _throw:_ When an error is detected, an exception is "thrown" to signal the issue. It can send any value, but commonly integers, strings, or objects are used to describe the nature of the error.  
&#8594; _catch_: Once an exception is thrown, the program searches for a "catch" block that can handle that particular type of exception. The catch block specifies how to respond to a certain type of exception. The type of exception thrown must match the type expected by the catch block. If no matching catch block is found, the program terminates.  
&#8594; _try:_ This block contains the code that could potentially trigger an exception. If an exception occurs within the try block, control is passed to the corresponding catch block to handle the error.  
<br>
Flow of Exception Handling:  
When an exception is raised inside the try block, the program immediately redirects execution to the catch block. If the catch block matches the thrown exception, it is executed. If no appropriate catch block is found, the program halts execution.
**Code:** <br>
<br>
```
#include <iostream>
using namespace std;

int main() 
{
    int den,num;
    float ans;

    cout << "Enter the numerator: ";
    cin >> num;
    cout << "Enter the denominator: ";
    cin >> den;

    try 
    {
        if (den == 0) 
        {
            throw 0;  
        }

        cout << "Answer: "<< num/den << endl;
    }

    catch (int x) 
    {
        cout << "ERROR: DIVISION BY ZERO" << endl;
    }

}

```
<br>

**Outputs:**  <br>
<br>
![exp16a output](https://github.com/tanishaamenon/CDS---Exception-Handling/blob/main/exp16a.JPG) <br>
![exp16b output](https://github.com/tanishaamenon/CDS---Exception-Handling/blob/main/exp16a.JPG) <br>
<br>

**Conclusion:** <br>
&#8594; We learnt about exception handling in C++. <br>
&#8594; We learnt the flow of exception handling in C++. <br>
*******
<br>
