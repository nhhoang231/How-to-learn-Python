# List
---
## Giới thiệu
Cấu trúc dữ liệu cơ bản nhất trong Python là dãy (sequence). Mỗi phần tử trong dãy được gán một số, là vị trí hoặc chỉ mục của nó. Chỉ mục đầu tiên là 0, chỉ mục thứ hai là 1, và …

Python có sáu kiểu dãy đã được xây dựng sẵn, hai kiểu được sử dụng phổ biến nhất là List và Tuple.

## List trong Python
List trong Python là cấu trúc dữ liệu mà có khả năng lưu giữ các kiểu dữ liệu khác nhau.

List trong Python là thay đổi (mutable), nghĩa là Python sẽ không tạo một List mới nếu bạn sửa đổi một phần tử trong List.

List là một container mà giữ các đối tượng khác nhau trong một thứ tự đã cho. Các hoạt động khác nhau như chèn hoặc xóa có thể được thực hiện trên List.

Một List có thể được tạo ra bởi lưu trữ một dãy các kiểu giá trị khác nhau được phân biệt bởi các dấu phảy. Dưới đây là cú pháp để tạo List:

__Cú pháp:__
```python
<ten_list>=[giatri1, giatri2, ..., giatriN];
```

VD:
```python
list1 = ['vatly', 'hoahoc', 1997, 2000];
list2 = [1, 2, 3, 4, 5 ];
list3 = ["a", "b", "c", "d"];
```
> Một List trong Python được bao xung quanh bởi các dấu ngoặc vuông [].

> Tương tự như chỉ mục của chuỗi, chỉ mục của List bắt đầu từ 0.

## Truy cập các giá trị trong List
__Cú pháp:__

```python
<ten_list>[index]
```
VD:
```python
list1 = ['vatly', 'hoahoc', 1997, 2000];
list2 = [1, 2, 3, 4, 5, 6, 7 ];

print "list1[0]: ", list1[0]
print "list2[1:5]: ", list2[1:5]

#KQ:
list1[0]:  vatly
list2[1:5]:  [2, 3, 4, 5]
```

## Các hoạt động cơ bản trên List
Có thể thực hiện các hoạt động nối với toán tử `+` hoặc hoạt động lặp với `*` như trong các chuỗi. Điểm khác biệt là ở đây nó tạo một List mới, không phải là một chuỗi.

VD:
```python
list1=[10,20]
list2=[30,40]
list3=list1+list2
print list3

#KQ
[10, 20, 30, 40]
```

> Toán tử + ngụ ý rằng cả hai toán hạng được truyền cho nó phải là List, nếu không sẽ báo lỗi

## Cập nhật List
__Cú pháp:__
```python
<ten_list>[index]=<giatri>
```

VD:
```python
list = ['vatly', 'hoahoc', 1997, 2000];

print "Gia tri co san tai chi muc thu 2 : "
print list[2]
list[2] = 2001;
print "Gia tri moi tai chi muc thu 2 : "
print list[2]

#KQ:
Gia tri co san tai chi muc thu 2 :
1997
Gia tri moi tai chi muc thu 2 :
2001
```

## Nguồn
http://vietjack.com/python/list_trong_python.jsp

