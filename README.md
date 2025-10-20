# Program-6-e
## C-Module 6
## EX_NO-06)e)-User Defined Datatype
### Date: 19-10-2025
### Name: Anish D
### Register Number:25010086
## AIM:
Create a structure for Electricity Bill calculation using function-Passing structure to a function by address(reference)(use service no, name, previous reading, current reading, unit consumption & amount as data members).
## ALGORITHM:
1. Start the program.
2. Define a structure named eb with four members: 

     a. no (integer for service number)  

     b. name (character array of size 20)  

    c. unit1 (integer for previous reading)  

    d. unit2 (integer for current reading)  

3. Declare a variable of type struct eb.
4. Read the service number, name, previous reading, and current reading from the user using scanf.
5. Calculate the units consumed: un = unit1 - unit2.
6. Declare an integer variable amt to store the bill amount and initialize it to 0.
7. Calculate the amount based on units consumed:

   a. If un ≤ 100, amt = un * 2.  
 
    b. If un > 100 and ≤ 300, amt = (100*2) + ((un-100)*3).  

   c. If un > 300, amt = (100*2) + (200*3) + ((un-300)*5).  
8. Print the service number, service name, unit consumption, and amount in a formatted manner using printf.
9. End the program.
## PROGRAM:
```
#include<stdio.h>
struct eb
{
    int no,unit1,unit2;
    char name[20];
};
int main()
{
    struct eb s;
    scanf("%d%s%d%d",&s.no,s.name,&s.unit1,&s.unit2);
    int un=s.unit1-s.unit2;
    int amt=0;
    if(un<=100)
    amt=un*20;
    else if(un<=300)
    amt=(100*2)+((un-100)*3);
    else
    amt=(100*2)+(200*3)+((un-300)*5);
    printf("service number:%d\nservice name:%s\nunit consumption:%d\namount:%d.00",s.no,s.name,un,amt);
}
```
## OUTPUT:
<img width="834" height="481" alt="Screenshot 2025-10-20 095113" src="https://github.com/user-attachments/assets/7198b42d-6c01-4ba6-b182-094e4dc4868b" />

## RESULT:
Thus the program to structure for Electricity Bill calculation using function-Passing structure to a function by address(reference)(use service no, name, previous reading, current reading, unit consumption & amount as data members) has been executed successfully
