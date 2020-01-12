# Array

The implementation of array in C++ STL is **vector**

```
vector<T> v;
```

## Usage

When you need to store data **in order**. And will need to frequently access elements **by their indices**. This is a widely used data structure for storing sequence of data. It provides quick access to store elements.

## Basic Operations

### Insert

There are two different ways of inserting an element to a vector.

- **Insert it to the end of the vector by:**

```
void push_back (T val);
```

Time Complexity: O(1) (If no resize happened. Resizing the array takes O(n) time. )


- **Insert to a selected position by:**

```
void insert (iterator itr, T val);
```

Time Complexity: Expected to be O(n). Runtime is linear to the number of element behind the insert position.

Detailed reference: [vector::push_back](http://www.cplusplus.com/reference/vector/vector/push_back/),  [vector::insert](http://www.cplusplus.com/reference/vector/vector/insert/)


### Delete
There are also two different ways of deleting an element to a vector.

- **Delete the last element of the vector by:**

```
void pop_back (T val);
```

Time Complexity: O(1)


- **Delete the element at a selected position by:**

```
void erase (iterator itr, T val);
```
Time Complexity: O(1)


Detailed reference: [vector::pop_back](http://www.cplusplus.com/reference/vector/vector/pop_back/),  [vector::erase](http://www.cplusplus.com/reference/vector/vector/erase/)

### Access

There are two different functions of accessing an element in a vector.

```
reference operator[] (size_t n);
reference at (size_t n);
```


### Search

There is no single funtion to perform searching on vector. It can only be done by iterating through every elements. 

```
for(auto i : v){
 // look for target element...
}
```

Time complexity: O(n)

## Other Important Operations

```
void emplace_back (Args... args);
```

## Summary
| Operation | Function | Time Complexity |
| --------- | -------- | --------------- |
| Insert | push_back() <br> insert()| O(1) |
| Delete | pop_back() <br> delete()| O(1) |
| Access | [] operator <br> find()|  O(1) |
| Search | use a loop | O(n) |