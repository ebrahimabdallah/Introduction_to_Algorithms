```
#include<iostream>
#include<algorithm>
#include<vector>
using namespace std;

int main()
{
	int n;       
	cin >> n; 
    vector<int>v(n);

	for (int i = 0; i < n; i++)
	{
		cin >> v[i];  // insert element 
	}

	for (int i = 0; i < n; i++)
	{
		int key = v[i];  
		int j = i - 1;  
		while (j>=0 && v[j]> key) //comper key and element of v[j]
		{
			v[j + 1] = v[j];  //move to the next two elements and compare them
			j--;  
		}
		v[j + 1] = key;  
	}
	for (auto i:v)
	{
		cout << i << " ";
	}
}

	
```