* implement a stack using an array
```
#include <iostream>
#include <cmath>
#include <algorithm>

using namespace std;

const int MAX_SIZE = 50;

class stack
{
    int top;
    int items[MAX_SIZE];

public:
    stack() : top(-1)
    {}

    void push(int element)
    {
        if (top >= MAX_SIZE - 1)
        {
            cout << "Stack is full" << endl;
        }
        else
        {
            top++;
            items[top] = element;
        }
    }

    bool empty()
    {
        return top < 0;
    }
    void pop(int& element)
    {
        if (empty())
        {
            cout << "Stack is empty" << endl;
        }
        else
        {
            element = items[top];
            top--;
        }
    }

    void Top(int& Stacktop)
    {
        if (empty())
        {
            cout << "Stack is empty" << endl;
        }
        else
        {
            Stacktop = items[top];
            cout << Stacktop << endl;
        }
    }

    void print()
    {
        for (int i = top; i >= 0; i--)
        {
            cout << items[i] << endl;
        }
    }
};

int main()
{
    stack S;
    S.push(1);
    S.push(11);
    S.push(111);
    S.push(2222);
    int topElement;
    //S.Top(topElement);
    //S.push(10000);
    //S.pop(topElement);
    //S.print();
    return 0;
}
```
