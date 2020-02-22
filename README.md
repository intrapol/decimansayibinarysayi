# DECİMAL SAYIYI BİNARY SAYIYA ÇEVİRME
```#include <iostream>
using namespace std;
int main()
{
    // sayilar değişkenini çıkan sonucu ters çevirmek için kullanıcağız
    int sayi,sayilar[100],i;
    cout<<"Bir sayi giriniz : ";
    cin>>sayi;
// for içinde decimal sayıyı binary şekline çeviriyoruz 
    for(i=0;;i++)
    {
        if(sayi<2)
        {
           sayilar[i]=(sayi%2);
            break;
        }
        sayilar[i]=(sayi%2);
        sayi=sayi/2;
    }
    // çevirdiğimiz binary sayı yukarıdaki for içinde ters oluştu
    // bunun için sayıyı tekrardan sondan başlayarak yazdırıyoruz 
    while(i>=0){
        cout<< sayilar[i];
        i--;
    }
}```
