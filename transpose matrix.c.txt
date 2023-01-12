#include <stdio.>
int main()
{
//WAP to transpose rows of an array into columns
    int m,n,i,j; 
    printf("enter the number of rows and columns of the array\n");//m- denotes no. of rows & n-denotes no. of columns
    scanf("%d%d",&m,&n);
    int arr1[m][n],arr2[n][m];
    printf("input the values of array\n");
    for(i=0;i<m;i++)
    {
        for(j=0;j<n;j++)
        scanf("%d",&arr1[i][j]);
    }
    printf("array formed before transpose:\n");
    for(i=0;i<m;i++)
    {
        for(j=0;j<n;j++)
         printf("%d ",arr1[i][j]);
         printf("\n");
    }
     for(i=0;i<m;i++)
    {
        for(j=0;j<n;j++)
       arr2[j][i]=arr1[i][j];
    }
    printf("array formed after transpose:\n");
    for(i=0;i<n;i++)
    {
        for(j=0;j<m;j++)
         printf("%d ",arr2[i][j]);
         printf("\n");
    }
return 0;
}