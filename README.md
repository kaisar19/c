#include<stdio.h>
int main()
{
    int a[10][10],transpose[10][10],row,col,i,j;
    printf("Enter the row and col:\n");
    scanf("%d %d",&row, &col);
    //scanning array
    for(i=0; i<row; i++)
    {
        for(j=0; j<col; j++)
        {
            printf("a[%d][%d]=",i,j);
            scanf("%d",&a[i][j]);
        }
    }

    //transpose array
    printf("Elements of array a :\n");
    for(i=0; i<row; i++)
    {
        for(j=0; j<col; j++)
        {

    transpose[j][i]=a[i][j];

        }
    }
    //printing array A
     printf("array a :\n");
    for(i=0; i<row; i++)
    {
        for(j=0; j<col; j++)
        {
            printf("%d ",a[i][j]);
        }
        printf("\n");
    }
 //transpose array printing
  printf("Elements of transpose matrix :\n");
    for(i=0; i<col; i++)
    {
        for(j=0; j<row; j++)
        {
            printf("%d ",transpose[i][j]);
        }
        printf("\n");
    }






}
