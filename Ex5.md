# Ex.No:5
# Ex.Name: Write a C++ program to multiply two numbers using  derived constructor.
## Date:
## Aim:
To write a C++ program to display the Employee details using the multiple inheritance constructors.

## Algorithm:
Start the program.
Create base class EmpID with constructor to set employee ID.
Create base class EmpName with constructor to set employee name.
Create derived class Employee inheriting from both base classes.
In derived class constructor, call both base class constructors and set designation.
Add function in derived class to display ID, name, and designation.
In main(), get ID, name, and designation from user.
Create Employee object with input values.
Call display function.
End the program.




## Program:
```
#include <iostream>
using namespace std;
class base1
{
    public:
        int eid;
        void get1(){
            cin>>eid;
        }

};
class base2
{
    public:
        string name,desig;
        
        void get2(){
            cin>>name>>desig;
        }
};
class derive1 : public base1, public base2
{
    public:
        void display(){
            cout<<" Employee ID : "<<eid<<endl;
            cout<<" Employee Name : "<<name<<endl;
            cout<<" Employee Designation : "<<desig<<endl;
        }
};
int main ()
{
    derive1 obj;
    obj.get1();
    obj.get2();
    obj.display();
 return 1;   
}
```


## Output:
<img width="1020" height="397" alt="image" src="https://github.com/user-attachments/assets/a5d75783-ef28-4c7a-ae16-4ea971068c84" />



## Result:
The program successfully executed to display the Employee details using the multiple inheritance constructors.

