# Constructor và destructor trong Python
---
## 1. Phương thức khởi tạo - constructor
Phương thức khởi tạo là một phương thức đặc biệt ở trong class, phương thức này mặc định sẽ được gọi khi khởi tạo class. Phương thức được dùng để khởi tạo các thuộc, xử lý phương thức hoặc là dùng để nhận các tham số truyền vào class khi khởi tạo.

__Cú pháp__
```python
class className:
    def __init__(self, param1, param2,...):
```

Ý nghĩa:
- `className` là tên class.
- `param1, param2,...` là các tham số muốn nhận khi kèm khi khởi tạo class.

VD:
```python
class Person:
    def __init__(self):
        print("Class person được khởi tạo!")
        
person = Person()

# KQ: 
Class person được khởi tạo!
```

## 2. Phương thức hủy bỏ - deconstructor
Trái ngược với phương thức khởi tạo, thì phương thức hủy sẽ được gọi khi class được hủy,. Phương thức dùng để giải phóng tài nguyên của class.

__Cú pháp khai báo:__
```python
def __del__(self):
    # code
```

> Khai báo một phương thức có tên là `__del__`

VD:
```python
class Person:
    def __init__(self, name, age, male):
        print("Class person được khởi tạo!")
        print("Name: %s - Age: %d - Male: %d" %(name, age, male))
    def __del__(self):
        print('Class Person được hủy')
person = Person('Nguyen Huy Hoang', 21, True)
# kết quả: 
# Class person được khởi tạo!
# Name: Nguyen Huy Hoang - Age: 21 - Male: 1
# Class Person được hủy
```

## Nguồn
https://toidicode.com/constructor-va-destructor-trong-python-358.html
