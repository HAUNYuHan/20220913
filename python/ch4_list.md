## list
```
list1 = ["小明","Gudio",666,True]
print(list1)
```
```
list1 = ["小明","Gudio",666,True]
print(list1)
```
- append()
```
list1.append("小張")
print(list1)
```
```
['小明', 'Gudio', 666, True, '小張']
```
- extend()
```
list1.extend(["小王","小李"])
print(list1)
```
```
['小明', 'Gudio', 666, True, '小張', '小王', '小李']
```
- insert()
```
list1.insert(1,"小杜")
print(list1)
```
```
list1.insert(1,"小杜")
print(list1)
```
- +
```
list2 = ["小巴","小新","阿尼亞"]
list3 = list2 + list1
print(list3)
```
```
['小巴', '小新', '阿尼亞', '小明', '小杜', 'Gudio', 666, True, '小張', '小王', '小李']
```
- index
```
num = list3.index("小杜")
print(num)
```
```
4
```
- in
```
check1 = "小新" in list3
check2 = "蠟筆" in list3
print(check1)
print(check2)
```
```
True
False
```
- for
```
for i in list3:
  if "小新" == i:
    print("存在")
    break
```
```
存在
```
### 修改
```
list3[5]="王八"
print(list3)
```
```
['小巴', '小新', '阿尼亞', '小明', '小杜', '王八', 666, True, '小張', '小王', '小李']
```
- clear()
```
list1.clear()
print(list1)
```
```
[]
```
- pop()
```
list3.pop(6)
print(list3)
```
```
['小巴', '小新', '阿尼亞', '小明', '小杜', '王八', True, '小張', '小王', '小李']
```
- remove()
```
list3.remove(True)
print(list3)
```
```
['小巴', '小新', '阿尼亞', '小明', '小杜', '王八', '小張', '小王', '小李']
```
- del
```
del list3[5:8]
print(list3)
```
```
['小巴', '小新', '阿尼亞', '小明', '小杜']
```
### 分片
```
print(list3)
print(list3[0:])
print(list3[:4])
print(list3[2:3])
```
```
['小巴', '小新', '阿尼亞', '小明', '小杜']
['小巴', '小新', '阿尼亞', '小明', '小杜']
['小巴', '小新', '阿尼亞', '小明']
['阿尼亞']
```
### sort()
```
a = [9,8,7,6,5]
b = ["zxc","asd","qwe","vbn"]
a.sort()
b.sort()
print(a)
print(b)
```
```
[5, 6, 7, 8, 9]
['asd', 'qwe', 'vbn', 'zxc']
```
