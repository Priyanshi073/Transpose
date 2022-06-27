//Matrix Transpose
#include <stdio.h> 
void main() 
   
  { 
  int x1[50][50],y1[50][50],i,j,r,c; 
       printf("\n\nTranspose of a Matrix :\n"); 
       printf("---------------------------\n");  
       printf("\nInput the rows and columns of the matrix : "); 
       scanf("%d %d",&r,&c); 
       printf("Input elements in the first matrix :\n"); 
       for(i=0;i<r;i++) 
        { 
            for(j=0;j<c;j++) 
            { 
	           printf("element - [%d],[%d] : ",i,j); 
	           scanf("%d",&x1[i][j]); 
            } 
        }  
	 printf("\nThe matrix is :\n"); 
  		for(i=0;i<r;i++) 

    		{ 
      		printf("\n"); 
      		for(j=0;j<c;j++) 
          	printf("%d\t",x1[i][j]); 
    		} 
  for(i=0;i<r;i++) 
     { 
      for(j=0;j<c;j++) 
            { 
                   y1[j][i]=x1[i][j]; 
            } 
      } 
      printf("\n\nThe transpose of a matrix is : "); 
      for(i=0;i<c;i++){ 
      printf("\n"); 
      for(j=0;j<r;j++){ 
           printf("%d\t",y1[i][j]); 
      } 
  } 
      printf("\n\n"); 
} 
