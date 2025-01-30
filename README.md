Diamond number pattern printing
In this section, we learn about  Diamond numbers pattern printing. Here we will see how to use loops to print the numbers starting from 1 up to N in the form of diamond. the diamond will be made using two triangles one triangle will be printed by one loop and other by another loop.  Both the triangles in Diamond numbers pattern printing are opposite from each other that why we need to take two loop for print diamond pattern. 

diamond number pattern
1. Write a program to print the following pattern
Enter the number of row 5

    1
   123
  12345
 1234567
123456789
 1234567
  12345
   123
    1
Working
Step 1- Initialize first outer loop for the print the first pyramid, this loop work from 1 to row.

Step 2- Now we need two loop inside the outer loop .

Step 3- The first inner loop work on printing space, so this loop work from 1 to n-i, because we need to reduce space after every row.

Step 4- The second inner loop work on the printing number, so it will start from 1 to 2*i-1, because we need to increment number with 2 in every row.

Step 5- Now initialize second outer loop which is work for the second opposite pyramid.this loop start from row-1 to 1

Step 6 – The inner loop of the second pyramid work same as the first outer loop.

Step 7- Stop. 

 

C	JAVA	Python
#include <stdio.h>  
int main()  
{
    int n, i, j;
    printf("Enter number of rows : ");
    scanf("%d",&n);
    for(i=1; i<=n; i++)
    {
        for(j=1;j<=n-i;j++)
        {
            printf(" ");
        }
        for(j=1;j<=i*2-1;j++)
        {
            printf("%d",j);
        }
        printf("\n");  
    }
    for(i=n-1;i>0;i--)
    {
        for(j=1;j<=n-i;j++)
        {
            printf(" ");
        }
        for(j=1;j<=i*2-1;j++)
        {
            printf("%d",j);
        }
        printf("\n");
    }
    return 0;
}  
2. Write a program to print the following pattern
Enter the number of row 5

    1
   222
  33333
 4444444
555555555
 4444444
  33333
   222
    1
C	JAVA	Python
#include <stdio.h>  
int main()  
{
    int n, i, j;
    printf("Enter number of rows : ");
    scanf("%d",&n);
    for(i=1; i<=n; i++)
    {
        for(j=1;j<=n-i;j++)
        {
            printf(" ");
        }
        for(j=1;j<=i*2-1;j++)
        {
            printf("%d",i);
        }
        printf("\n");  
    }
    for(i=n-1;i>0;i--)
    {
        for(j=1;j<=n-i;j++)
        {
            printf(" ");
        }
        for(j=1;j<=i*2-1;j++)
        {
            printf("%d",i);
        }
        printf("\n");
    }
    return 0;
}  
