# stanton
# program structure example

#include <stdio.h>
struct StudentData{ 
char *stu_name; 
char *stu_course; 
int stu_reg; int stu_yearofstudy;
};
int main(){ struct StudentData student; 
student.stu_name = "Sammy";
 student.stu_course= "statistics";
 student.stu_reg = 83048;
 student.stu_yearofstudy = 4;
 printf("Student Name is: %s \n", student.stu_name); 
printf("Student Course is: %s", student.stu_course);
 printf("\nStudent Reg is: %d", student.stu_reg);
 printf("\nStudent Yearofstudy is: %d", student.stu_yearofstudy);
 return 0;
}


# syntax in c example
#include <stdio.h>
int main () 
{
int length, width, area;
length=100;width=14;
area= length * width;
printf("Area is : %d\n",area);
return 0;
}

# Data types
#include <stdio.h>
int main() 
{
// datatypesint a = 10;
char b = 'S';
float c = 2.88;
double d = 28.888;
printf("Integer datatype : %d\n",a);
printf("Character datatype : %c\n",b);
printf("Float datatype : %f\n",c);
printf("Double Float datatype : %lf\n",d);
return 0;
}


# Constants in c
#include <stdio.h>
int main() 
{
const int HEIGHT = 10;
 const int BASE = 5; 
const char NEWLINE = '\n';
 int area;  
 area = (HEIGHT * BASE)/2; 
printf("value of area : %d", area); 
printf("%c", NEWLINE);
 return 0;
}


# variables in c

#include <stdio.h>
// Variable declaration(optional)extern int a, b;
extern int c;
int main () 
{
/* variable definition:*/
int a, b, c;
/* actual initialization*/
a=7;
b=14;
/*using addition operator*/
c= a + b;
/*display the result*/
printf("Sum is : %d\n",c);
return 0;
}

 # Storage in c
include <stdio.h> 

  
/* function declaration */ void func(void); 
  
static int count = 5;   	/* global variable */ 
  main() { 
   while(count--) 
   {       func(); 
   }    return 0; 
} 
/* function definition */ void func( void ) 
{ 
   static int i = 5;   	/* local static variable */    i++; 
   printf("i is %d and count is %d\n", i, count); 
}

 # Operators in c
#include <stdio.h> 
 main() { 
   int a = 21;    int c ; 
    c =  a; 
   printf("Line 1 - =  Operator Example, Value of c = %d\n", c ); 
 
   c +=  a; 
   printf("Line 2 - += Operator Example, Value of c = %d\n", c ); 
 
   c -=  a; 
   printf("Line 3 - -= Operator Example, Value of c = %d\n", c ); 
 
   c *=  a; 
   printf("Line 4 - *= Operator Example, Value of c = %d\n", c );  
   c /=  a; 
   printf("Line 5 - /= Operator Example, Value of c = %d\n", c ); 
 
   c  = 200;    c %=  a; 
   printf("Line 6 - %= Operator Example, Value of c = %d\n", c ); 
 
   c <<=  2; 
   printf("Line 7 - <<= Operator Example, Value of c = %d\n", c ); 
 
   c >>=  2; 
   printf("Line 8 - >>= Operator Example, Value of c = %d\n", c ); 
 
   c &=  2; 
   printf("Line 9 - &= Operator Example, Value of c = %d\n", c ); 
 
   c ^=  2; 
   printf("Line 10 - ^= Operator Example, Value of c = %d\n", c ); 
 
   c |=  2; 
   printf("Line 11 - |= Operator Example, Value of c = %d\n", c );  
} 
