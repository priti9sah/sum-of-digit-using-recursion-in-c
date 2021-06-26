# sum-of-digit-using-recursion-in-c
Program in C to find the sum of digits of a number using recursion

#include<stdio.h>
int sum(int x);
int main()
{
	int n,result;
	printf("enter the sum of digits of number=");
	scanf("%d",&n);
	result = sum(n);
	printf("Sum of digit in %d is %d",n,result);
	return 0;
}
int sum(int n)
{
	if(n!=0)
	{
		return (n%10 + sum(n/10));
	}
	else
	{
		return 0;
	}
}
