# sorting-programs.-
#bubble_sort:
#include<stdio.h>
int main()
{
     int n,a[100],i,j,temp;
     scanf("%d",&n); 

     for(i=0; i<n; i++)
     {
         scanf("%d",&a[i]);
     }

     for(i=0;i<n-1;i++) 
     {
         for(j=0;j<(n-i-1);j++)
         {
             if(a[j]>a[j+1])
             {
                 temp=a[j];
                 a[j]=a[j+1];
                 a[j+1]=temp;
             }
         }
     }
     for(i=0;i<n;i++)
    {
        printf("%d",a[i]);
    }
 
 }       
Output:
5
15 16 6 8 5
5 6 8 15 16 //sorted_array
#selection_sort:
#include<stdio.h>
int main()
{
     int n,a[100],i,j,temp,min;
     scanf("%d",&n); 

     for(i=0; i<n; i++)
     {
         scanf("%d",&a[i]);
     }

     for(i=0;i<n-1;i++) 
     {
         min=i;
         for(j=i+1;j<n;j++)
         {
             if(a[j]<a[min])
             {
                 min=j;
             }
             temp=a[min];
             a[min]=a[i];
             a[i]=temp;
         }
     }
     for(i=0;i<n;i++)
    {
        printf("%d",a[i]);
    }
 
 }       
Output:
6
7 4 10 8 3 1
1 3 4 7 8 10 //sorted_array
#insertion_sort:

        #include<stdio.h>
int main()
{
     int n,a[100],i,j,temp;
     scanf("%d",&n); 

     for(i=0; i<n; i++)
     {
         scanf("%d",&a[i]);
     }

     for(i=0;i<=n-1;i++) 
     {
         temp=a[i];
         j=i;
         while(a[j-1]>temp && j>=1)
        {
            a[j]=a[j-1];
            j--;
        }
        a[j]=temp;    
     }
     for(i=0;i<n;i++)
     {
        printf("%d",a[i]);
     }
 
 }       
Output:
6
5 4 10 1 6 2
1 2 4 5 6 10 //sorted_array
   
