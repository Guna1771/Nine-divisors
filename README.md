# Nine-divisors
Find the number of integers with exactly 9 divisors
#include<stdio.h>
int main()
{
int n,count=0;
printf(“\nEnter the number : “);
scanf(“%d”, &n);
printf(“\nThe number which has exactly 9 divisors : “);
for (int i = 1; i <= n; i++)
{
int c = 0;
for (int j = 1; j <= i j++)
{
if (i % j == 0)
c = c + 1;
}
if (c == 9)
{
printf(“%d “, i);
count = count + 1;
}
}
printf(“\n\nTotal = %d\n”, count);
return 0;
}

