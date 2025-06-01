# 3A INHERITANCE(BASE CLASS & DERIVED CLASSES) 

## PROGRAM STATEMENT:
write a C++ program to read regno,name & gender in one class and display the above details in another class using inheritance.

## ALGORITHM:
1. Define a base class Student with regno, name, gender and input method.
2. Create a derived class Display using public inheritance.
3. In the derived class, create a method to display the student details.
4. In main(), create an object of the derived class.
5. Call input and display methods, and end the program.

## PROGRAM:
```
#include <iostream>
using namespace std;
class A
{
    public:
        int regno;
        string name,gender;
};
class B: public A
{ 
public:
void func()
{
cin>>regno>>name>>gender;
}
void disp()
{
cout<<"Register Number: "<<regno<<endl;
cout<<"Name: "<<name<<endl;
cout<<"Gender: "<<gender<<endl;
}
};
int main()
{
    A a;
    B b;
    b.func();
    b.disp();
    
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/6475ec5d-c8f5-456b-98dc-697b9b658810)

## RESULT:
Thus,the C++ program to read regno,name & gender in one class and display the above details in another class using inheritance has been created successfully.


# 3B PROTECTED MEMBERS & OVERRIDING 

## PROGRAM STATEMENT:
Write a program to implement protected member with string.

## ALGORITHM:
1. Define a class with a protected string member name.
2. Create a public method to set the value of name.
3. Inherit the class, and use a method to display the protected member.
4. In main(), create object of derived class and call methods.
5. Display the string and end the program.

## PROGRAM:
```
#include<iostream>
using namespace std;
class A
{
    protected:
    string name;
};
class B:protected A
{
    public:
    void display()
    {
        cin>>name;
        cout<<"The value of n is: "<<name<<endl;
    }
};
int main()
{
    B s;
    s.display();
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ca904253-888b-490d-a818-7952d267f313)

## RESULT:
Thus,the program to implement protected member with string has been created successfully.


# 3C PUBLIC,PRIVATE & PROTECTED INHERITANCE 

## PROGRAM STATEMENT:
Write a C++ program to get two numbers from two base classes and display the quotient in the derived class.

## ALGORITHM:
1. Create two base classes, each with a float number and input method.
2. Define a derived class using multiple inheritance from the two base classes.
3. Add a method in the derived class to calculate and display the quotient.
4. In main(), create an object of the derived class and call input methods.
5. Call the display method to show the result and end the program.

## PROGRAM:
```
#include <iostream>
using namespace std;

class A {
    protected:
    int a;
    public:
    void seta(int x)
{
a=x;
}
};

class B
{
    protected:
    int b;
    public:
    void setb(int y)
    {
        b=y;
    }
};

class C : public A,public B{
    public:
    int c;
    void bit()
    {
        c=a/b;
        cout<<"Product of two numbers = "<<c;
    }
};
  
int main() {
  int x,y;
  C obj;
  cin>>x>>y;
  obj.seta(x);
  obj.setb(y);
  obj.bit();
  return(0);
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/fdf6e846-dbfe-451b-a0b1-7466240700f5)

## RESULT:
Thus,the  C++ program to get two numbers from two base classes and display the quotient in the derived class has been created successfully.



# 3D CONSTRUCTOR & DESTRUCTOR IN DERIVED CLASS

## PROGRAM STATEMENT:
Write a C++ program to pass the integer value to the parameterized constructor of a base class through derived class.

## ALGORITHM:
1. Define a base class with a parameterized constructor.
2. Create a derived class that passes the argument to the base constructor using an initializer list.
3. Add a method in the base class to display the value.
4. In main(), create an object of the derived class and pass an integer.
5. Call the display method and end the program.

## PROGRAM:
```
#include<iostream>
using namespace std;
class Parent
{
    float x;
    public:
    Parent(float i)
    {
        x = i;
        cout <<" The value passed to the base class is "<<x<<endl;
    }     
};
class Child : public Parent
{
    public:
    Child(float x): Parent(x)
    {
        cout<<" The value "<<x<<" is passed through the derived class constructor" <<endl;
    }
};
 int main()
{
    float a;
    cin>>a;
    Child obj1(a);
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/5ce01122-f7c3-4fd5-8641-920b625651a1)

## RESULT:
Thus,the C++ program to pass the integer value to the parameterized constructor of a base class through derived class has been created successfully.




