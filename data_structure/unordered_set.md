# Hash Set

The implementation of set in C++ STL is **unoreder_set**

```
unoreder_set<T> v;
```

Unordered set is similar to **set**. The two data structure both have a same feature that the elements they contain are unique. The differennce is that elements in a set follow a specific order, but not in unordered_set. 

The underlying data structure of set implementation is hash table.

## Usage

When you need to store data **uniquely**, and would **frequently access them**. Unordered set is commonly used in situations such as storing a value for future search.

## Basic Operations

### Insert

```
pair<iterator,bool> insert (const T& val);
```

Time Complexity: O(1). 

Detailed reference: [unordered_set::insert](http://www.cplusplus.com/reference/unordered_set/unordered_set/insert/)


### Delete

```
size_type erase (const T& val);
```
Time Complexity: O(1)

Detailed reference: [unordered_set::erase](http://www.cplusplus.com/reference/unordered_set/unordered_set/erase/)

### Access

There is no direct way to access elements in a set. You can only perform searching.

### Search

```
iterator find (const T& val) const;
size_t count (const T& val);
```

The find function returns an iterator of the first occurance, and null if it does not exist. The count function returns the number of occurance (in a set, it can only be 1 or 0).

Time complexity: Expected to be O(1)

Detailed reference: [unordered_set::find](http://www.cplusplus.com/reference/unordered_set/unordered_set/find/), [unordered_set::count](http://www.cplusplus.com/reference/unordered_set/unordered_set/count/)

## Other Important Operations



## Summary
| Operation | Function | Time Complexity |
| --------- | -------- | --------------- |
| Insert | insert()| O(1) |
| Delete | erase()| O(1) |
| Access | | |
| Search | find() | O(1) |
