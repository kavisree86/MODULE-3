# Ex.No:4
# Ex.Name: Write a C++ program to pass a password (Admin@123 )to the parameterized constructor of a base class through the derived class constructor.
## Date:
## Aim:
To write a C++ program to pass a password (Admin@123 )to the parameterized constructor of a base class through the derived class constructor.

## Algorithm:

Start the program.
Define a base class with a string member to store a password.
Create a parameterized constructor in the base class to initialize the password.
Define a derived class that inherits from the base class.
In the derived class constructor, call the base class constructor and pass the password "Admin@123".
Provide a function in the base class to display the password.
In main(), create an object of the derived class.
Call the function to display the password.
End the program.



## Program:
```
#include<iostream>
using namespace std;
 
class Parent {
    public:
    
    string pass="Admin@123";
    
    Parent(){
        cin>>pass;
        cout<<"The Password passed to the base class is "<<pass<<endl;
    }
     
    
};
 
class Child : public Parent
 {
     public:
     
     Child(){
         cout<<"The Password "<<pass<<" is passed through the derived class constructor"<<endl;
     }
 };
 int main()
 {
     Child obj;
 }
 ```


## Output:
<img width="1221" height="278" alt="image" src="https://github.com/user-attachments/assets/03a08ce2-945d-478f-9739-dedd471df26f" />



# #Result:
The program successfully executed to pass a password (Admin@123 )to the parameterized constructor of a base class through the derived class constructor.
