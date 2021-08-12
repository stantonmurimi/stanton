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
