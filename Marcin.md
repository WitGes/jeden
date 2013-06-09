```C++
#include <iostream>
#include "stdlib.h"
#include "time.h"
using namespace std;

int main(){
	int i=0, j=0, dlugslowa=0;
	char k; 
	string array[30000];
	srand((unsigned)time(NULL));
	for (i = 0; i<30000; i++)  {
		dlugslowa = 4+rand()%8;
        	for (j = 0; j<dlugslowa; j++){
            		k = 97+rand()%25;
            		array[j][1] = k;
            		cout << array[j][1];
            	}
        cout << endl;
    }
}
```
Formuła na rand():
```C++
int = dolnyzakres+rand() % górnyzakres-dolnyzakres+1;
```
