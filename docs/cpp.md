# C++

## Basic
- Print using `std::cout << "print message";`

## Class

### Vector
```cpp
std::vector<float> x;

//initialize
x.resize(size, initial_value);

//sub array

```

## Pointer

### Function
```cpp
void test1 (float x){
  x = 1;
}
void test2 (float &x){
  x = 1;
}

int main()
{
    float t = 2.0;
    test1(t); // t = 2
    test2(t); // t = 1
    return 0;
}

```
