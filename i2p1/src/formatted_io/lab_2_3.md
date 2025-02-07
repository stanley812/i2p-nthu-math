## Lab 2-3: 正實數乘法 (20%)

* 輸入：兩正實數的整數部分、正實數的小數部分 (1/10,000,000,000)，正實數的小數部分不超過 10 位數。
* 輸出：兩正實數數值、兩正實數的積，並且以 `double` 形式搭配 `std::setprecision(15)` 輸出。
* 檔名：lab2_3_<學號>.cpp (e.g. lab2_3_106062802.cpp)

程式需提示使用者輸入兩正實數的整數部分、正實數的小數部分，程式需輸出兩正實數數值、兩正實數的積。

```text
Input real number (a), before decimal point: <(a) before decimal point>
Input real number (a), after decimal point: <(a) after decimal point>
The real number is: <real number (a)>
Input real number (b), before decimal point: <(b) before decimal point>
Input real number (b), after decimal point: <(b) after decimal point>
The real number is: <real number (b)>
(a) * (b) = <real number (a) * (b)>
```

Example:

```console
$ ./a.out
Input real number (a), before decimal point: 1
Input real number (a), after decimal point: 2000000000
The real number (a) is: 1.2
Input real number (b), before decimal point: 12
Input real number (b), after decimal point: 3000000000
The real number (b) is: 12.3
(a) * (b) = 14.76

$ ./a.out
Input real number (a), before decimal point: 1
Input real number (a), after decimal point: 2000000000
The real number (a) is: 1.2
Input real number (b), before decimal point: 12
Input real number (b), after decimal point: 3
The real number (b) is: 12.0000000003
(a) * (b) = 14.40000000036
```
