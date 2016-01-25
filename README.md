# Semiprime
Semiprime calculator
#include <iostream>
using namespace std;

int main()
{
	int prime1 = 2;
	int prime2 = 3;
	int semiprime;

	for (int i = 0; i < 1000; i++)
	{
		for (int j = 0; j < 1000; j++)
		{
			semiprime = prime1 * prime2;
			
			if (semiprime / 2 && semiprime / 3)
			{
				prime1++;
				prime2++;
				semiprime = prime1 * prime2;
			}
			else
			{
				cout << semiprime;
			}
		}
	}

	system("pause");
	return 0;
}
