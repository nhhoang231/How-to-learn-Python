# Class và cách khai báo class trong Python
---
## 1. Khai báo class
Một đối tượng có thể có một hoặc nhiều class và trong mỗi class thì lại chứa một hoặc nhiều các thuộc tính và các phương thức... 

__Cú pháp khai báo Class:__
```python
class className:
    # code
```
__Ý nghĩa:__

- className: Tên class muốn khai báo

## 2. Khai báo thuộc tính 
Một class có thể chứa một hoặc rất nhiều các thuộc tính. Thuộc tính trong class, cũng tương tự như biến ở trong lập trình hướng thủ tục.

__Cú pháp khai báo thuộc tính:__
```python
class Person:
    name = "Lacoski";
    age = 22;
    male = True
```
## 3. Khai báo phương thức trong Class (methods)
Phương thức ở trong hướng đối tượng cũng tương tự như hàm ở trong lập trình hướng thủ tục và một class thì có thể không có hoặc có nhiều phương thức.

__Cú pháp khai báo phương thức__
```python
class Person:
    # thuộc tính
    name = "Lacoski";
    age = 22;
    male = True
    # phương thức
    def setName(self, name):
        self.name = name
    
    def getName(self):
        return self.name
    
    def setAge(self, age):
        self.age = age
    
    def getAge(self):
        return self.age
    
    def setMale(self, male):
        self.male = male
    
    def getMale(self):
        return self.male
```
> Từ khóa `self` thể hiện lại chính class đang chứa nó, và dựa vào nó thì ta có thể truy cập vào các phần tử đang có trong class hiện tại.

## 4. Khởi tạo Class
__Cú pháp khởi tạo Class__
```python
variableName = className()
```

__ý nghĩa thuộc tính__
- `variableName` là biến thể hiện lại đối tượng.
- `className` là class khởi tạo.

VD:
```python
person = Person()
```

Sử dụng dấu `.` để truy cập các thuộc tính, methods 
__Cú pháp:__

```python
# truy cap thuoc tinh
object.propertyName

#truy cap dphuong thuc
object.methodName()
```
ý nghĩa:
- `object` là biến thể hiện tại object.
- `propertyName` là thuộc tính muốn truy xuất.
- `methodName` là phương thức muốn truy xuất.

## Nguồn 
https://toidicode.com/class-va-cach-khai-bao-class-trong-python-357.html
