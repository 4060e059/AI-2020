# 廻圈loop
## range() 函式
##### rang(整數值)
##### rang(開始值,結束值)
##### rang(開始值,結束值,間隔值)
### rang(整數值)
```
list1=range(10)
print(list1)
```
### rang(開始值,結束值)
##### rang(0,5)，預設是從0開始算,出來的結果會是[0,1,2,3,4]沒有5
```
list2=range(0,5)
print(list(list2))
```
### rang(開始值,結束值,間隔值)
```
list3=range(-4,5,2)
print(list(list3))
```
```
list4=range(-4,6,2)
print(list(list4))
```
## 使用for迴圈
##### 使用for 廻圈 執行固定次數的廻圈運算(通常)
```
for n in range(5):
  print(n)
```
```
for n in range(10):
    print(n, end='@') 
```
##### mysum += 0 是 mysum = mysum + n
```
mysum = 0

for n in range(5):
  mysum += n
  print(mysum)
```
```
mysum = 0

for n in range(5):
  mysum += n

print(mysum)
```
```
x = int(input("請輸入一個正整數:"))
mysum = 0

for n in range(x):
  mysum += n

print(mysum)
```

## Python eval() 函数
##### eval() 函數用來執行一個字符串表達式，並返回表達式的值。
```

```
## 也可以一次輸入多個資料
```

```

