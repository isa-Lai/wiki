# Python
Python

## General
### To check data type
```python
type(x)
isinstance(x,int)
```

### To make nxn empty list
```python
matrix = [[0] * n for _ in range(n)]
```
 
### Assign two value to two parameter resqectively
```python
row, col = row + dx, col + dy
```

### range()
```python
range(start, stop, step) # start default 0
range(6) # from 0 to 5 
```

### Dictionary
Dictionary can be used as hash table
```python
my_dict={'Dave' : '001' , 'Ava': '002' , 'Joe': '003'}
print("All keys")
for x in my_dict:
    print(x)       #prints the keys
print("All values")
for x in my_dict.values():
    print(x)       #prints values
print("All keys and values")
for x,y in my_dict.items():
    print(x, ":" , y)       #prints keys and values

print(my_dict.keys()) # dict_keys([‘Dave’, ‘Ava’, ‘Joe’])
print(my_dict.values()) # dict_values([‘001’, ‘002’, ‘003’])
print(my_dict.get('Dave')) # 001
# check contains key
if key in dict.keys()
if key in dict
dict.has_key(key)

del my_dict['Dave']  #removes key-value pair of 'Dave'
my_dict.pop('Ava')   #removes the value of 'Ava'
my_dict.popitem()    #removes the last inserted item
#only joe remains
```
 
### Set
Set can be used as Hash table without key
```python
occ = set()
occ.remove(item)
occ.add(item)
```
 
### List
List in python can be used as stack
```python
mylist = []
mylist.append(item) # push
mylist.pop() # pop
mylist[len(self.items)-1] # peek
```

### Queue
```python
from Queue import Queue
q=Queue(maxsize=5)
q.put(i)
result = q.get()

# or use deque
import collections
d = collections.deque()
d.append(1) # insert at right
d.appendleft(2) # insert at left
x = d.pop() # pop from right
x = d.popleft() # pop from left
```

### Use of def inside def
```python
    def pathSum(self, root: TreeNode, targetSum: int) -> List[List[int]]:
        ret = list()
        path = list()
        
        def dfs(root: TreeNode, targetSum: int):
            if not root:
                return
            path.append(root.val)
            targetSum -= root.val
            if not root.left and not root.right and targetSum == 0:
                ret.append(path[:])
            dfs(root.left, targetSum)
            dfs(root.right, targetSum)
            path.pop()
        
        dfs(root, targetSum)
        return ret
```
