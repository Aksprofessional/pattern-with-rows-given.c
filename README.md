# pattern-with-rows-given.c
//  C program to print pattern with given rows // example enter no. of rows=6  enter rows=7 A            A AB          BA ABC        CBA ABCD      DCBA ABCDE    EDCBA ABCDEF  FEDCBA ABCDEFGGFEDCBA 
//  C program to print pattern with given rows
// example enter no. of rows=6

enter rows=7
A            A
AB          BA
ABC        CBA
ABCD      DCBA
ABCDE    EDCBA
ABCDEF  FEDCBA
ABCDEFGGFEDCBA

#include <stdio.h>
int main() {
    int i,j,n;
    printf("enter rows=");
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        for(j=0;j<=i;j++)
         printf("%c",65+j);
        for(j=0;j<=(n-2)-i;j++)
         printf(" ");
         for(j=0;j<=(n-2)-i;j++)
         printf(" ");
        for(j=i;j>=0;j--)
         printf("%c",65+j);
        printf("\n");
    }
    return 0;
}
