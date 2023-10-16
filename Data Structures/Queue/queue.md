# simple queue array implementation

```
#include <iostream>
using namespace std;

const int MAX_SIZE = 5;  

class Queue {
     int arr[MAX_SIZE];

     int front = -1;
     int rear = -1;

public:
    Queue() { front = -1;
    rear = -1;
}

    void enqueue(int x)
    {
        if (rear != MAX_SIZE - 1)
        {
            if (rear == -1 && front == -1)
            {
                front++;
                arr[++rear] = x;
            }
            else
            {
                arr[++rear] = x;  
            }
        }
        else
        {
            cout << "Queue Full" << endl;
        }

    }

    void deQueue()
    {
        
            if (rear != -1 && front != -1 && front<=rear)
            {
                front++;

            }
            else
            {
                cout << "Queue Empty" << endl;
            }
        }
    void print()
    {
        if (rear != -1 && front != -1 && front <= rear)
        {
            for (int i = front; i <=rear ; i++)
            {
                cout << arr[i] << " ";
            }
        }
        else
        {
            cout << "Queue Empty" << endl;

        }
    }

};

int main() {
    Queue q;

    q.enqueue(1);
    q.enqueue(3);
    q.enqueue(4);
    cout << "queue before  " ;
    q.print();
    cout<<endl;
    q.deQueue();
    q.deQueue();
    cout << "queue after = ";
     q.print();

    return 0;
}
```
