#include<stdio.h>
#include<conio.h>
#include<string.h>


struct org
{
char name[30];
double emp_id,salary,num;

};
int main()
{


struct org employee[20];
int n,i;

printf("\nEnter the number of employeed in your organization(<=20):");
scanf("%d",&n);


for(i=0;i<n;i++)
{
printf("\nEnter Person %d\n Name :",i+1);
scanf("%s",&employee[i].name);
printf("\nAge :");
scanf("%d",&employee[i].emp_id);
printf("\n Phone Number :");
scanf("%d",&employee[i].num);
printf("\nEmployee Salary :");
scanf("%d",&employee[i].salary);
}


printf("\nEmployees Information\n");
for(i=0;i<n;i++)
{
printf("\nPerson %d\n Name : %s",i+1,employee[i].name);
printf("\nAge: %d",employee[i].emp_id);

printf("\nPhone Number: %d",employee[i].num);
printf("\nEmployee Salary : %d",employee[i].salary);
}
getch();
}
