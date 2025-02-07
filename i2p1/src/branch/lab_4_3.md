## Lab 4-3: 計算機輸入檢查及例外處理 (20%)

* 輸入：
  1. 要執行的計算功能，分別如下：
     1. 加 (`+`)
     2. 減 (`-`)
     3. 乘 (`*`)
     4. 除 (`/`)
     5. 取餘數 (`%`)
  2. 兩個以 10 為底的實數。
  實數的正負號 (sign)、實數的尾數 (mantissa，1/100,000,000)、實數的指數部分 (exponent)。
  正負號輸入大於等於 0 為正數，小於 0 為負數。
  尾數部分不超過 9 位數字。
  指數部分為 -38 至 +38。
  第二個實數為任意非 `0` 的數字。
  若為取餘數運算，兩數皆須為整數，且第二個整數需不為 `0`。
* 輸出：所選擇的運算子字元 (i.e. `+`, `-`, `*`, `/`)及兩實數的運算結果，以科學記號表示，有效位數為 15 位。若輸入不合法的數字則需顯示 `Invalid input: <input>` 並結束程式。 (e.g. `Invalid input: 1234567890`)。
* 檔名：lab4_3_<學號>.cpp (e.g. lab4_3_106062802.cpp)

程式需提示使用者輸入需要的運算功能，輸出該運算功能的運算子字元。
程式需檢查使用者輸入的是否符合題目要求，不合法的輸入需在當下的輸入完成後顯示 `Invalid input: <user input>` 並結束程式。
不合法輸出格式範例請參考以下範例。
使用者會在每次輸入時輸入任意實數，請考慮所有數字輸入的可能性。

```text
Simple scientific calculator
1) plus (+)
2) minus (-)
3) multiplication (*)
4) division (/)
5) modulation (%)
Please select the operator: <1-5>
You selected: <+, -, *, /, %>
Input real number (a), sign: <sign a>
Input real number (a), mantissa: <mantissa a>
Input real number (a), exponent: <exponent a>
Input real number (b), sign: <sign b>
Input real number (b), mantissa: <mantissa b>
Input real number (b), exponent: <exponent b>
The real number (a) is: <output real number a>
The real number (b) is: <output real number b>
(a) <+, -, *, /, %> (b) = <result>
```

Example:

```console
$ ./a.out
Simple scientific calculator
1) plus (+)
2) minus (-)
3) multiplication (*)
4) division (/)
5) modulation (%)
Please select the operator: 3
You selected: *
Input real number (a), sign: -100
Input real number (a), mantissa: 123456789
Input real number (a), exponent: 10
Input real number (b), sign: -10
Input real number (b), mantissa: 123456788
Input real number (b), exponent: 10
The real number (a) is: -1.23456789e+10
The real number (b) is: -1.23456788e+10
(a) * (b) = 1.52415786267337e+20

$ ./a.out
Simple scientific calculator
1) plus (+)
2) minus (-)
3) multiplication (*)
4) division (/)
5) modulation (%)
Please select the operator: 6
Invalid input: 6

$ ./a.out
Simple scientific calculator
1) plus (+)
2) minus (-)
3) multiplication (*)
4) division (/)
5) modulation (%)
Please select the operator: 4
You selected: /
Input real number (a), sign: 0
Input real number (a), mantissa: 12345678912
Invalid input: 12345678912

$ ./a.out
Simple scientific calculator
1) plus (+)
2) minus (-)
3) multiplication (*)
4) division (/)
5) modulation (%)
Please select the operator: 4
You selected: /
Input real number (a), sign: -100
Input real number (a), mantissa: 123456789
Input real number (a), exponent: 10
Input real number (b), sign: -10
Input real number (b), mantissa: 0
Invalid input: 0
```
