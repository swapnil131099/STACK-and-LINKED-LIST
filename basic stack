// stack
// the basic structure of a stack
#include<stdio.h>
#include<stdlib.h>
#define max 10
int stackarr[max]; 
int top=-1;
void push(int item);
int pop();
int peek();
int empty();
int full();
void display();
main()
{
	int choice, item;
	while(1)
	{
		printf("1.Push\n");
		printf("2.Pop\n");
		printf("3.Display the top element\n");
		printf("4.Display the stack element\n");
		printf("5.Quit\n");
		printf("Enter your choice");
		scanf("%d",&choice);
		switch(choice)
		{
			case 1: 
				printf("Enter the item to be pushed: ");
				scanf("%d",&item);
				push(item);
				break;
			case 2:
				item = pop();
				printf("Poped item is %d",item);
				break;
			case 3:
			
				printf("Item at the top is %d",peek());
				break;
			case 4:
				display();
				exit(1);
			default:
				printf("Wrong choice.!!!");
		}
	}
}
void push(int item)
{
	if(full())
	{
		printf("Stack overflow");
		return;
	}
	top = top+1;
	stackarr[top]=item;
}
int pop()
{
	int item;
	if(empty())
	{
		printf("Stack underflow");
		exit(1);
	}
	item =stackarr[top];
	top=top-1;
	return item;
}
int peek()
{
	if(empty())
	{
		printf("stack underflow");
		exit(1);
	}
	return stackarr[top];
}
int empty()
{
	if(top==-1)
	{
		return 1;
	}
	else
	{
		return 0;
	}
}
int full()
{
	if(top==max-1)
	{
		return 1;
	}
	else
	{
		return 0;
	}
}
void display()
{
	int i;
	if(empty())
	{
		printf("Stack is empty");
		return;
	}
	printf("Stack element: ");
	for(i=top; i>=0; i--)
	{
		printf("%d",stackarr[i]);
	}
	printf("\n");
}
