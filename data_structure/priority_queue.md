# Priority Queue

The implementation of priority_queue in C++ STL is [priority_queue](http://www.cplusplus.com/reference/queue/priority_queue/)

```
priority_queue<T> s;
```

## Usage

Priority queue is specifically designed to guarentee that the first element always has the highest priority. The definition of priority depends on the compare funtion user defines.

Data is inputed from only one end, and processed at the other end of the structure. It is typically used when the elements needs to be processde in the order they are inserted, for example in algorithms such as Dijkstra.

## Basic Operations

### Insert

You can only insert new element to the end of the priority queue, by

```
void push (T val);
```

Time Complexity: Depends on its actual implementation. Default setting of priority_queue in C++ provides O(log n) time.

Detailed reference: [priority_queue::push](http://www.cplusplus.com/reference/queue/priority_queue/push/)


### Delete

You can only delete the first element of the priority queue, by

```
void pop();
```

Time Complexity: Depends on its actual implementation. Default setting of priority_queue in C++ provides O(log n) time.

Detailed reference: [priority_queue::pop](http://www.cplusplus.com/reference/queue/priority_queue/pop/)

### Access

You can only access the first element of the priority queue, by

```
T top();
```

Time Complexity: O(1)

Detailed reference: [priority_queue::top](http://www.cplusplus.com/reference/queue/priority_queue/top/)

### Search

There is no single funtion to perform searching on priority queue. It can only be done by popping out every elements, but that's not a effective way of using this data structure. If you ever need to perform searching, you should not store your data in priority queue.

## Other Important Operations

```
void emplace (Args... args);
```

## Summary
| Operation | Function | Time Complexity |
| --------- | -------- | --------------- |
| Insert | push() | O(log n) |
| Delete | pop() | O(log n) |
| Access | top() |  O(1) |
| Search | - | - |
