#include <stdio.h>

float balance = 1000.0; // Initial hardcoded balance

void checkBalance() {
    printf("Your current balance is: Rs. %.2f\n", balance);
}

void depositMoney() {
    float amount;
    printf("Enter amount to deposit: Rs. ");
    scanf("%f", &amount);
    if (amount > 0) {
        balance += amount;
        printf("Amount deposited successfully.\n");
    } else {
        printf("Invalid deposit amount.\n");
    }
}

void withdrawMoney() {
    float amount;
    printf("Enter amount to withdraw: Rs. ");
    scanf("%f", &amount);
    if (amount > 0 && amount <= balance) {
        balance -= amount;
        printf("Amount withdrawn successfully.\n");
    } else {
        printf("Invalid or insufficient balance.\n");
    }
}

int main() {
    int choice;
    do {
        printf("\n===== ATM Menu =====\n");
        printf("1. Check Balance\n");
        printf("2. Deposit Money\n");
        printf("3. Withdraw Money\n");
        printf("4. Exit\n");
        printf("Choose an option: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1:
                checkBalance();
                break;
            case 2:
                depositMoney();
                break;
            case 3:
                withdrawMoney();
                break;
            case 4:
                printf("Thank you for using the ATM!\n");
                break;
            default:
                printf("Invalid choice. Try again.\n");
        }
    } while (choice != 4);

    return 0;
}
