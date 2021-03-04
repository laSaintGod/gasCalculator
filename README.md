#include<iostream>
using namespace std;

int main() {
	//declearation
	char gasOptions;
	int travelTime;
	const double carbornDioxide = 258.0, air = 332.5, helium = 972.0, hydrogen = 1270.0;

	//gas type selection.
	cout << " Please select your gas type:" << endl;
	cout << "A. Carbon Dioxide" << endl;
	cout << "B. Air" << endl;
	cout << "C. Helium" << endl;
	cout << "D. Hydrogen" << endl;
	cin >> gasOptions;

	switch (gasOptions)
	{
	case 'a':
	case 'A':

	case'b':
	case'B':

	case'c':
	case'C':

	case'd':
	case'D':

		cout << "Please enter the number of secods it took" << endl
			<< "for the gas to travel";

		cin >> travelTime;

		if (travelTime < 0, travelTime >30)
		{
			cout << "Please time  not be less than 0 or more than 30 " << endl;
		}
		else
		{
			if (gasOptions == 'a', 'A') {
				travelTime *= carbornDioxide;
				cout << "Carbon Dioxide";
			}
			else if (gasOptions == 'b', 'B') {
				travelTime *= air;
				cout << "Air";
			}
			else if (gasOptions == 'c', 'C') {
				travelTime *= helium;
				cout << "Helium";
			}
			else if (gasOptions == 'd', 'D') {
				travelTime *= hydrogen;
				cout << "Hydrogen";
			}
			cout <<" " << "is" << " " << travelTime << "meters away." << endl;
		}

	default:
		cout << "please enter a letter between A to D" << endl;

		break;
	}
	return 0;
}

