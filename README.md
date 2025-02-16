#include<stdio.h>
void main(){
    float pin,choice,credit,debit,balance=30000;
    printf("ENTER A PIN:");
    scanf("%f",&pin);
    if(pin==7337){
        printf("WELCOME TO OUR ATM");
        printf("\nOptions;");
        printf("\n 1.Balance \n 2.Credit \n 3.Debit");
        printf("\nEnter a Option :");
        scanf("%f",&choice);
        }
    if(choice==1){
        printf("Your currrent balances is %f",balance);
    }
    else if(choice==2){
        printf("Enter a amount:");
        scanf("%f",&credit);
        printf("%f",balance+credit);
    }
    else if(choice==3){
        printf("Enter a amount:");
        scanf("%f",&debit);
        if(debit>=500){
        printf("%f",balance-debit);
        }
        else {
            printf("Enter amount morethan 500");
        }
    }    
    else{
        printf("Invalid pin");
        }
        printf("\n\nThank you!visit again");
}
