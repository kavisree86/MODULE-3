# Ex.No:1
# Ex.Name: Write a c++ program to find simple & compound interest by using Hierarchical Inheritance (read the data In the order of p, n & r)
## Date:
## Aim:
To wite a c++ program to find simple & compound interest by using Hierarchical Inheritance (read the data In the order of p, n & r)

## Algorithm:

Start the program.
Create a base class to store principal, time, and rate with input function.
Derive SimpleInterest class to calculate (p * n * r) / 100.
Derive CompoundInterest class to calculate p * (pow((1 + r/100), n) - 1).
In main(), create objects of derived classes.
Call input function once from base class.
Calculate and display SI and CI.
End the program.



## Program:
```
#include <iostream>  
#include<cmath>
using namespace std;  
  
int main()
{
    float p,n,r,k;
    cin>>p>>n>>r;
    cout<<"Simple Interest Amount is :="<<p*n*r/100<<endl;
    k=p*pow((1+r/100),n)-p;
    cout<<"Compound Interest Amount is :="<<k;
}
```


## Output:

<img width="1124" height="382" alt="image" src="https://github.com/user-attachments/assets/e6ff6e19-385d-4d2f-a892-5bedf34671f3" />


## Result:
The program successfully executed for simple & compound interest by using Hierarchical Inheritance.
