# Ex.No:2
# Ex.Name: Write a program to implement protected member with fractional values?
## Date:
## Aim:
To write a program to implement protected member with integer values

## Algorithm:
Algorithm:
Start the program.
Define a base class with a protected integer variable.
Provide a public function in the base class to assign value to the protected variable.
Define a derived class inheriting from the base class.
In the derived class, create a function to display the protected variable.
In main(), create an object of the derived class.
Call the base class function to set the value.
Call the derived class function to display the value.
End the program.




## Program:
```
#include <iostream>
using namespace std;

class Base 
{
protected:
    int num;  

public:
    void setNum(int n)
    {
        num = n;
    }
};

class Derived : public Base
{
public:
    void displayNum()
    {
        cout << "The value of num is: " << num << endl;
    }
};

int main()
{
    Derived obj;
    int input;

    cin >> input;

    obj.setNum(input);

    obj.displayNum();

    return 0;
}
```


## Output:

<img width="952" height="293" alt="image" src="https://github.com/user-attachments/assets/44e47be3-1975-47c1-bf82-ce87611d6749" />


## Result:
The program successfully executed to implement protected member with integer values.
