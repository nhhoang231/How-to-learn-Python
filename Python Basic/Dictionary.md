# Dictionary
---
Dictionary là một tập hợp các cặp key và value không có thứ tự. Nó là một container mà chứa dữ liệu, được bao quanh bởi các dấu ngoặc móc đơn `{}`.

Mỗi cặp `key-value` được xem như là một item. Key mà đã truyền cho item đó phải là duy nhất, trong khi đó value có thể là bất kỳ kiểu giá trị nào. `Key` phải là một kiểu dữ liệu không thay đổi `(immutable)` như chuỗi, số hoặc tuple.

Key và value được phân biệt riêng rẽ bởi một dấu hai chấm `(:)`. Các item phân biệt nhau bởi một dấu phảy `(,)`.

VD:
```python
data={100:'Hoang', 101:'Nam', 102:'Binh'}
print data

# KQ
{100: 'Hoang', 101: 'Nam', 102: 'Binh'}
```

## Các thuộc tính của key
- Key phải là duy nhất, nếu key bị lặp kết quả gán cuối cùng sẽ được công nhận
- Key phải thuộc dạng `immutable`, như list hoặc số, tuple

## Truy cập các giá trị trong Dictionary
Không thể truy cập bằng chỉ mục trong Dictionary, các giá trị trong Dictionary có thể được truy cập thông qua các key.

__Cú pháp:__
```python
<ten_dictionary>[key]
```

VD:
```python
data1={'Id':100, 'Ten':'Hoang', 'Nghenghiep':'Developer'}
data2={'Id':101, 'Ten':'Nam', 'Nghenghiep':'Trainer'}
print "Id cua nhan vien dau tien la",data1['Id']
print "Id cua nhan vien thu hai la",data2['Id']
print "Ten cua nhan vien dau tien la:",data1['Ten']
print "Nghe nghiep cua nhan vien thu hai la:",data2['Nghenghiep']
```

## Cập nhật Dictionary
Item (cặp key-value) có thể cập nhật. Kiểu cho phép thêm một entry mới hoặc một cặp key-value mới, sửa đổi một entry đã tồn tại.

VD:
```python
data1={'Id':100, 'Ten':'Hoang', 'Nghenghiep':'Developer'}
data2={'Id':101, 'Ten':'Nam', 'Nghenghiep':'Trainer'}
data1['Nghenghiep']='Manager' # sửa
data2['Mucluong']=17000000    # Thêm mới
data1['Mucluong']=12000000    # Them mới
print data1
print data2
```

## Xóa phần tử Dictionary
Kiểu cho phép có thể xóa một phần tử đơn hoặc xóa toàn bộ nội dung của Dictionary. Sử dụng lệnh del để thực hiện các hoạt động này.

__Cú pháp__
```python
# Xoa phan tu
del ten_dictionary[key]

# Xoa toan bo
del ten_dictionary
```

VD:
```python
data={100:'Hoang', 101:'Thanh', 102:'Nam'}
del data[102]
print data
del data

#KQ
{100: 'Hoang', 101: 'Thanh'}
```

## Nguồn
http://vietjack.com/python/dictionary_trong_python.jsp

