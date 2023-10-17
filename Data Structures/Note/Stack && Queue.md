| # | Stack |Queue |
| --------------- | --------------- | --------------- |
| define |  abstract data type (ADT) that follows the Last-In-First-Out (LIFO)    |A queue is an abstract data type (ADT) that follows the First-In-First-Out (FIFO)    |
| Working | Top  | FRONT && REAR ||Head && Tail |
| Operations | Pop && Push  && isEmpty && isFull | Dequeue()  && Enqueue(item)  &&    && isFull()  && isEmpty|
| underflows | pop an empty stack  | when trying to remove an element from an empty queue|
| overflows |try to push more items on a stack than it can hold. | trying to add an element onto a full |
| Real-world applications | Balanced Bracket| CPU task scheduling && Asynchronous data transfer && Email |
| Types |Fixed Size  && Dynamic Size   |Simple Queue && Circular Queue(bank) && Priority Queue && Double Ended Queue |
| description | ![stack(1)](https://github.com/ebrahimabdallah/Introduction_to_Algorithms/assets/119238955/0d8c6491-9aad-4e3c-a5c5-c894604f4a6d)| ![queue](https://github.com/ebrahimabdallah/Introduction_to_Algorithms/assets/119238955/0a3114af-5e14-458c-b14e-4cd6b7ee68d2)|




* overflow && underflow

* Queue overflow results from trying to add an element onto a full queue and queue
* underflow happens when trying to remove an element from an empty queue
```
enqueue(Q, x):
	if head[Q] == tail[Q] + 1  //full 
		 error "overflow"
	 
dequeue(Q):
	if head[Q] == tail[Q] //empty
		 error "underflow"
 ```

 # problems
* https://codeforces.com/group/c3FDl9EUi9/contest/263096/problem/E
* https://codeforces.com/group/c3FDl9EUi9/contest/263096/problem/D
* https://codeforces.com/group/c3FDl9EUi9/contest/263096/problem/G
* https://codeforces.com/group/c3FDl9EUi9/contest/263096/problem/H
* https://codeforces.com/group/MWSDmqGsZm/contest/223340/problem/B
