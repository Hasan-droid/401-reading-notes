
# Preparation Materials

>Intro to Hash Tables

- Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

- The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value.

- Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

- Hash maps take advantage of an array’s `O(1)` read access.

- Basically, a hash code turns a key into an integer.
- A hashtable traditionally is created from an array.

- Hash Maps can have any number of buckets.

- `Add()` > When adding a new key/value pair to a hashtable
- `Find()` > The Find takes in a key, gets the Hash, and goes to the index location specified.
- `Contains()` > The Contains method will accept a key, and return a bool on if that key exists inside the hashtable.   The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.

- `GetHash()`

&nbsp;

&nbsp;

> basics of hash tables

- Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects. Some examples of how hashing is used in our lives include:

1. In universities, each student is assigned a unique roll number that can be used to retrieve information about them.
2. In libraries, each book is assigned a unique number that can be used to determine information about the book, such as its exact position in the library or the users it has been issued to etc.

- Hashing is implemented in two steps:

1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

```React
hash = hashfunc(key)
index = hash % array_size
```

- To achieve a good hashing mechanism, It is important to have a good hash function with the following basic requirements:

1. Easy to compute: It should be easy to compute and must not become an algorithm in itself.

2. Uniform distribution: It should provide a uniform distribution across the hash table and should not result in clustering.

3. Less collisions: Collisions occur when pairs of elements are mapped to the same hash value. These should be avoided.

- Applications

1. Associative arrays: Hash tables are commonly used to implement many types of in-memory tables. They are used to implement associative arrays (arrays whose indices are arbitrary strings or other complicated objects).
2. Database indexing: Hash tables may also be used as disk-based data structures and database indices (such as in dbm).
3. Caches: Hash tables can be used to implement caches i.e. auxiliary data tables that are used to speed up the access to data, which is primarily stored in slower media.
4. Object representation: Several dynamic languages, such as Perl, Python, JavaScript, and Ruby use hash tables to implement objects.
5. Hash Functions are used in various algorithms to make their computing faster
&nbsp;

&nbsp;
