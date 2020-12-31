#include<iostream>
#include<conio.h>

using namespace std;
struct address {
	int H;                   //House
	int S;                   //street
	char C[20];              //City
	char P[20];              //Provice
	char w[20];              //country
};
struct Name {
	char FN[20];                //First name
	char LN[20];                //Last name

};
struct Registration {
	int se;                        //session
	char De[5];                    //Department
	int Rollno;                    
};
struct Dob {
	int day;
	int mounth;
	int year;

};
struct studentinformation
{
	Name N;
	Registration R;
	 long  cell;
	Dob D;
	address ADD;


};

void main() {
	studentinformation Detail;
	cout << "Enter first name : ";
	cin.getline(Detail.N.FN, 20);
	cout << endl<< "ENter Last name : ";
	cin.getline(Detail.N.LN, 20);
	cout <<endl<< "Enter your  Roll no : ";
	cin >> Detail.R.se >> Detail.R.De >> Detail.R.Rollno;
	cout <<endl<<"Enter your Date of Birth : ";
	cin >> Detail.D.day >> Detail.D.mounth >> Detail.D.year;
	cout << endl<< "Enter your Cell no : ";
	cin >> Detail.cell;
	cout << endl<< "Enter your Address like (house#, street, city, province, country) : ";
	cin >> Detail.ADD.H >> Detail.ADD.S;
	cin.getline(Detail.ADD.C, 20);
	cin.getline(Detail.ADD.P, 20);
	cin.getline(Detail.ADD.w, 20);
	cout << endl << endl << endl;

	cout << "                     ::Details::"<<endl;
	cout << "                    ----------------              "<<endl;
	cout << "Name  :  " << Detail.N.FN << Detail.N.LN << endl;
	cout << "Registration No : " << Detail.R.se << "-" << Detail.R.De << "-" << Detail.R.Rollno<<endl;
	cout << "date of Birth : " << Detail.D.day << "//" << Detail.D.mounth << "//" << Detail.D.year << endl;
	cout << "Cell no : " << Detail.cell << endl;
	cout << " Address : " << "house# " << Detail.ADD.H << ", street# " << Detail.ADD.S << ", " << Detail.ADD.C << ", "
		<< Detail.ADD.P << ", " << Detail.ADD.w;
		
	



	_getch();
}
