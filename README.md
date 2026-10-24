#include<stdio.h>
int main()
{ int choice;
    printf("Press 1 for Addition: \n ");
    printf("Press 2 for Subtraction: \n ");
    printf("Press 3 for Multiplication: \n ");
    printf("Press 4 for Division: \n ");
    scanf("%d", &choice);
    float a,b;
  printf("Enter two numbers");
  scanf("%f %f", &a, &b);
  switch(choice)
    {
        case 1:
        printf("Addition=%f", a+b);
        break;
        case 2:
        printf("Subtraction=%f", a-b);
        break;
        case 3:
        printf("Multiplication=%f", a*b);
        break;
        case 4:
        if(b!=0)
            printf("Division=%f", a/b);
        else
            printf("Division by zero is not allowed.");
        break;
        default:
        printf("Invalid choice");
    }
}
