#include <iostream>
using namespace std;

// Hàm hoán vị sử dụng con trỏ
void hoanVi(float* x, float* y) {
    float temp = *x;
    *x = *y;
    *y = temp;
}

int main() {
    float a, b;

    // Nhập hai số thực
    cout << "Nhap so thuc a: ";
    cin >> a;
    cout << "Nhap so thuc b: ";
    cin >> b;

    // In ra trước khi hoán vị
    cout << "Truoc khi hoan vi: a = " << a << ", b = " << b << endl;

    // Gọi hàm hoán vị
    hoanVi(&a, &b);

    // In ra sau khi hoán vị
    cout << "Sau khi hoan vi: a = " << a << ", b = " << b << endl;

    return 0;
}
