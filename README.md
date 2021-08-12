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

Data types
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


Constants in c
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
