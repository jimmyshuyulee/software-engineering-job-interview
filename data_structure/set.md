# Set

The implementation of set in C++ STL is **set**

```
set<T> v;
```

Set is similar to **unordered_set**. The two data structure both have a same feature that the elements they contain are unique. The differennce is that elements in a set follow a specific order, but not in unordered_set. 

The underlying data structure of set implementation is binary tree.

## Usage

When you need to store data **uniquely**, and would like them to be **in a self defined order**. Set is commonly used in situations such as extracting unique values and storing them in a sorted order.

## Basic Operations

### Insert

```
pair<iterator,bool> insert (const T& val);
```

Time Complexity: O(log n). 

Detailed reference: [set::insert](http://www.cplusplus.com/reference/set/set/insert/)


### Delete

```
size_type erase (const T& val);
```
Time Complexity: O(log n)

Detailed reference: [set::erase](http://www.cplusplus.com/reference/set/set/erase/)

### Access

There is no direct way to access elements in a set. You can only perform searching.

### Search

```
iterator find (const T& val) const;
size_t count (const T& val);
```

The find function returns an iterator of the first occurence, and null if it does not exist. The count function returns the number of occurence (in a set, it can only be 1 or 0).

Time complexity: O(log n)

Detailed reference: [set::find](http://www.cplusplus.com/reference/set/set/find/), [set::count](http://www.cplusplus.com/reference/set/set/count)

## Other Important Operations

```
iterator lower_bound (const T& val) const;
iterator upper_bound (const T& val) const;
```

## Summary
| Operation | Function | Time Complexity |
| --------- | -------- | --------------- |
| Insert | insert()| O(log n) |
| Delete | erase()| O(log n) |
| Access | |   |
| Search | find() | O(log n) |
