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

## Data Type Conversion

### Implicit and Explicit
**(byte，short，char)->int->long->float->double**
Form narrow to wide is **Implicit**, from wide to narrow is **Explicit**.
byte,short,char are on the same level, they cannot be converted to each other.
```java
long a = 1;
float b = a; //automatic
int c = (int)a; //explicit
```

### Using Class
**Boolean, Character, Integer, Long, Float and Double**
```java
// double to int
double d=100.00;
System.out.println(d);//100.00
Double D=new Double(d);
System.out.println(D);//100.00
int i=D.intValue();
System.out.println(i);//100
//int to double
int i=200;
System.out.println(i);//200
double d=i;
System.out.println(d);//200.0
```

### String
**Boolean, Character, Integer, Long, Float and Double** can use toString();
Basic Data Type can use String.valueOf(num);

### Date
```java
import java.text.SimpleDateFormat;
import java.util.Date;

class convert {
 public static void main(String[] args) {
    Date date = new Date();
    SimpleDateFormat sy1=new SimpleDateFormat("yyyyMMdd");
    String dateFormat=sy1.format(date);
    System.out.println(dateFormat);//20210504
    SimpleDateFormat sy=new SimpleDateFormat("yyyy");
    String year=sy.format(date);
    System.out.println(year);//2021
    SimpleDateFormat sm=new SimpleDateFormat("MM");
    String month=sm.format(date);
    System.out.println(month);//05
    SimpleDateFormat sd=new SimpleDateFormat("dd");
    String day=sd.format(date);
    System.out.println(day);//04
 }
}   
```




