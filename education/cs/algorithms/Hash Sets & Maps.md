When using a map, three main operations are used.

- Insert 
- Remove 
- Search 

| TreeMap | HashMap | Operation |
| ------- | ------- | --------- |
| O(logn) | O(1)    | Insert    |
| O(logn) | O(1)    | Remove    |
| O(logn) | O(1)    | Search    |
| O(n)    |         | In Order  |
HashMaps do not maintain any ordering, meaning each key has to be sorted first.

Map each key to an integer value and search through the array, example below.
Each key / value pair is added to the map for each first time it's seen, if it occurs twice, it is incremented.

```
names = ["alice", "brad", "collin", "brad", "dylan", "kim"]

alice : 1
brad : 1 -> would be incremented by +1 as brad has been seen twice.
collin : 1
```
