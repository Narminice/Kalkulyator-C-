# Kalkulyator-C-
#include <iostream>
using namespace std;

int main() {
    double sayi1, sayi2;
    char emeliyyat;

    cout << "Birinci eded: ";
    cin >> sayi1;
    cout << "Emeliyyat (+, -, *, /): ";
    cin >> emeliyyat;
    cout << "Ikinci eded: ";
    cin >> sayi2;

    switch (emeliyyat) {
        case '+':
            cout << "Netice: " << sayi1 + sayi2 << endl;
            break;
        case '-':
            cout << "Netice: " << sayi1 - sayi2 << endl;
            break;
        case '*':
            cout << "Netice: " << sayi1 * sayi2 << endl;
            break;
        case '/':
            if (sayi2 != 0)
                cout << "Netice: " << sayi1 / sayi2 << endl;
            else
                cout << "Xeta: Sifira bolmek olmaz!" << endl;
            break;
        default:
            cout << "Xeta: Yanlish emeliyyat!" << endl;
    }

    return 0;
}
