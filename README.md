#include<iostream>
using namespace std;

int prime(int x)
{
	int z;/*阶层数*/
    z = 1;
	while (x!=0)
	{

		z = z * x;
		x = x - 1;

	}
	return (z);
}
int main()
{
	int i, sum;
	sum = 0;
	for (i = 1; i <= 3; i++)
	{
		sum = prime(i) + sum;
	}
		cout << "1到20的阶层数只和为：" << sum << endl;
		return 0;

}
