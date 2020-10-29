# python決策與選擇結構
```
if
if ...else
if ...elsif
if ...elsif ...else
各種判斷條件
AND
OR
```
```
單一條件判斷 if 對的才會做
單一條件判斷 if ...else 二選一
多重條件判斷 if ...elsif ...else 多選一
```
## 讀取使用者輸入
##### python輸入:raw_input 跟 input
```
x = input('請輸入名字:')
print('Hello, ' + x)
```
##### 使用Python內建的type()函數顯示資料型態
```
type(a)
```
## 使用者如果直接輸入計算會錯誤
```
a = input("請輸入：")
a

b=a+1
b
```
## Python eval() 函数
##### eval() 函數用來執行一個字符串表達式，並返回表達式的值。
```
a = eval(input("請輸入："))
a

b=a+1
b
```
## 也可以一次輸入多個資料
```
a,b = eval(input("請輸入兩個數位："))
a,b
```

