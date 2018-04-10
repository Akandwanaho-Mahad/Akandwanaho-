The following are the solutions to the assignment questions.
Question 1;

#include <stdio.h>
int x=1;
int main()
{
    if (x==1){
    printf("x equals 1");
    } else{
    printf("x does not equal 1");
    }

    return 0;
}

Question 2;
i)  float do_it(char a,char b,char c);
ii) void print_a_number( int a);
iii) whats wrong with the program?
answer: - When calling the function, the sentence "This is a message to print" is not supposed to be there ie it brings in more arguments.
        - also
  
Question 3;
i)  long b[50]; 
ii)b[49]=123.456;
iii) The values of x are 0,1,2,3,......99
iv) THe values of ctr are 2,5,8.
v) while(ctr<=100){
   printf("ctr is %d\n",ctr);
   ctr+=3;}
vi) the problem is that the for loop is not supposed to be terminated.

Question 4;
#include <stdio.h>
#include <conio.h>
void addarrays( int a[10],int b[10]);
int main()
{

    int a[10]={1,2,3,4,5,6,7,8,9,10};
    int b[10]={1,2,3,4,5,6,7,8,9,10};



  addarrays(a,b);
    getch();
}
void addarrays( int a[10],int b[10]){

int c[10];

int i;
for(i=0;i<10;i++){

c[i]=b[i]+a[i];
printf("The sum of b[%d] and a[%d] is %d\n",i,i,c[i]);
int *ptr;
ptr=&c[i];
printf("The address is %x\n",ptr);

}
    printf("\nThe Three arrays are:\n\n");
    printf("The first array is [");
   for(i=0;i<10;i++){
    printf("%d,",a[i]);}
    printf("]");
    printf("\nThe second array is [");
    for(i=0;i<10;i++){
    printf("%d, ",b[i]);}
    printf("]");
    printf("\nThe array of the sums is [");
    for(i=0;i<10;i++){
    printf("%d, ",c[i]);}
    printf("]");

return 0;
}

