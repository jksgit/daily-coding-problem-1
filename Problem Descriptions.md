# Problem Description

-----
## Table of Content

[Problem 1-30](#1-30)  
[Problem 31-60](#31-60)

## <a id='31-60'></a> Problem 31-60

---
### Problem 36
This problem was asked by Dropbox.

Given the root to a binary search tree, find the second largest node in the tree.

### Problem 35
This problem was asked by Google.

Given an array of strictly the characters `'R'`, `'G'`, and `'B'`, segregate the values of the array so that all the Rs come first, the Gs come second, and the Bs come last. You can only swap elements of the array.

Do this in linear time and in-place.

For example, given the array `['G', 'B', 'R', 'R', 'B', 'R', 'G']`, it should become `['R', 'R', 'R', 'G', 'G', 'B', 'B']`.


### Problem 34
This problem was asked by Quora.

Given a string, find the palindrome that can be made by inserting the fewest number of characters as possible anywhere in the word. If there is more than one palindrome of minimum length that can be made, return the lexicographically earliest one (the first one alphabetically).

For example, given the string `"race"`, you should return `"ecarace"`, since we can add three letters to it (which is the smallest amount to make a palindrome). There are seven other palindromes that can be made from `"race"` by adding three letters, but `"ecarace"` comes first alphabetically.

As another example, given the string `"google"`, you should return `"elgoogle"`.

### Problem 33
This problem was asked by Microsoft.

Compute the running median of a sequence of numbers. That is, given a stream of numbers, print out the median of the list so far on each new element.

Recall that the median of an even-numbered list is the average of the two middle numbers.

For example, given the sequence `[2, 1, 5, 7, 2, 0, 5]`, your algorithm should print out:
```
2
1.5
2
3.5
2
2
2
```

### Problem 32
This problem was asked by Jane Street.

Suppose you are given a table of currency exchange rates, represented as a 2D array. Determine whether there is a possible arbitrage: that is, whether there is some sequence of trades you can make, starting with some amount A of any currency, so that you can end up with some amount greater than A of that currency.

There are no transaction costs and you can trade fractional quantities.

### Problem 31
This problem was asked by Google.

The edit distance between two strings refers to the minimum number of character insertions, deletions, and substitutions required to change one string to the other. For example, the edit distance between `“kitten”` and `“sitting”` is three: substitute the `“k”` for `“s”`, substitute the `“e”` for `“i”`, and append a `“g”`.

Given two strings, compute the edit distance between them.

----

## <a id='1-30'></a> Problem 1-30

----
### Problem 30
This problem was asked by Facebook.

You are given an array of non-negative integers that represents a two-dimensional elevation map where each element is unit-width wall and the integer is the height. Suppose it will rain and all spots between two walls get filled up.

Compute how many units of water remain trapped on the map in `O(N)` time and `O(1)` space.

For example, given the input `[2, 1, 2]`, we can hold 1 unit of water in the middle.

Given the input `[3, 0, 1, 3, 0, 5]`, we can hold 3 units in the first index, 2 in the second, and 3 in the fourth index (we cannot hold 5 since it would run off to the left), so we can trap 8 units of water.

### Problem 29
This problem was asked by Amazon.

Run-length encoding is a fast and simple method of encoding strings. The basic idea is to represent repeated successive characters as a single count and character. For example, the string `"AAAABBBCCDAA"` would be encoded as `"4A3B2C1D2A"`.

Implement run-length encoding and decoding. You can assume the string to be encoded have no digits and consists solely of alphabetic characters. You can assume the string to be decoded is valid.

### Problem 28
This problem was asked by Palantir.

Write an algorithm to justify text. Given a sequence of words and an integer line length `k`, return a list of strings which represents each line, fully justified.

More specifically, you should have as many words as possible in each line. There should be at least one space between each word. Pad extra spaces when necessary so that each line has exactly length `k`. Spaces should be distributed as equally as possible, with the extra spaces, if any, distributed starting from the left.

If you can only fit one word on a line, then you should pad the right-hand side with spaces.

Each word is guaranteed not to be longer than `k`.

For example, given the list of words `["the", "quick", "brown", "fox", "jumps", "over", "the", "lazy", "dog"]` and `k = 16`, you should return the following:

```
["the  quick brown", # 1 extra space on the left
"fox  jumps  over", # 2 extra spaces distributed evenly
"the   lazy   dog"] # 4 extra spaces distributed evenly
```


### Problem 27
This problem was asked by Facebook.

Given a string of round, curly, and square open and closing brackets, return whether the brackets are balanced (well-formed).

For example, given the string `"([])[]({})"`, you should return `true`.

Given the string `"([)]"` or `"((()"`, you should return false.


### Problem 26
This problem was asked by Google.

Given a singly linked list and an integer `k`, remove the <code>k<sup>th</sup></code> last element from the list. `k` is guaranteed to be smaller than the length of the list.

The list is very long, so making more than one pass is prohibitively expensive.

Do this in constant space and in one pass.

### Problem 25
This problem was asked by Facebook.

Implement regular expression matching with the following special characters:

`. (period)` which matches any single character
`* (asterisk)` which matches zero or more of the preceding element
That is, implement a function that takes in a string and a valid regular expression and returns whether or not the string matches the regular expression.

For example, given the regular expression `"ra."` and the string `"ray"`, your function should return true. The same regular expression on the string `"raymond"` should return false.

Given the regular expression `".*at"` and the string `"chat"`, your function should return true. The same regular expression on the string "chats" should return false.

### Problem 24
This problem was asked by Google.

Implement locking in a binary tree. A binary tree node can be locked or unlocked only if all of its descendants or ancestors are not locked.

Design a binary tree node class with the following methods:

`is_locked`, which returns whether the node is locked
`lock`, which attempts to lock the node. If it cannot be locked, then it should return false. Otherwise, it should lock it and return true.
`unlock`, which unlocks the node. If it cannot be unlocked, then it should return false. Otherwise, it should unlock it and return true.

You may augment the node to add parent pointers or any other property you would like. You may assume the class is used in a single-threaded program, so there is no need for actual locks or mutexes. Each method should run in `O(h)`, where `h` is the height of the tree.

### Problem 23
This problem was asked by Google.

You are given an M by N matrix consisting of booleans that represents a board. Each True boolean represents a wall. Each False boolean represents a tile you can walk on.

Given this matrix, a start coordinate, and an end coordinate, return the minimum number of steps required to reach the end coordinate from the start. If there is no possible path, then return null. You can move up, left, down, and right. You cannot move through walls. You cannot wrap around the edges of the board.

For example, given the following board:

```
[[f, f, f, f],
[t, t, f, t],
[f, f, f, f],
[f, f, f, f]]
```

and `start = (3, 0) (bottom left)` and `end = (0, 0) (top left)`, the minimum number of steps required to reach the end is `7`, since we would need to go through `(1, 2)` because there is a wall everywhere else on the second row.

### Problem 22
This problem was asked by Microsoft.

Given a dictionary of words and a string made up of those words (no spaces), return the original sentence in a list. If there is more than one possible reconstruction, return any of them. If there is no possible reconstruction, then return null.

For example, given the set of words `'quick', 'brown', 'the', 'fox'`, and the string `"thequickbrownfox"`, you should return `['the', 'quick', 'brown', 'fox']`.

Given the set of words `'bed', 'bath', 'bedbath', 'and', 'beyond'`, and the string `"bedbathandbeyond"`, return either `['bed', 'bath', 'and', 'beyond]` or `['bedbath', 'and', 'beyond']`.


### Problem 21
This problem was asked by Snapchat.

Given an array of time intervals `(start, end)` for classroom lectures (possibly overlapping), find the minimum number of rooms required.

For example, given `[(30, 75), (0, 50), (60, 150)]`, you should return 2.

### Problem 20
This problem was asked by Google.

Given two singly linked lists that intersect at some point, find the intersecting node. The lists are non-cyclical.

For example, given `A = 1 -> 3 -> 7 -> 8 -> 10` and `B = 99 -> 1 -> 8 -> 10`, return the node with value 8.

In this example, assume nodes with the same value are the exact same node objects.

Do this in `O(M + N)` time (where M and N are the lengths of the lists) and constant space.

### Problem 19
This problem was asked by Facebook.

A builder is looking to build a row of `N` houses that can be of `K` different colors. He has a goal of minimizing cost while ensuring that no two neighboring houses are of the same color.

Given an `N by K` matrix where the n<sup>th</sup> row and k<sup>th</sup> column represents the cost to build the n<sup>th</sup> house with k<sup>th</sup> color, return the minimum cost which achieves this goal.


### Problem 18
This problem was asked by Google.

Given an array of integers and a number `k`, where `1 <= k <= length` of the array, compute the maximum values of each subarray of length `k`.

For example, given `array = [10, 5, 2, 7, 8, 7]` and `k = 3`, we should get: `[10, 7, 8, 8]`, since:

```
10 = max(10, 5, 2)
7 = max(5, 2, 7)
8 = max(2, 7, 8)
8 = max(7, 8, 7)
```

Do this in `O(n)` time and `O(k)` space. You can modify the input array in-place and you do not need to store the results. You can simply print them out as you compute them.

### Problem 17
This problem was asked by Google.

Suppose we represent our file system by a string in the following manner:

The string `"dir\n\tsubdir1\n\tsubdir2\n\t\tfile.ext"` represents:
```
dir
    subdir1
    subdir2
        file.ext
```
The directory `dir` contains an empty sub-directory `subdir1` and a sub-directory `subdir2` containing a file `file.ext`.

The string `"dir\n\tsubdir1\n\t\tfile1.ext\n\t\tsubsubdir1\n\tsubdir2\n\t\tsubsubdir2\n\t\t\tfile2.ext"` represents:

```
dir
    subdir1
        file1.ext
        subsubdir1
    subdir2
        subsubdir2
            file2.ext
```

The directory `dir` contains two sub-directories `subdir1` and `subdir2`. `subdir1` contains a file `file1.ext` and an empty second-level sub-directory `subsubdir1`. `subdir2` contains a second-level sub-directory `subsubdir2` containing a file `file2.ext`.

We are interested in finding the longest (number of characters) absolute path to a file within our file system. For example, in the second example above, the longest absolute path is `"dir/subdir2/subsubdir2/file2.ext"`, and its length is 32 (not including the double quotes).

Given a string representing the file system in the above format, return the length of the longest absolute path to a file in the abstracted file system. If there is no file in the system, return 0.

Note:

The name of a file contains at least a period and an extension.

The name of a directory or sub-directory will not contain a period.

### Problem 16
This problem was asked by Twitter.

You run an e-commerce website and want to record the last N order ids in a log. Implement a data structure to accomplish this, with the following API:
```
record(order_id): adds the order_id to the log
get_last(i): gets the ith last element from the log. i is guaranteed to be smaller than or equal to N.
```
You should be as efficient with time and space as possible.

### Problem 15
This problem was asked by Facebook.

Given a stream of elements too large to store in memory, pick a random element from the stream with uniform probability.

### Problem 14
This problem was asked by Google.

The area of a circle is defined as <code>πr<sup>2</sup></code>. Estimate π to 3 decimal places using a Monte Carlo method.

Hint: The basic equation of a circle is <code>x<sup>2</sup> + y<sup>2</sup> = r<sup>2</sup></code>.

### Problem 13
This problem was asked by Amazon.

Given an integer k and a string s, find the length of the longest substring that contains at most k distinct characters.

For example, given s = `"abcba"` and k = 2, the longest substring with k distinct characters is `"bcb"`.

### Problem 12
This problem was asked by Amazon.

There exists a staircase with N steps, and you can climb up either 1 or 2 steps at a time. Given N, write a function that returns the number of unique ways you can climb the staircase. The order of the steps matters.

For example, if N is 4, then there are 5 unique ways:
```
1, 1, 1, 1
2, 1, 1
1, 2, 1
1, 1, 2
2, 2
```
What if, instead of being able to climb 1 or 2 steps at a time, you could climb any number from a set of positive integers X? For example, if `X = {1, 3, 5}`, you could climb 1, 3, or 5 steps at a time.

### Problem 11
This problem was asked by Twitter.

Implement an autocomplete system. That is, given a query string s and a set of all possible query strings, return all strings in the set that have s as a prefix.

For example, given the query string de and the set of strings `[dog, deer, deal]`, return `[deer, deal]`.

Hint: Try preprocessing the dictionary into a more efficient data structure to speed up queries.

### Problem 10
This problem was asked by Apple.

Implement a job scheduler which takes in a function f and an integer n, and calls f after n milliseconds.

### Problem 9
This problem was asked by Airbnb.

Given a list of integers, write a function that returns the largest sum of non-adjacent numbers. Numbers can be 0 or negative.

For example, [2, 4, 6, 2, 5] should return 13, since we pick 2, 6, and 5. [5, 1, 1, 5] should return 10, since we pick 5 and 5.

Follow-up: Can you do this in O(N) time and constant space?

### Problem 8
This problem was asked by Google.

A unival tree (which stands for "universal value") is a tree where all nodes under it have the same value.

Given the root to a binary tree, count the number of unival subtrees.

For example, the following tree has 5 unival subtrees:
```
   0
  / \
 1   0
    / \
   1   0
  / \
 1   1
```

### Problem 7
This problem was asked by Facebook.

Given the mapping a = 1, b = 2, ... z = 26, and an encoded message, count the number of ways it can be decoded.

For example, the message '111' would give 3, since it could be decoded as 'aaa', 'ka', and 'ak'.

You can assume that the messages are decodable. For example, '001' is not allowed.

(Not sure if '10001' is valid)

> Question: How do deal with 0 if there are any?

> Let's just assume there is no ZERO in the message;

### Problem 6
This problem was asked by Google.

An XOR linked list is a more memory efficient doubly linked list. Instead of each node holding next and prev fields, it holds a field named both, which is a XOR of the next node and the previous node. Implement a XOR linked list; it has an add(element) which adds the element to the end, and a get(index) which returns the node at index.

If using a language that has no pointers (such as Python), you can assume you have access to 'get_pointer' and 'dereference_pointer' functions that converts between nodes and memory addresses.

### Problem 5
This problem was asked by Jane Street.

`cons(a, b)` constructs a pair, and `car(pair)` and `cdr(pair)` returns the first and last element of that pair. For example, `car(cons(3, 4))` returns 3, and `cdr(cons(3, 4))` returns 4.

Given this implementation of cons:
```
def cons(a, b):
    def pair(f):
        return f(a, b)
    return pair
```
Implement car and cdr.

### Problem 4
This problem was asked by Stripe.

Given an array of integers, find the first missing positive integer in linear time and constant space. In other words, find the lowest positive integer that does not exist in the array. The array can contain duplicates and negative numbers as well.

For example, the input `[3, 4, -1, 1]` should give 2. The input `[1, 2, 0]` should give 3.

You can modify the input array in-place.

Some other thoughts:

> A naive method to solve this problem is to search all positive integers, starting from 1 in the given array. We may have to search at most n+1 numbers in the given array. So this solution takes O(n^2) in worst case.

> We can use sorting to solve it in lesser time complexity. We can sort the array in O(nLogn) time. Once the array is sorted, then all we need to do is a linear scan of the array. So this approach takes O(nLogn + n) time which is O(nLogn).

> We can also use hashing. We can build a hash table of all positive elements in the given array. Once the hash table is built. We can look in the hash table for all positive integers, starting from 1. As soon as we find a number which is not there in hash table, we return it. This approach may take O(n) time on average, but it requires O(n) extra space.

### Problem 3
This problem was asked by Google.

Given the root to a binary tree, implement `serialize(root)`, which serializes the tree into a string, and `deserialize(s)`, which deserializes the string back into the tree.

For example, given the following Node class
```
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right
```
The following test should pass:
```
node = Node('root', Node('left', Node('left.left')), Node('right'))
assert deserialize(serialize(node)).left.left.val == 'left.left'
```

### Problem 2
This problem was asked by Uber.

Given an array of integers, return a new array such that each element at index `i` of the new array is the product of all the numbers in the original array except the one at `i`.

For example, if our input was `[1, 2, 3, 4, 5]`, the expected output would be `[120, 60, 40, 30, 24]`. If our input was `[3, 2, 1]`, the expected output would be `[2, 3, 6]`.

Follow-up: what if you can't use division?

### Problem 1
This problem was recently asked by Google.

Given a list of numbers and a number `k`, return whether any two numbers from the list add up to `k`.

For example, given `[10, 15, 3, 7]` and `k` of 17, return true since 10 + 7 is 17.

Bonus: Can you do this in one pass?
