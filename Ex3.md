# Ex.No:3
# Ex.Name: Write a C++ program to get two numbers from two base classes and display the quotient in the derived class.
(Illustrate multiple Inheritance and use appropriate access specifier)
## Date:
## Aim:

To write a c++ program to find difference & quotient of two numbers using Hierarchical inheritance
## Algorithm:

Start the program.
Create a base class with two integer members and a function to read values.
Derive a class Difference from the base class and add a function to calculate a - b.
Derive another class Quotient from the base class and add a function to calculate a / b.
In main(), create objects of derived classes.
Call the base class function to input numbers.
Call the respective functions to display difference and quotient.
End the program.



## Program:
```
#include<iostream>
using namespace std;
class Base
{
    public:
    int a,b;
};
class Derived1:public Base
{
    public:
    void product()
    {
        cin>>a>>b;
        cout<<"Difference="<<a-b<<endl;
    }
};
class Derived2:public Base
{
    public:
    void Sum()
    {
        cin>>a>>b;
        cout<<"Quotient="<<a/b<<endl;
    }
};
int main()
{
    Derived1 d1;
    d1.product();
    Derived2 d2;
    d2.Sum();
    return 0;
}
```


## Output:

<img width="793" height="330" alt="image" src="https://github.com/user-attachments/assets/266d4cb6-3f3a-4099-ba31-ca0ad641fe39" />


## Result:
The program successfully executed for difference & quotient of two numbers using Hierarchical inheritance.
