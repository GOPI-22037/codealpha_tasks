#include <iostream>
using namespace std;

class BankAccount {
    string name;
    int accountNumber;
    float balance;

public:
    BankAccount(string n, int acc) {
        name = n;
        accountNumber = acc;
        balance = 0;
    }

    void deposit(float amount) {
        balance += amount;
        cout << "Deposited ₹" << amount << endl;
    }

    void withdraw(float amount) {
        if (amount > balance) {
            cout << "Insufficient balance!\n";
        } else {
            balance -= amount;
            cout << "Withdrew ₹" << amount << endl;
        }
    }

    void checkBalance() {
        cout << "Current balance: ₹" << balance << endl;
    }
};

int main() {
    BankAccount acc("Gopika", 12345);
    int choice;
    float amount;

    do {
        cout << "\n1. Deposit\n2. Withdraw\n3. Check Balance\n4. Exit\nEnter choice: ";
        cin >> choice;

        switch (choice) {
            case 1:
                cout << "Enter amount to deposit: ";
                cin >> amount;
                acc.deposit(amount);
                break;
            case 2:
                cout << "Enter amount to withdraw: ";
                cin >> amount;
                acc.withdraw(amount);
                break;
            case 3:
                acc.checkBalance();
                break;
            case 4:
                cout << "Exiting...\n";
                break;
            default:
                cout << "Invalid choice!\n";
        }
    } while (choice != 4);

    return 0;
}
