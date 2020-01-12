# Deque

The implementation of deque in C++ STL is [deque](http://www.cplusplus.com/reference/deque/deque/)

```
deque<T> s;
```

Noticed that deque shares a lot of same functions and many similar features with [stack](http://www.cplusplus.com/reference/stack/stack/)

## Usage

deque is designed to provide **first-in first-out (FIFO)** fashion. Data is inputed from only one end, and processed at the other end of the structure. It is typically used when the elements needs to be processde in the order they are inserted, for example in algorithms such as Breath-First-Search (DFS).

## Basic Operations

### Insert

You can only insert new element to the end of the deque, by

```
void push (T val);
```

Time Complexity: O(1) (Actual runtime depends on its underlying container. )

Detailed reference: [deque::push](http://www.cplusplus.com/reference/deque/deque/push/)


### Delete

You can only delete the first element of the deque, by

```
void pop();
```

Time Complexity: O(1)

Detailed reference: [deque::pop](http://www.cplusplus.com/reference/deque/deque/pop/)

### Access

You can only access the first element of the deque, by

```
T top();
```

Time Complexity: O(1)

Detailed reference: [deque::top](http://www.cplusplus.com/reference/deque/deque/top/)

### Search

There is no single funtion to perform searching on deque. It can only be done by popping out every elements, but that's not a effective way of using this data structure. If you ever need to perform searching, you should not store your data in deque.

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
