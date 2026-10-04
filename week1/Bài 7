#include <iostream>
#include <vector>

using namespace std;

long long tinhTongMang(const vector<vector<int>>& a) {
    long long sum = 0;
    for (int i = 0; i < a.size(); i++) {
        for (int j = 0; j < a[i].size(); j++) {
            sum += a[i][j];
        }
    }
    return sum;
}

void xoaDong(vector<vector<int>>& a, int rowIndex) {
    if (rowIndex < 0 || rowIndex >= a.size()) {
        cout << "Vi tri dong khong hop le!" << endl;
        return;
    }
    a.erase(a.begin() + rowIndex);
}

void inMang2Chieu(const vector<vector<int>>& a) {
    for (int i = 0; i < a.size(); i++) {
        for (int j = 0; j < a[i].size(); j++) {
            cout << a[i][j] << " ";
        }
        cout << endl;
    }
}

int main() {
    int n, m;
    cout << "Nhap kich thuoc N x M: ";
    cin >> n >> m;

    vector<vector<int>> a(n, vector<int>(m));
    cout << "Nhap cac phan tu cua mang 2 chieu:\n";
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < m; j++) {
            cin >> a[i][j];
        }
    }

    cout << "Tong cac phan tu trong mang 2 chieu: " << tinhTongMang(a) << endl;

    int rowIndex;
    cout << "Nhap chi so dong i can xoa (0-indexed): ";
    cin >> rowIndex;
    xoaDong(a, rowIndex);

    cout << "Mang 2 chieu sau khi xoa dong " << rowIndex << ":\n";
    inMang2Chieu(a);

    return 0;
}
// Time N*M
// Memory N*M
