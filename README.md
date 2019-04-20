# voting-system
#include<conio.h>
#include<stdio.h>
void main()
{
	int n,ch,count=0,county=0,i;
	char ans;
	printf("enter total candidate");
	scanf("%d",&n);
	
	
	for(i=0;i<n;i++)
	{
		printf("PRESS 1 FOR BJP");
		printf("PRESS 2 FOR TMC");
		scanf("%d",&ch);	
		//for(int i=0;i<n;i++)
			
		switch(ch)
		{
			case 1:
				count++;
				break;
			case 2:
				county++;
				break;
			case 3:		
				out(count);
				outp(county);
				break;
			default:
				printf("Choose correcte option!!!!");
				
		}
		printf("\nDo you want to stop voting (y)?\n");
		scanf("%c",&ans);
		if(ans=='y')break;
	}
}
int out(count)
{
		printf("BJP VOTE = %d",count);
//		printf("\nTMC VOTE IS =%d",county);
}
int outp(yu)
{
//		printf("BJP VOTE = %d",count);
		printf("\nTMC VOTE IS =%d",yu);
}

