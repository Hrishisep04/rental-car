# rental-car
#include <iostream>
#include <fstream>
#include <conio.h>
#include <stdlib.h>

using namespace std;
class customer
{
	private:
	public:
	string customername;
    string carmodel;
    string carnumber;
    char data;
};
class rent : public customer
{
	public:
	int days=0,rentalfee=0;
	void data()
	{
    int login();
	login();
	cout << "\t\t\t\tPlease Enter your Name: ";
    cin >> customername;
    cout<<endl;
    do
    {
        cout <<"\t\t\t\tPlease Select a Car"<<endl;
        cout<<"\t\t\t\tEnter 'A' for Tesla 20011."<<endl;
        cout<<"\t\t\t\tEnter 'B' for Hyundai 2015."<<endl;
        cout<<"\t\t\t\tEnter 'C' for Ford 2017."<<endl;
        cout<<"\t\t\t\tEnter 'D' for Mercedes 2017."<<endl;
        cout<<"\t\t\t\tEnter 'E' for Audi 2017."<<endl;
        cout<<"\t\t\t\tEnter 'F' for Skoda 2017."<<endl;
        cout<<"\t\t\t\tEnter 'G' for Volkswagun 2017."<<endl;
        cout<<"\t\t\t\tEnter 'H' for Toyota 2017."<<endl;
        cout<<endl;
        cout<<"\t\t\t\tChoose a Car from the above options: ";
        cin >>carmodel;
        cout<<endl;
 cout<<"--------------------------------------------------------------------------"<<endl;
 if(carmodel=="A")
 {
 	system("CLS");

		cout<<"You have choosed Tesla model 2011"<<endl;
		 ifstream inA("A.txt");
		 char str[200];
         while(inA) {
         inA.getline(str, 200);
         if(inA) cout << str << endl;
}
system("pause");
  }
  if(carmodel=="B")
  {
  	system("CLS");

		cout<<"You have choosed Hyundai model 2015"<<endl;
		 ifstream inB("B.txt");
         char str[200];
         while(inB) {
         inB.getline(str, 200);
         if(inB) cout << str << endl;

     }
     //sleep(2);
     system("pause");
 }
 if(carmodel=="C")
 {
 	system("CLS");
	     cout<<"You have choosed Ford model 2017"<<endl;
		 ifstream inC("C.txt");
         char str[200];
         while(inC)
     {
         inC.getline(str, 200);
         if(inC) cout << str << endl;
     }
     //sleep(2);
     system("pause");
}
if(carmodel=="D")
 {
 	system("CLS");
	     cout<<"You have choosed mercedes model 2017"<<endl;
		 ifstream inD("D.txt");
         char str[200];
         while(inD)
     {
         inD.getline(str, 200);
         if(inD) cout << str << endl;
     }
     //sleep(2);
     system("pause");
}
if(carmodel=="E")
 {
 	system("CLS");
	     cout<<"You have choosed audi model 2017"<<endl;
		 ifstream inE("E.txt");
         char str[200];
         while(inE)
     {
         inE.getline(str, 200);
         if(inE) cout << str << endl;
         cout<<"driver is ram";
     }
     //sleep(2);
     system("pause");
}
if(carmodel=="F")
 {
 	system("CLS");
	     cout<<"You have choosed skoda model 2017"<<endl;
		 ifstream inF("F.txt");
         char str[200];
         while(inF)
     {
         inF.getline(str, 200);
         if(inF) cout << str << endl;
     }
     //sleep(2);
     system("pause");
}
if(carmodel=="G")
 {
 	system("CLS");
	     cout<<"You have choosed volkawagen model 2017"<<endl;
		 ifstream inG("G.txt");
         char str[200];
         while(inG)
     {
         inG.getline(str, 200);
         if(inG) cout << str << endl;
     }
     //sleep(2);
     system("pause");
}
if(carmodel=="H")
 {
 	system("CLS");
	     cout<<"You have choosed toyota model 2017"<<endl;
		 ifstream inH("H.txt");
         char str[200];
         while(inH)
     {
         inH.getline(str, 200);
         if(inH) cout << str << endl;
     }
     //sleep(2);
     system("pause");
}
if(carmodel!="A" && carmodel!="B" &&  carmodel !="C" && carmodel != "D" && carmodel!="E" && carmodel!="F" && carmodel!="G" && carmodel!="H")

      cout<<"Invaild Car Model. Please try again!"<<endl;
        }
while(carmodel !="A" && carmodel !="B" &&  carmodel !="C" && carmodel!="D" && carmodel!="E" && carmodel!="F" && carmodel!="G" && carmodel!= "H");
    cout<<"--------------------------------------------------------------------------"<<endl;
    cout << "Please provide following information: "<<endl;
    cout<<"Please select a Car No. : ";
    cin >> carnumber;
    cout<<"Number of days you wish to rent the car : ";
    cin >> days;
    cout<<endl;
	}
	void calculate()
	{
		system("pause");
		system ("CLS");
		cout<<"Calculating rent. Please wait......"<<endl;
		system("pause");
		if(carmodel == "A"||carmodel=="a")
        rentalfee=days*56;
        if(carmodel == "B" ||carmodel=="b")
        rentalfee=days*60;
        if(carmodel == "C" ||carmodel=="c")
        rentalfee=days*75;
        if(carmodel == "D" ||carmodel=="d")
        rentalfee=days*85;
        if(carmodel == "E" ||carmodel=="e")
        rentalfee=days*95;
        if(carmodel == "F" ||carmodel=="f")
        rentalfee=days*65;
        if(carmodel == "G" ||carmodel=="g")
        rentalfee=days*55;
        if(carmodel == "H" ||carmodel=="h")
        rentalfee=days*75;
    }
void showrent()
    {
    cout << "\n\t\t                       Car Rental - Customer Invoice                  "<<endl;
    cout << "\t\t	///////////////////////////////////////////////////////////"<<endl;
    cout << "\t\t	| Invoice No. :"<<"------------------|"<<"#Cnb81353" <<"|"<<endl;
    cout << "\t\t	| Customer Name:"<<"-----------------|"<<customername<<"|"<<endl;
    cout << "\t\t	| Car Model :"<<"--------------------|"<<carmodel    <<"|"<<endl;
    cout << "\t\t	| Car No. :"<<"----------------------|"<<carnumber   <<"|"<<endl;
     cout << "\t\t	| Car color. :"<<"-------------------|"<<"black"     <<"|"<<endl;
    cout << "\t\t	| Number of days :"<<"---------------|"<<days        <<"|"<<endl;
    cout << "\t\t	| Your Rental Amount is :"<<"--------|"<<rentalfee   <<"|"<<endl;
    cout << "\t\t	| Caution Money :"<<"----------------|"<<"0"         <<"|"<<endl;
    cout << "\t\t	| Advanced :"<<"---------------------|"<<"0"         <<"|"<<endl;
    cout << "\t\t	 ________________________________________________________"<<endl;
    cout <<"\n";
    cout << "\t\t	| Total Rental Amount is :"<<"-------|"<<rentalfee             <<"|"<<endl;
    cout << "\t\t	 ________________________________________________________"<<endl;
    cout << "\t\t	 # This is a computer generated invoce and it does not"<<endl;
    cout << "\t\t	 require an authorised signture #"<<endl;
    cout <<" "<<endl;
    cout << "\t\t	///////////////////////////////////////////////////////////"<<endl;
    cout << "\t\t	You are advised to pay up the amount before due date."<<endl;
    cout << "\t\t	Otherwise penelty fee will be applied"<<endl;
    cout << "\t\t	///////////////////////////////////////////////////////////"<<endl;
    int f;
    system("PAUSE");

    system ("CLS");

     ifstream inf("thanks.txt");
  char str[300];
  while(inf)
  {
    inf.getline(str, 300);
    if(inf) cout << str << endl;
  }
  inf.close();
	}
};
class welcome
{
	public:
	int welcum()
	{
 ifstream in("welcome.txt");

  if(!in)
  {
    cout << "Cannot open input file.\n";
  }
  char str[1000];
  while(in)
{
    in.getline(str, 1000);
    if(in) cout << str << endl;
}
  in.close();
  system("pause");
  cout<<"\nStarting the program please wait....."<<endl;
  system("pause");
  cout<<"\nloading up files....."<<endl;
  system("pause");
  system ("CLS");
}
};
int main()
{
welcome obj1;
obj1.welcum();
rent obj2;
obj2.data();
obj2.calculate();
obj2.showrent();
return 0;
}

int login(){
   string pass ="";
   char ch;
   cout<<"\n\n\n\n\n\n\n\n\t\t\t\t\t       CAR RENTAL SYSTEM \n\n";
   cout<<"\t\t\t\t\t------------------------------";
   cout<<"\n\t\t\t\t\t\t     LOGIN \n";
   cout<<"\t\t\t\t\t------------------------------\n\n";
   cout << "\t\t\t\t\tEnter Password: ";
   ch = _getch();
   while(ch != 13)
    {
      pass.push_back(ch);
      cout << '*';
      ch = _getch();
   }
   if(pass == "pass")
    {
      cout << "\n\n\n\t\t\t\t\t\tAccess Granted! \n";
      system("PAUSE");
      system ("CLS");
   }
else
   {
      cout << "\n\n\t\t\t\t\t\t\tAccess Aborted...\n\t\t\t\t\t\t\tPlease Try Again\n\n";
      system("PAUSE");
      system("CLS");
      login();
   }
}

