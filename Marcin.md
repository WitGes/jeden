#include <iostream>
#include <cstdlib>
#include <time.h>
using namespace std;

int main(){
  int slowa=0, i=0, j=0, k=0, dlugslowa=0;
	string slowo;
	cin >> slowo;
	string array[30];
	srand (time(NULL));



	/*for (i=0; i<slowa; i++)
	{
		cin >> array[i];
	}*/
	for (i = 0; i<30; i++)  {
		dlugslowa = (rand() % 10 + 1);
		for (j = 0; j<dlugslowa; i++){
			k = (rand() % 65 + 57);
			char k;
			array[j][1] = k;
			cout << array[j][1];
		}
	}
	cin >> slowa;
}
