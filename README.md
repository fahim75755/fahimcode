#include <stdio.h>
#include <stdlib.h>
int main() {
    int i,j,mat1[10][10],mat2[10][10],mat3[10][10], row1,col1,row2,col2;
    //kk
    printf("number of rows in mat1 ");
    scanf("%d", &row1);
    printf("number of col in mat1 ");
    scanf("%d", &col1);
    printf("number of rows in mat2 ");
    scanf("%d", &row2);
    printf("number of col in mat2 ");
    scanf("%d", &col2);
    
if(row1 !=row2 || col1 != col2){
printf("ORDER OF TWO MATRICES ARE NOT SAME ");
exit(0);
}
for(i=0;i<row1;i++){
    for(j=0;j<col1;j++){
        printf("enter the elements for mat1 [%d][%d]", i,j);
        scanf("%d",&mat1[i][j]);
    }
}
for(i=0;i<row2;i++){
    for(j=0;j<col2;j++){
        printf("enter the elements for mat2[ %d][%d]",i,j);
        scanf("%d", &mat2[i][j]);
    }
}
for (i = 0; i < row1; i++){
for (j = 0; j < col1; j++) {
    mat3[i][j]=mat1[i][j]+mat2[i][j];
}
}
for (i = 0; i < row1; i++) {
for (j = 0; j < col1; j++) {
printf("%d ", mat3[i][j]); 
}
printf("\n");
}
}
