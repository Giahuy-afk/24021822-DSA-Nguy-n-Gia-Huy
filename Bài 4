#include <iostream>

using namespace std;


long long UCLN(long long x, long long y) {
    x = abs(x);
    y = abs(y);
    while (y != 0) {
        long long r = x % y;
        x = y;
        y = r;
    }
    return x;
}


void rutGonPhanSo(long long a, long long b) {
    if (b == 0) {
        cout << "Mau so phai khac 0!" << endl;
        return;
    }

    long long ucln = UCLN(a, b);
    a /= ucln;
    b /= ucln;

   
    if (b < 0) {
        a = -a;
        b = -b;
    }

    cout << "Phan so sau khi rut gon: " << a << "/" << b << endl;
}

int main() {
    long long a, b;
    cout << "Nhap tu so a va mau so b: ";
    cin >> a >> b;

    rutGonPhanSo(a, b);

    return 0;
}
// Time logN
// Memory 1
