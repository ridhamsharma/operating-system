#include<stdio.h>
#include<conio.h>
int main()
{
	printf("\t\t\t\t\t*****************************************************\n");
	printf("\t\t\t\t\t****\t\tWELCOME TO MY PROGRAM\t\t ****\n");
	printf("\t\t\t\t\t*****************************************************\n");
	//Here I take n_process = Q = Number of processes
	//And n_resources = P = Number of Resourses
	//And smax = summation of all maximum
	printf("\n\n\t\t\t\t    CHECK YOUR SYSTEM WHETHER IT IS IN SAFE STATE OR IN DEADLOCK");
	printf("\n\t\t\t\t____________________________________________________________________\n\n");
int n_process,n_resources,smax,sflag=0;
int i=0,j,flag[10],n=0,kill=0,sum=0,available=0;
int a[10];
int max[10],alloc[10],need[10];
printf("Enter the number of processes:"); 
scanf("%d",&n_process);
printf("Enter the number of resources:");
scanf("%d",&n_resources);
smax=n_resources+n_process;

for(i=0;i<n_process;i++)
{
//sum of all max[i]<n_resources+n_process;
if(i==0)
{
max[i]=n_resources-1;//random value which statisfies 2 conditions
}
else
{
max[i]=1;
}
}

//allocate resources to processes
for(i=0;i<n_process;i++)
{
if(i==0)
{
alloc[i]=n_resources-2; 
}
else
{alloc[i]=0;}
}

for(i=0;i<n_process;i++)
{
sum=alloc[i]+sum;
}
available=n_process-sum;

for(i=0;i<n_process;i++)
{
need[i]=max[i]-alloc[i];
}

while(n<=n_process)
{
for(i=0;i<n_process;i++)
{
if(need[i]<available)
{
available=available+need[i];
flag[i]=1;
n=n+1;
}

else
{flag[i]=0;}
}
for(i=0;i<n_process;i++)
{
if(flag[i]==1)
sflag=sflag+1;
}
if(sflag==0)
{
n=n_process+1;
kill=1;
}
}

if(kill==1){printf("\n\t\tDeadlock occured in System");}

else
{
	printf("\n\t\tSystem are in Safe State");
}
}
