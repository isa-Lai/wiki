# Java

## Useful Library

```java
//Array
dataType[] arrayRefVar = new dataType[arraySize];
arrayRefVar.length;
int[] nums;
for(int x:nums){} //for each int in nums

//Stack
Deque<Character> stack = new LinkedList<Character>();
stack.pop();
stack.push(num);
stack.isEmpty();
stack.peek();

//Hash Table
Map<T, T> hashtable = new HashMap<T, T>();
hashtable.get(index);
hashtable.put(index,value);
hashtable.containsKey(index);

//Hash Set
Set<Character> occ = new HashSet<Character>();

//Integer
Integer.MIN_VALUE; //-2^31
Integer.MAX_VALUE; //2^31-1

//String
s.length();
s.substring(i,k);  //return substring in string s from index i to k; //not include i
s.substring(i);  //i to the very end
s.charAt(i);  //return char at index i
char[] charArray = s.toCharArray();
```

