```C++
#include <iostream>
#include <string>
#include <cstdlib>
#include <cstdio>
#include "time.h"
using namespace std;
int main()
{
  srand((unsigned)time(NULL));
	int i=0;
	string c[30000];
	int j=0,k=0;
	i=0;
	int a=0;
	while(i<30000)
	{
		while(j<(3+rand()%(8)))
		{
			a=65+rand()%(58);
			if ((a!=91) && (a!=92) && (a!=93) && (a!=94) && (a!=95) && (a!=96))
			{
				c[i]+=a;
			}
			else
			{
				j--;
			}
			j++;
		}
		j=0;
		i++;
	}
	i=0; 
	while (i<30000)
	{
		cout << c[i] << endl;
		i++;
	}
}
```
