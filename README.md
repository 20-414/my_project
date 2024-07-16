#include"myheader.h"

STUDENT * AddFirst(STUDENT *head)
{
	STUDENT *newnode=NULL;
	newnode=malloc(sizeof(STUDENT));
	if(newnode==NULL)
	{
		printf("Node not created\n");
	}
	else
	{
		printf("enter the roll\n");
		scanf("%d",&newnode->roll);
		printf("enter the name\n");
		scanf("%s",newnode->name); 
    printf("enter the marks\n");
    scanf("%d",&newnode->marks\n);
		newnode->link=NULL;

		newnode->link=head;
		head=newnode;
	}
	return head;

}
