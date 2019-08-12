# Restaurant-Application-C-
#include <iostream>
using namespace std ;
int main ()
{
	setlocale(LC_ALL,"Turkish") ;
	int a,b,mercimek=5,ayran=3,pilav=7,hesap;
	yeniden :
	cout << "Please enter your language(Lütfen Dilinizi Giriniz!) ! Turkish = 1 , English = 2 " << endl ;
	cin >> b ;
	if ( b == 1) 
	{
		cout << " ÇayBardağı Kafe'ye Hoşgeldiniz :)  " << "Lütfen para biriminizi girin ! TL/USD "; 
	string birim ;
	cin >> birim ;
	yeniden2:
	cout << "Ne istersiniz?" << endl << "Mercimek Çorbası = 1 - Pilav = 2 - Ayran = 3 - Hepsi = 4" << endl ;
	cin >> a ;
	if ( a == 4 )
	  {
			cout << "Mercimek Çorbası = 5" << birim << endl ;
			cout << "Ayran = 3" << birim << endl ;
			cout << "Pilav = 7" << birim << endl ;
			hesap = ayran+pilav+mercimek  ;
			cout << "Hesabınız : " << hesap << " " << birim ;
	  }
	  else 
	  {
	  	cout << "Hepsini Almadan Bırakmam :)" ;
	  	goto yeniden2 ;
	  }
	}
	
	else if ( b == 2)
	{
		cout << "Welcome to ÇayBardağı CAFE :)  " << "Please enter your currency TL/USD " << endl ; 
	string birim ;
	cin >> birim ;
	yeniden3 :
	cout << "What Do you Want?" << endl << "Lentil Soup = 1 - Rice = 2 - Ayran = 3 - ALL = 4" << endl;
	cin >> a ;
	if ( a == 4)
	   {
			cout << "Lentil Soup = 5" << birim << endl ;
			cout << "Ayran = 3" << birim << endl ;
			cout << "Rice = 7" << birim << endl ;
			hesap = ayran+pilav+mercimek ;
			cout << "Your Bills : " << hesap << " " << birim ;
			 
	   }
	   else
	   {
	   	cout << "You must buy them all" ;
	   	goto yeniden3 ;
	   }
    }    
else
{
	cout << "ERROR!" ;
	goto yeniden ;
}
	return 0 ;
}
