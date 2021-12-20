//Loopy
  
#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;
  
int main() {

	int myInt; int counter = 0;
	cout << "Enter number: ";
	cin >> myInt;
	do {
		cout << counter;
		if (myInt != counter) cout << ',';	
		else cout << '.';
		counter++;
		
	} while (counter <= myInt);
	
	return 0;

}

//Pointless Box

#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {

	int myNum ;
	here:
	cout << "Enter (1/2): ";
	cin >> myNum;
	while (myNum == 1 || myNum ==2)
	{
		if (true){

			cout << "you have entered: " << myNum << endl;
			break;
		}
		else {
			cout << "you have entered: " << myNum << endl;
		}
	}
	if (myNum > 2 || myNum <= 0)
	{
		cout << "Invalid Input, Try again  "; goto here;
	}
	return 0;
}


//Reverse 9 Times table

#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {

	int myNum = 108;

	while (myNum > 0)
	{
		cout << myNum << endl;
		myNum -= 9;
	}
	return 0;
}


//Remain Positive

#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {

	double myNum = 20;

	while (myNum >= 0)
	{
		cout << myNum << endl;
		myNum -= 0.5;
	}
	return 0;
}
//Brute Force I

#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {

	int cp = 246, p;
	cout << "Enter Password: ";
	cin >> p;
	while (p != cp) {
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Wrong Password, Try again: ";
		cin >> p;
	}
  cout << "You are now logged in " << endl;

	return 0;
}
  
//Brute Force II
  
#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {	
	
	int cp = 246, a = 5, p; 
	cout << "Enter Password: ";
	cin >> p;
	while (p != cp) {
		cin.clear();
		cin.ignore(1000, '\n');
		cout << a << " Attempts remaining " << "Wrong Password, Try again: ";
		cin >> p;
		a--;
		if (a <= 0) {
			cout << "Your Account is now locked";
			break;
		}
	}
	if (p == cp) cout << "You are now logged in " << endl;

	return 0;
}
//Input Improvement
                                                       
#include <iostream>
#include <string>
#include <math.h>
#include <array>
using namespace std;

int main() {

	char input;
	do {
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Would you like to Quit (Y/N)?" << endl;
		cin >> input;
	} while ((input != 'Y') && (input != 'N') && (input != 'y') && (input != 'n'));
	
	return 0;
}                                                    
