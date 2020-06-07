# String
---
## Giới thiệu
String là một trong các kiểu phổ biến nhất trong Python. String trong Python là immutable. Có thể tạo các chuỗi bằng cách bao một text trong một trích dẫn đơn hoặc trích dẫn kép. Python coi các lệnh trích dẫn đơn và kép là như nhau.

Ví dụ:
```python
var1 = 'Hello World!'
var2 = "Python Programming"
```

## Truy cập các giá trị trong String
> Python không hỗ trợ một kiểu chữ cái; chúng được coi như các chuỗi có độ dài là 1.

String được lưu giữ dưới dạng các ký tự đơn trong vị trí ô nhớ liên tiếp nhau. Lợi thế của sử dụng String là nó có thể được truy cập từ cả hai hướng (tiến về trước forward hoặc ngược về sau backward).

 __Cơ chế:__
- Chỉ mục với hướng forward bắt đầu với 0,1,2,3,…
- Chỉ mục với hướng backward bắt đầu với -1,-2,-3,…
VD:

```python
var1 = 'Hello World!'
var2 = "Python Programming"

print "var1[0]: ", var1[0]
print "var2[1:5]: ", var2[1:5]

#KQ
var1[0]:  H
var2[1:5]:  ytho
```

## Cập nhật String
Cập nhật một chuỗi đang tồn tại bằng cách gán (hoặc tái gán) một biến cho string khác. Giá trị mới có thể liên quan hoặc khác hoàn toàn giá trị trước đó.

VD:
```python
var1 = 'Hello World!'

print "Chuoi hien tai la :- ", var1[:6] + 'Python'

#KQ
Chuoi hien tai la :-  Hello Python
```

## Các ký tự đặc biệt (xem thêm)

## Thao tác với String
Có ba kiểu toán tử được hỗ trợ bởi String:
- Toán tử cơ bản
- Toán tử membership
- Toán tử quan hệ

### Các toán tử cơ bản để thao tác với String
__Toán tử nối chuỗi `+`__

VD:
```python
"hoang" + "nam"

#KQ
'hoangnam'
```
> Cả hai toán hạng được truyền cho phép nối chuỗi này phải cùng kiểu, nếu không sẽ tạo một lỗi.

__Toán tử lặp chuỗi `*`__

VD:
```python
5*"Hoang"

#KQ
'HoangHoangHoangHoangHoang'
```

### Các toán tử membership
- Toán tử in: trả về true nếu một ký tự là có mặt trong chuỗi đã cho, nếu không nó trả về false.
- Toán tử not in: trả về true nếu một ký tự là không tồn tại trong chuỗi đã cho, nếu không nó trả về false.

VD:
```python
>>> str1="javapoint"
>>> str2='sssit'
>>> str3="seomount"
>>> str4='java'
>>> st5="it"
>>> str6="seo"
>>> str4 in str1
True
>>> str5 in str2
>>> st5 in str2
True
>>> str6 in str3
True
>>> str4 not in str1
False
>>> str1 not in str4
True
```

### Các toán tử quan hệ
Tất cả các toán tử quan hệ `(như <,>, <=, >=, ==, !=, <>)` cũng có thể áp dụng cho các String.

VD:
```python
>>> "HOANG"=="HOANG"
True
>>> "afsha">='Afsha'
True
>>> "Z"<>"z"
True
```

### Dấu chia chuỗi []
__Cú pháp:__

```python
<ten_chuoi>[chi_muc_bat_dau:chi_muc_ket_thuc]
hoac
<ten_chuoi>[:chi_muc_ket_thuc]
hoac
<ten_chuoi>[chi_muc_bat_dau:]
```

VD:
```python
>>> str="Nikhil"
>>> str[0:6]
'Nikhil'
>>> str[0:3]
'Nik'
>>> str[2:5]
'khi'
>>> str[:6]
'Nikhil'
>>> str[3:]
'hil'
```

## Toán tử định dạng chuỗi
Một trong những đặc điểm hay nhất trong Python là toán tử định dạng chuỗi %

VD:
```python
print "Ten toi la %s va toi nang %d kg!" % ('Hoang', 80)
```

## Nguồn
http://vietjack.com/python/string_trong_python.jsp

