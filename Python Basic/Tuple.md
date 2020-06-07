# Tuple
---
## Giới thiệu
Tuple là một dãy các đối tượng không thay đổi (immutable) trong Python, vì thế tuple không thể bị thay đổi. Các tuple cũng là các dãy giống như List.

Không giống List mà sử dụng các dấu ngoặc vuông, thì tuple sử dụng các dấu ngoặc đơn `()`.

VD:
```python
>>> data=(10,20,'ram',56.8)
>>> data2="a",10,20.9
>>> data
(10, 20, 'ram', 56.8)
>>> data2
('a', 10, 20.9)
>>>
```
> Nếu các dấu ngoặc đơn không được cung cấp với một dãy, thì nó được coi như là tuple.

```python
# Tuple trống
tup1 = ()

# Tuple chỉ có một giá trị đơn
tup1 = (50,)

# Các tuple cũng có thể được lồng vào nhau
tupl1='a','hoang',10.56
tupl2=tupl1,(10,20,30)

print tupl1
print tupl2

##KQ
('a', 'hoang', 10.56)
(('a', 'hoang', 10.56), (10, 20, 30))
```
## Truy cập các giá trị trong tuple
Truy cập tương tự list
```python
tup1 = ('vatly', 'hoahoc', 1997, 2000);
tup2 = (1, 2, 3, 4, 5, 6, 7 );

print "tup1[0]: ", tup1[0]
print "tup2[1:5]: ", tup2[1:5]

# KQ
tup1[0]:  vatly
tup2[1:5]:  [2, 3, 4, 5]
```

## Sử dụng tuple
Giống như String và List, có thể sử dụng toán tử nối + và toán tử lặp *.

> Điểm khác biệt là nó tạo ra một tuple mới, không tạo ra một chuỗi hay list.

VD:
```python
data1=(1,2,3,4)
data2=('x','y','z')
data3=data1+data2
print data1
print data2
print data3

# KQ
(1, 2, 3, 4)
('x', 'y', 'z')
(1, 2, 3, 4, 'x', 'y', 'z')
```

## Xóa tuple
> Xóa các phần tử đơn của tuple là điều không thể. Chỉ có thể xóa toàn bộ tuple

VD
```python
data=(10,20,'hoang',40.6,'z')
print data
del data      #se xoa du lieu cua tuple
print data	#se hien thi mot error boi vi tuple da bi xoa
```

## Cập nhật tuple
> Các phần tử của Tuple không thể được cập nhật. Vì tình chất `immutable`

Để cập nhật cần tạo tuple mới trên tuple cũ
```python
data1=(10,20,30)
data2=(40,50,60)
data3=data1+data2
print data3

# KQ
(10, 20, 30, 40, 50, 60)
```

## Tại sao sử dụng tuple?
- Trình xử lý các tuple là `nhanh hơn các` List.
- Làm cho `dữ liệu an toàn` hơn bởi vì tuple là không thay đổi (immutable) và vì thế nó không thể bị thay đổi.
- Các tuple được sử dụng để định dạng String.

## Nguồn
http://vietjack.com/python/tuple_trong_python.jsp

