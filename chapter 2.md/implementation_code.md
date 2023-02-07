```
//implementation algo with c++

#include<iostream>
#include<algorithm>
#include<vector>
using namespace std;

int main()
{
	int n;       
	cin >> n; 
	int key;
    vector<int>v(n);

	for (int i = 0; i < n; i++)
	{
		cin >> v[i];  // insert element 
	}
	// Ascending order
		for (int i = 0; i < n; i++)
	{
		 key = v[i];  
		int j = i - 1;   
		while (j>=0 && v[j]> key) //comper key and element of v[j] && If the condition is met, we will switch element
		{
			v[j + 1] = v[j];  //swap element with previous element
			j--;  
		}
		v[j + 1] = key;  //move to the next two elements and compare them
	}
	
	//Display items in order
	
	for (auto i:v)
	{
		cout << i << " ";
	}
}

	
```
