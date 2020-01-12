# Stack

The implementation of stack in C++ STL is [stack](http://www.cplusplus.com/reference/stack/stack/)

```
stack<T> s;
```

Noticed that stack shares a lot of same functions and many similar features with [queue](http://www.cplusplus.com/reference/queue/queue/)

## Usage

Stack is designed to provide **last-in first-out (LIFO)** fashion. Data is manipulated from only one end of the structure. It is typically used when the last inserted element needs to be the first one extracted, for example in algorithms such as Depth-First-Search (DFS).

## Basic Operations

### Insert

You can only insert new element to the top of the stack, by

```
void push (T val);
```

Time Complexity: O(1) (Actual runtime depends on its underlying container. )

Detailed reference: [stack::push](http://www.cplusplus.com/reference/stack/stack/push/)


### Delete

You can only delete the top element of the stack, by

```
void pop();
```

Time Complexity: O(1)

Detailed reference: [stack::pop](http://www.cplusplus.com/reference/stack/stack/pop/)

### Access

You can only access the top element of the stack, by

```
T top();
```

Time Complexity: O(1)

Detailed reference: [stack::top](http://www.cplusplus.com/reference/stack/stack/top/)

### Search

There is no single funtion to perform searching on stack. It can only be done by popping out every elements, but that's not a effective way of using this data structure. If you ever need to perform searching, you should not store your data in stack.

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
