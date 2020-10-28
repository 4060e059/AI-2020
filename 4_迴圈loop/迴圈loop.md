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
