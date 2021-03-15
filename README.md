# main.c
Exercise 4-1: Write a program to print your name, social security number, and
date of birth.

#include <stdio.h> 
 int main()  
  {
     printf("Name   : Gabriela Canche\n"); 
     printf("Mobile : 99-9999999999\n"); 
     printf("DOB    : June 18, 2002\n"); 
     return(0); 
  }
  
Exercise 4-2: Write a program to print a block E using asterisks (*), where the E
has a height of seven characters and a width of five characters.

#include<stdio.h>
#include<stdlib.h>
int main(void)
{
int i;
for(i=0;i<10;i++)
printf("*");

for(i=0;i<5;i++)
printf("*\n");

for(i=0;i<10;i++)
printf("*");

for(i=0;i<5;i++)
printf("*\n");

for(i=0;i<10;i++)
printf("*");

return 0;
}

Exercise 4-3: Write a program to compute the area and perimeter of a rectangle
with a width of three inches and a height of five inches. What changes must be made
to the program so that it works for a rectangle with a width of 6.8 inches and a
length of 2.3 inches?

/*
* C Program to find perimeter of a rectangle
*/
#include <stdio.h>
#include <conio.h>
 
int main(){
 float length, width, perimeter;
 printf("Enter length of Rectangle\n");
 scanf("%f", &length);
 printf("Enter width of Rectangle\n");
 scanf("%f", &width);
 /* Perimeter of Rectangle = 2 X(Length + Width) */
 perimeter = 2*(length + width);
 printf("Perimeter of Rectangle : %0.4f\n", perimeter);
  
 getch();
 return 0;
}

Exercise 4-4: Write a program to print "HELLO" in big block letters; each letter
should have a height of seven characters and width of five characters.

int problem4_4()
{
    int i;

    for(i=0;i<7;++i)
    {
        if(i==3)
            cout<<"HHHHH\n";
        else
            cout<<"H   H\n";
    }

    for(i=7;i<14;i++)
    {
        if(i==7||i==10||i==13)
            cout<<"EEEEE\n";
        else
            cout<<"E\n";
    }

    return 0;
}

Exercise 4-5: Write a program that deliberately makes the following mistakes:
· Prints a floating-point number using the %d conversion.
[File: twice/twice.c]
#include <stdio.h>

int term;       /* term used in two expressions */
int main()
{
    term = 3 * 5;
    printf("Twice %d is %d\n", term, 2*term);
    printf("Three times %d is %d\n", term, 3*term);
    return (0);
}
· Prints an integer using the %f conversion.

#include <bits/stdc++.h>
using namespace std;
/* Iterative function to reverse digits of num*/
int reversDigits(int num)
{
    int rev_num = 0;
    while (num > 0) {
        rev_num = rev_num * 10 + num % 10;
        num = num / 10;
    }
    return rev_num;
}
 
/*Driver program to test reversDigits*/
int main()
{
    int num = 4562;
    cout << "Reverse of no. is " << reversDigits(num);
    getchar();
    return 0;
}
· Prints a character using the %d conversion.
