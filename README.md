#include <iostream>
#include <math.h>
using namespace std;

int main()
{
    double Nam;
    double TienGui;
    double TienKyVong;
    double LaiSuat;

    cout << "Nhap so tien gui: ";
    cin >> TienGui;

    cout << "Nhap so tien ky vong: ";
    cin >> TienKyVong;

    cout << "Nhap lai suat theo nam: ";
    cin >> LaiSuat;

    Nam = log(TienKyVong/TienGui)/log(1+LaiSuat);

    cout << "So nam can thiet de dat duoc so tien ky vong la: " << Nam << endl;
	
    return 0;
}
