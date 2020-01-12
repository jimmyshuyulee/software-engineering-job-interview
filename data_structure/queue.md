# Queue

The implementation of queue in C++ STL is [queue](http://www.cplusplus.com/reference/queue/queue/)

```
queue<T> s;
```

Noticed that queue shares a lot of same functions and many similar features with [stack](http://www.cplusplus.com/reference/stack/stack/)

## Usage

Queue is designed to provide **first-in first-out (FIFO)** fashion. Data is inputed from only one end, and processed at the other end of the structure. It is typically used when the elements needs to be processde in the order they are inserted, for example in algorithms such as Breath-First-Search (DFS).

## Basic Operations

### Insert

You can only insert new element to the end of the queue, by

```
void push (T val);
```

Time Complexity: O(1) (Actual runtime depends on its underlying container. )

Detailed reference: [queue::push](http://www.cplusplus.com/reference/queue/queue/push/)


### Delete

You can only delete the first element of the queue, by

```
void pop();
```

Time Complexity: O(1)

Detailed reference: [queue::pop](http://www.cplusplus.com/reference/queue/queue/pop/)

### Access

You can only access the first element of the queue, by

```
T top();
```

Time Complexity: O(1)

Detailed reference: [queue::top](http://www.cplusplus.com/reference/queue/queue/top/)

### Search

There is no single funtion to perform searching on queue. It can only be done by popping out every elements, but that's not a effective way of using this data structure. If you ever need to perform searching, you should not store your data in queue.

## Other Important Operations

```
void emplace (Args... args);
```

## Summary
| Operation | Function | Time Complexity |
| --------- | -------- | --------------- |
| Insert | push()| O(1) |
| Delete | pop()| O(1) |
| Access | top()|  O(1) |
| Search | - | - |
