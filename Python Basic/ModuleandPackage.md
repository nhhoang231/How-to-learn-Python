# Module và Package trong Python
---
## Module
### Tổng quan
Module được sử dụng để phân loại code thành các phần nhỏ hơn liên quan với nhau. Đơn giản, Module hỗ trợ tổ chức Python code một cách logic, dễ dang cho việc tìm kiếm, sử dụng lại.

Module là một đối tượng với các thuộc tính có thể đặt tên tùy ý, có thể gắn kết và tham chiếu.

Về cơ bản, một Module là một file, chia thành các lớp, hàm và biến được định nghĩa. Tất nhiên, một Module cũng có thể bao gồm code có thể chạy.

Ưu điểm:
- `Khả năng tái sử dụng`: Module có thể được sử dụng ở trong phần Python code khác, do đó làm tăng tính tái sử dụng code.
- `Khả năng phân loại`: Các kiểu thuộc tính tương tự nhau có thể được đặt trong một Module.

### Để import một Module
#### Sử dụng lệnh import trong Python
__Cú pháp__  
```python
import module1[, module2[,... moduleN]
```
VD:
```python
# file cùng cấp
# Tại file: addition.py
def add(a,b):
  c=a+b
  print c
  return
# Tại file: msg.py
def msg_method():
    print "Hom nay troi mua"
    return

# Tại file: main.py
import addition, msg
addition.add(10,20)
addition.add(30,40)
msg.msg_method()

```

#### Lệnh from…import
Sử dụng để import thuộc tính cụ thể từ một Module. Trong trường hợp mà bạn không muốn import toàn bộ Module nào đó thì bạn có thể sử dụng lệnh này.

__Cú pháp__
```python
from modname import name1[, name2[, ... nameN]]
```

VD:
```python
# area.py
def circle(r):
    print 3.14*r*r
    return

def square(l):
    print l*l
    return

def rectangle(l,b):
    print l*b
    return

def triangle(b,h):
    print 0.5*b*h
    return

# main.py
from area import square,rectangle
square(10)
rectangle(2,5)
```

#### Lệnh from…import*
Sử dụng import toàn bộ Module

__Cú pháp__
```python
from modname import *
```

#### Built-in Module
Rất nhiêu Module đã được xây dựng sẵn trong Python. VD: math, random, threading, collections, os, mailbox, string, time, … Mỗi Module được định nghĩa sẵn rất nhiều hàm, sử dụng để thực hiện các tính năng khác nhau.

```python
import math
a=4.6
print math.ceil(a)
print math.floor(a)
b=9
print math.sqrt(b)
print math.exp(3.0)
print math.log(2.0)
print math.pow(2.0,3.0)
print math.sin(0)
print math.cos(0)
print math.tan(45)
```

## Package
### Tổng quan
Package là một tập hợp các Module, sub-package, … tương tự nhau. Đó là một cấu trúc có thứ bậc của thư mục và file.

### Cách tạo, import package
- Bước 1: Tạo một thư mục, có tên là PackageTest.
- Bước 2: Đặt các module khác nhau bên trong thư mục PackageTest
  - msg1.py: msg1()
  - msg2.py: msg2()
  - msg3.py: msg3().
- Bước 3: Tạo một `__init__.py` file để xác định các thuộc tính trong mỗi Module.
- Bước 4: import package và sử dụng các thuộc tính trong package.

VD:
```python
# 1. Tạo thư mục
mkdir PackageTest
# 2. Tại file
touch msg1.py msg2.py msg3.py
## msg1.py
def msg1():
    print "Day la msg1"
## msg2.py
def msg2():
    print "Day la msg2"
## msg3.py
def msg3():
    print "Day la msg3"

# 3. Tạo `__init__.py`
from msg1 import msg1
from msg2 import msg2
from msg3 import msg3

# 4. Import package
import PackageTest
PackageTest.msg1()
PackageTest.msg2()
PackageTest.msg3()
```

> __init__.py file

> file được sử dụng để xem xét các thư mục trên disk dưới dạng package của Python. Về cơ bản, file này được sử dụng để khởi tạo các Package trong Python.

![](images/module-package-1.png)

