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

 # Decision making
#include <stdio.h> 

  int main () 
{ 
   /* local variable definition */    int a = 100;    int b = 200; 
  
   switch(a) {       case 100:  
         printf("This is part of outer switch\n", a );          switch(b) {             case 200: 
               printf("This is part of inner switch\n", a ); 
         }    } 
   printf("Exact value of a is : %d\n", a );    printf("Exact value of b is : %d\n", b ); 
  
   return 0; 
}

# loops in c
#include <stdio.h> 

  int main () 
{ 
   /* local variable definition */    int i, j; 
    
   for(i=2; i<100; i++) {       for(j=2; j <= (i/j); j++) 
        if(!(i%j)) break;   	// if factor found, not prime       if(j > (i/j)) printf("%d is prime\n", i); 
   } 
  
   return 0; 
}

Do while
#include <stdio.h> 
  int main () 
{ 
   /* local variable definition */    int a = 10; 
 
   /* do loop execution */    do    { 
       printf("value of a: %d\n", a);        a = a + 1; 
   }while( a < 20 ); 
  
   return 0; 
} 

# Scope rule
#include <stdio.h> 
  
/* global variable declaration */ int a = 20; 
  int main () 
{ 
  /* local variable declaration in main function */   int a = 10;   int b = 20;   int c = 0; 
 
  printf ("value of a in main() = %d\n",  a);   c = sum( a, b); 
  printf ("value of c in main() = %d\n",  c); 
 
  return 0; 
} 
 
/* function to add two integers */ int sum(int a, int b) 
{ 
    printf ("value of a in sum() = %d\n",  a);     printf ("value of b in sum() = %d\n",  b); 
 
    return a + b; 
} 

# Arrays in C
#include <stdio.h> 

  int main () 
{ 
   /* an array with 5 rows and 2 columns*/ 
   int a[5][2] = { {0,0}, {1,2}, {2,4}, {3,6},{4,8}};    int i, j; 
  
   /* output each array element's value */    for ( i = 0; i < 5; i++ ) 
   { 
      for ( j = 0; j < 2; j++ ) 
      { 
         printf("a[%d][%d] = %d\n", i,j, a[i][j] ); 
      }    }    return 0; 
} 

ACCESSING ARRAYS
#include <stdio.h> 
  int main () 
{ 
   int n[ 10 ]; /* n is an array of 10 integers */    int i,j; 
  
   /* initialize elements of array n to 0 */             for ( i = 0; i < 10; i++ ) 
   { 
      n[ i ] = i + 100;  	/* set element at location i to i + 100 */ 
   } 
    
   /* output each array element's value */    for (j = 0; j < 10; j++ ) 
   { 
      printf("Element[%d] = %d\n", j, n[j] ); 
   }   
   return 0; 
} 

