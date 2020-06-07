# Hàm trong python
---
## Định nghĩa một hàm trong Python
Khi định nghĩa các hàm để cung cấp một tính năng nào đó, bạn cần theo các qui tắc sau:
- Từ khóa def được sử dụng để bắt đầu phần định nghĩa hàm. Def xác định phần bắt đầu của khối hàm.
- def được theo sau bởi ten_ham được theo sau bởi các dấu ngoặc đơn ().
- Các tham số được truyền vào bên trong các dấu ngoặc đơn. Ở cuối là dấu hai chấm.
- Trước khi viết một code, một độ thụt dòng được cung cấp trước mỗi lệnh. Độ thụt dòng này nên giống nhau cho tất cả các lệnh bên trong hàm đó.
- Lệnh đầu tiên của hàm là tùy ý, và nó là Documentation String của một hàm đó.
- Sau đó là lệnh để được thực thi.

## Cú pháp
```python
def ten_ham( cac_tham_so ):
   "function_docstring"
   function_suite
   return [bieu_thuc]
```
VD:
```python
# Phan dinh nghia ham o day
def printme( str ):
   "Chuoi nay duoc truyen vao trong ham"
   print str
   return;

# Bay gio ban co the goi ham printme
printme("Loi goi dau tien toi custom func!")
printme("Loi goi thu hai toi custom func")
```

## Cách gọi hàm
Phần định nghĩa hàm cung cấp thông tin về tên hàm các tham số và định nghĩa những hoạt động nào được thực hiện bởi hàm đó.

Cú pháp như sau:
```python  
ten_ham( cac_tham_so )
```
VD:
```python
# Phan dinh nghia ham o day
def printme( str ):
   "Chuoi nay duoc truyen vao trong ham"
   print str
   return;

# Bay gio ban co the goi ham printme
printme("Loi goi dau tien toi custom func!")
printme("Loi goi thu hai toi custom func")
```

## Hàm có kết quả trả về - `return()`
Hàm return(bieu_thuc) được sử dụng để gửi điều khiển quay trở lại người gọi với bieu_thuc đã cho. Trong trường hợp không cung cấp bieu_thuc, thì hàm return này sẽ trả về None. Nói cách khác, lệnh return được sử dụng để thoát khỏi định nghĩa hàm.
```python
# Phan dinh nghia ham o day
def sum( arg1, arg2 ):
   # Cong hai tham so va tra ve ket qua."
   total = arg1 + arg2
   print "Ben trong ham : ", total
   return total;

# Bay gio ban co the goi ham sum nay
total = sum( 10, 20 );
print "Ben ngoai ham : ", total
```

## Phân biệt tham số và đối số - argument và parameter
Có hai kiểu dữ liệu được truyền trong hàm:
- Dữ liệu được truyền qua lời gọi hàm (argument). Có thể là hằng, biến hoặc biểu thức.
- Dữ liệu được định nghĩa trong hàm (parameter). Là biến để giữ các giá trị đang đến.

VD:
```python
def addition(x,y): # parameter
    		print x+y
x=15
addition(x ,10) # argument
addition(x,x)
y=20
addition(x,y)
```

## Tham số hàm trong Python
Python hỗ trợ các kiểu tham số:
- Tham số bắt buộc
- Tham số mặc định
- Tham số từ khóa (tham số được đặt tên)
- Số tham số thay đổi

### Tham số bắt buộc
VD:
```python
def sum(a,b):
 	c=a+b
  print c

sum(10,20)
sum(20) # chi co a thieu b
```

### Tham số mặc định

```python
def msg(Id,Ten,Age=21):
  print Id
  print Ten
  print Tuoi
  return

msg(Id=100,Ten='Hoang',Age=20)
msg(Id=101,Ten='Thanh') # khong loi vi co mac dinh
```

### Tham số từ khóa
```python
def msg(id,name):
  print id
  print ten
  return

msg(id=100,name='Hoang')
msg(name='Thanh',id=101)
```

### Hàm với số tham số thay đổi
Cú pháp
```python
def tenham([tham_so_chinh_thuc,] *var_args_tuple ):
   "function_docstring"
   function_suite
   return [bieu_thuc]
```

### Hàm nặc danh
Hàm nặc danh (hàm vô danh), hiểu theo cách đơn giản, là hàm không có tên và chúng không được khai báo theo cách chính thức bởi từ khóa def. Để khai báo hàm này, sử dụng từ khóa lambda.

Cú pháp:
```python
lambda [arg1 [,arg2,.....argn]]:bieu_thuc
```

VD:
```python
#Phan dinh nghia ham
square=lambda x1: x1*x1

#Goi square nhu la mot ham
print "Binh phuong cua so la",square(10)
```

## Nguồn
http://vietjack.com/python/ham_trong_python.jsp

