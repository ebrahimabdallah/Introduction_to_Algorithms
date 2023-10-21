```
#include <iostream>
using namespace std;

class Node {
public:
    int data;
    Node* next;
};

class Linkedlist
{
public:
    Node* head;
    Linkedlist()
    {
        head = NULL;
    }
    bool isEmpty()
    {
    
        return  (head == NULL);
    }
    void insertFirst(int newValue)
    {
        Node* newnode = new Node();
        newnode->data = newValue;

        if (isEmpty())
        {
            newnode->next = NULL;
            head = newnode;
        }
        else
        {
            newnode->next = head;
            head = newnode;
        }
    }
        void display()
        {
             Node* temp = head;
            while (temp != NULL)
            {
                cout << temp->data << endl;
                temp = temp->next;
            }

        }
        
        int count() {
            int counter = 0;
            Node* temp = head;
            while (temp != NULL) {
                counter++;
                temp = temp->next;
            }
            return counter;
        }

        bool isFound(int item)
        {
            bool found = false;
            Node* temp = head;
            while (temp != NULL)
            {
                if (temp->data == item)
                    found = true;
                   temp = temp->next;

            }
            return found;
        }
};
int main() 
{
    Linkedlist L;
    if (L.isEmpty())
        cout << "Empty"<<endl;
    else
        cout << "items list " << L.count() << endl;
    L.insertFirst(9);
    L.insertFirst(99);
    L.insertFirst(19);
    L.insertFirst(91);
    L.display();

    bool isFound = L.isFound(10);
    if (isFound)
    {
        cout << " Found" << endl;
    }
    cout << "Not Found" << endl;

}

```
