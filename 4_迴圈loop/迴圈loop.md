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
## 跑出奇數的結果
```
numbers = [21, 4, 35, 1, 8, 7, 3, 6, 9]
my_numbers = []

for number in numbers:
  if (number % 2 != 0): 
    my_numbers.append(number)

print(my_numbers)
```
### 底下程式如果第五行改成  if (number % 2 = 0):答案會是甚麼??
```
numbers = [21, 4, 35, 1, 8, 7, 3, 6, 9]
my_numbers = []

for number in numbers:
  if (number % 2 = 0): 
    my_numbers.append(number)

print(my_numbers)
```
## While Loop
### n階程的計算
```
total = i = 1

n = int(input("請輸入正整數 n 的值："))

while(i<=n):
    total *= i  
    i+=1      

print("%d!=%d" % (n, total))
```
## break 指令
##### 我們會希望在迴圈執行到一半的時候就離開迴圈，而不要等到做完一次迴圈裡的所有事情。
```
fruits = ["香蕉","蘋果","橘子","鳳梨","西瓜"]

while True:
    fruit = input("請輸入喜歡的水果(Enter 結束)：")

  #  if (fruit==""):
  #      break

    n = fruits.count(fruit) 
    if (n>0):  # 串列元素存在
        p=fruits.index(fruit)
        print("%s 在串列中的第 %d 項" %(fruit,p+1))
    else:
        print(fruit,"不在串列中!")
```
## continue 指令
##### 在廻圈執行中途暫時停住不往下執行，而跳到廻圈的起始處繼續執行
##### 撰寫一個可以排除數列中 5 的倍數的程式
##### 輸入::一個正整數 n
##### 輸出::
##### 使用者只要輸入一個正整數，
##### 程式會顯示由 1 到該整數的整數數列，但會將 5 的倍數排除
```
n = int(input("請輸入正整數："))

for i in range(1, n+1):
    if i % 5 ==0:
        continue
    print(i,end=" ")
```
### 限制範圍1到6，假如有三個空格可以填(數字不可重複)，請問排序組合
```
for i in range(1,6):
    for j in range(1,5):
        for k in range(1,7):
            if( i != k ) and (i != j) and (j != k):
                print(i,j,k)
```
### 0到18
```
for x in range(19):
  print(x)
```
### 0到18間隔2
```
for x in range(0,19,2):
  print(x)
```
###  20到12
```
for x in range(20,11,-1):
  print(x)
```
### 無法顯示
```
for x in range(0,19,-1):
  print(x)
```
### 把間隔的值貼到後面
```
output = ''

for x in range(0,19,3):
  output += str(x)
  print(output, end=" ")
```
### 如果少了output += str(x)
### 會顯示(0,3,6,9,12,15,18)
```
output = ''

for x in range(0,19,3):
  print(x, end=" ")
```
## 下列程式輸入淨利潤為11111時請問輸出為何?"""
##### 淨利潤:11111
##### 1111.1000000000001
##### 1111.1000000000001
```
i = int(input('淨利潤:'))

arr = [1000000,600000,400000,200000,100000,0]
rat = [0.01,0.015,0.03,0.05,0.075,0.1]
r = 0

for idx in range(0,6):
    if i>arr[idx]:
        r+=(i-arr[idx])*rat[idx]
        print((i-arr[idx])*rat[idx])
        i=arr[idx]

print(r)
```
## 巢狀廻圈Nested Loop
### 九九乘法表
### 廻圈中又包含廻圈的巢狀廻圈　
```
#巢狀迴圈
for i in range(1, 10, 1):
    for j in range(1, 10, 1):
        print(i, 'x', j, '=', i*j)
```
