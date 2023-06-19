**To Build:**

```
g++ -std=c++17 -c main.cpp -o main.o
g++ -std=c++17 -c other.cpp -o other.o
g++ -std=c++17 -O3 other.o main.o -o test
```

**Inspect:**

```
/tmp $ strings test |grep BYTERANGE
```
**Output:**

```
#EXT-X-BYTERANGE:
#EXT-X-BYTERANGE:
```

ie, binary contains 2 seperate strings.
