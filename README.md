#include <iostream>
#include <math.h>
using namespace std;

int main()
{	
    double Nam;
    double TienGui;
    double TienKyVong;
    double LaiSuat;
    
    do
    {
    	cout << "   Nhap so tien gui: ";
    	cin >> TienGui;

    	cout << "   Nhap so tien ky vong: ";
    	cin >> TienKyVong;

    	cout << "   Nhap lai suat theo nam: ";
    	cin >> LaiSuat;
    	if (TienKyVong <= TienGui || TienKyVong <= 0 || TienGui <= 0 || LaiSuat <= 0)
    	{
	     cout << "   Nhap sai du lieu,moi ban nhap lai.  " << endl;
    	}	
    }while(TienKyVong <= TienGui || TienKyVong <= 0 || TienGui<= 0 || LaiSuat <= 0);
	
    Nam = log(TienKyVong/TienGui)/log(1+LaiSuat);
    cout << "   So nam can thiet de dat duoc so tien ky vong la: " << Nam << endl;
    
    system("pause");
    
    return 0;
}
