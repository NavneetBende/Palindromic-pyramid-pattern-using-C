Palindromic pyramid pattern
The palindromic number are the number whose reverse is equal to the original number.

For example- 12321 is a original number whose reverse is same as the original number, that is 12321

So, here we learn how to print the pyramid pattern on palindromic number or word.

palindromic pattren
1. Write a program to print the following pattern.
Enter the row 5

    1
   121
  12321
 1234321
123454321
Working
Step 1- Initialize the there variable for the loop

Step 2- the first loop is for the the row, in how many row you want to print data.

Step 3- the second loop is for the spaces, the space print in the row from i to row-1.

Step 4- the third loop is for the the print element from i to row.

Step 5- print j.

Step 6. the forth loop is for print reverse number.

Step 7- print j.

Step 8. Stop.

C	JAVA
#include <stdio.h>  
int main()  
{
    int n, i, j;
    printf("Enter number of rows : ");
    scanf("%d",&n);
    for(i=1; i<=n; i++)
    {
        for(j=i; j<=n; j++)
        {
            printf(" ");
        }
        for(j=1; j<=i; j++)
        {
            printf("%d",j);
        }
        for(j=i-1; j>=1; j--)
        {
            printf("%d",j);
        }
        printf("\n");
    }
    return 0;
}  
2. Write a program to print the following pattern
Enter the row 5                                                                                                             

     A                                                                                                                     
    ABA                                                                                                                    
   ABCBA                                                                                                                   
  ABCDCBA                                                                                                                  
 ABCDEDCBA  
C	JAVA
#include <stdio.h>  
int main()  
{
    int n, i, j;
    printf("Enter number of rows : ");
    scanf("%d",&n);
    for(i=1; i<=n; i++)
    {
        for(j=i; j<=n; j++)
        {
            printf(" ");
        }
        for(j=1; j<=i; j++)
        {
            printf("%c",j+64);
        }
        for(j=i-1; j>=1; j--)
        {
            printf("%c",j+64);
        }
        printf("\n");
    }
    return 0;
}  
