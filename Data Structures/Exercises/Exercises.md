# 10.1-3
| index| top | top | top |top  |top  | top |
| -- | -- | -- | -- | -- | -- |--|
|1| 4| 4 |4|4| 4 |4 |
|2|  | 1| 1|1| 1| 1|
|3|  |  | 3| | 8| |
|4|  |  | | | | |
|5|   |    | || | |
|6|   |    | || | |
_______________________
# 10.1-3

| index| 1 | 2 | 3 | 4 | 5 | 6 |
| -- | -- | -- | -- | -- | -- |--|
|| 4 |    |  | | | |
||  4| 1  |  | | | |
|| 4 |  1 | 3| | | |
||   | 1  | 3| | | |
||   |    |3 |8| | |


  
 
_____________________________________________________________________________________________

# 10.1-4

/**
Queue overflow results from trying 
to add an element onto a full
queue and queue underflow happens when trying 
to remove an element from an empty queue
**/
```
#include <iostream>
using namespace std;

const int MAX_SIZE = 5;

class Queue {
    int arr[MAX_SIZE];
    int front;
    int rear;

public:
    Queue() {
        front = -1;
        rear = -1;
    }

    bool Full() {
        return rear == MAX_SIZE - 1;
    }

    bool Empty() {
        return front == -1 || front > rear;
    }

    void enqueue(int x) {
        if (Full()) {
            cout << "Queue Overflow" << endl;
            return;
        }

        if (rear == -1 && front == -1) {
            front++;
        }

        arr[++rear] = x;
    }

    void deQueue() {
        if (Empty()) {
            cout << "Queue Underflow" << endl;
            return;
        }

        front++;
    }

    void print() {
        if (Empty()) {
            cout << "Queue Empty" << endl;
        }
        else {
            for (int i = front; i <= rear; i++) {
                cout << arr[i] << " ";
            }
            cout << endl;
        }
    }
};

int main() {
    Queue q;

    q.enqueue(1);
    q.enqueue(3);
    q.enqueue(4);
    q.enqueue(3);
    q.enqueue(4);
    q.enqueue(4);

    q.deQueue();
    q.deQueue();
    q.deQueue();
    q.deQueue();
    q.deQueue();
    q.deQueue();
    q.print();

    return 0;
}
```
