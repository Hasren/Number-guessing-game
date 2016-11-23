# Number-guessing-game



#include "stdafx.h"
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;


int main()
{
	int done;
	int x;
	int y;
	cout << "guess a number between 1 and 100" << endl;
	cin >> x;
	
	srand(time(0));
	y = 1 + rand() % 100;


	while (x != y)
	{
		if (x < y)
			cout <<"Guess a higher number" << endl;
		else if (x > y)
			cout << "Guess a lower number" << endl;
		else
			cout <<"thats not a whole number between 1 and 100, try again" << endl;

		cout << "guess a number between 1 and 100" << endl;
		cin >> x;
	}

	if (x = 50)
		cout << "You are correct, thanks for playing!" << endl;

	cin >> done;

	return 0;
}
