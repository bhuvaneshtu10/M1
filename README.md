
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
    #include<stdio.h>
    int main()
    {
    char a,b,c;
    printf("Enter three characters\n");
    scanf(" %c %c %c", &a, &b, &c);
    printf("REVERSE ORDER:\n%c %c %c",c,b,a);
    return 0;
    }

## OUTPUT:

![image](https://github.com/user-attachments/assets/be0206d0-ab04-412a-bd3a-450c90a53a75)

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
    #include<stdio.h>
    int main()
    {
    int a; 
     scanf("%d",&a);
     if(a>0)
    {
	printf("It is a positive number");
    }
    else
    {
	printf("It is not a positive number");
    }
    }

# OUTPUT:

![image](https://github.com/user-attachments/assets/5240ceec-3add-4c27-8c3a-aefb28b2056f)

![image](https://github.com/user-attachments/assets/8136d266-8a31-4fa8-b3bc-2f3e57ac6fd3)

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
    #include<stdio.h>
    int main()
    {
    int n1,d1,n2,d2;
    float f1,f2,res;
    printf("FIRST FRACTION:\n");
    scanf("%d%d",&n1,&d1);
    printf("SECOND FRACTION:\n");
    scanf("%d%d",&n2,&d2);
    f1=(float)n1/d1;
    f2=(float)n2/d2;
    res=(f1 < f2) ? f1 : f2;
    printf("The minimum value is: %.2f\n",res);
    return 0;
    }
## OUTPUT:

![image](https://github.com/user-attachments/assets/fe0eb760-9d95-4768-b786-5e8c98dbea91)

## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
    #include<stdio.h>
    int main()
    {
    int a;
    scanf("%d",&a);
    if(a==1)
    {
	printf("It is equal to 1");
    }
    else
    {
	printf("It is not equal to 1");
    }
    }
## OUTPUT:

![image](https://github.com/user-attachments/assets/7199eb0e-c63e-4d1e-83c2-6eb0e9a48fa1)

![image](https://github.com/user-attachments/assets/34d8be6d-4cdd-4611-9015-c762e98951fb)

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
    #include<stdio.h>
    int main()
    {
    int m1,m2,m3;
    float tot,per;
    printf("Enter marks:\n");
    scanf("%d%d%d",&m1,&m2,&m3);
    tot=m1+m2+m3;
    per=tot/3;
    printf("Total Marks = %.2f\n",tot);
    printf("Percentage = %.2f%%\n",per);
    if(m1>=40&&m2>=40&&m3>=40) 
    {
    if(per>=60) 
	{
        printf("Division = First\n");
    }
    else if(per>=48)
	 {
        printf("Division = Second\n");
    }
    else if(per>=36)
	{
        printf("Division = Pass\n");
    }
    }
    else 
    {
    printf("Division = Fail\n");
    }
    return 0;
    }

## OUTPUT:

![image](https://github.com/user-attachments/assets/07607bf5-4107-4411-8992-d8192d5c23fc)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

