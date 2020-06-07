# Làm việc với File
---
## Giới thiệu
Python cung cấp nhiều cách tiện lợi để làm việc với file. Một file là một nơi lưu trữ ngoại vi trên hard disk, tại đó dữ liệu có thể được lưu trữ và thu nhận.

## Mở file
Trước khi làm việc với File, ta cần mở File. Để mở một File, Python cung cấp hàm `open()`. Nó trả về một đối tượng File mà được sử dụng với các hàm khác.

__Cú pháp__
```python
doi_tuong_file = open(ten_file [, access_mode][, buffer])
```
> `ten_file` là tên File muốn truy cập.

> `access_mode` xác định chế độ của File đã được mở. Mode phụ thuộc vào các hoạt động muốn thực hiện trên File. Chế độ truy cập mặc định là read.

> `buffer`: Nếu buffer được thiết lập là 0, sẽ không có trình đệm nào diễn ra. Nếu xác định là 1, thì trình đệm dòng được thực hiện trong khi truy cập một File. Nếu là số nguyên lớn hơn 1, thì hoạt động đệm được thực hiện với kích cỡ bộ đệm đã cho. Nếu là số âm, thì kích cỡ bộ đệm sẽ là mặc định (hành vi mặc định).


## Đóng File
Sau khi thực hiện xong các hoạt động trên File thì ta cần đóng File đó. Python tự động đóng một File khi đối tượng tham chiếu của một File đã được giải phóng hoặc thu hồi. Tuy nhiên cần thao tác tay để bảo đảm dữ liệu.

__Cú pháp__
```python
fileObject.close();
```

## Đọc File
__Cú pháp__
```python
doi_tuong_file.read(giatri);  
```

## Ghi File
__Cú pháp__
```python
doi_tuong_file.write(string);  
```

VD:
```python
obj=open("abcd.txt","w")
obj.write("Python xin chao cac ban")
obj.close()
obj1=open("abcd.txt","r")
s=obj1.read()
print s
obj1.close()
obj2=open("abcd.txt","r")
s1=obj2.read(20)
print s1
obj2.close()

# KQ
```

## Các thuộc tính của File
- `file.closed` -	Trả về true nếu file đã được đóng, nếu không là false
- `file.mode` -	Trả về chế độ truy cập nào mà file đã mở với
- `file.name` - Trả về tên file
- `file.softspace` - Trả về false nếu space được yêu cầu tường minh với print, nếu không là true

## Các chế độ truy cập file (xem thêm docs)
| Mode | Miêu tả                                                                                                                                 |
|------|-----------------------------------------------------------------------------------------------------------------------------------------|
| r    | Mở file trong chế độ đọc, đây là chế độ mặc định. Con trỏ tại phần bắt đầu của File                                                     |
| rb   | Mở file trong chế độ đọc cho định dạng nhị phân, đây là chế độ mặc định. Con trỏ tại phần bắt đầu của File                              |
| r+   | Mở file để đọc và ghi. Con trỏ tại phần bắt đầu của File                                                                                |
| w    | Mở File trong chế độ ghi. Nếu file đã tồn tại, thì ghi đè nội dung của file đó, nếu không thì tạo một file mới                          |
| wb   | Mở File trong chế độ ghi trong định dạng nhị phân. Nếu file đã tồn tại, thì ghi đè nội dung của file đó, nếu không thì tạo một file mới |
| w+   | Mở file để đọc và ghi. Nếu file tồn tại thì ghi đè nội dung của nó, nếu file không tồn tại thì tạo một file mới để đọc và ghi           |
| a    | Mở file trong chế độ append. Con trỏ là ở cuối file nếu file này đã tồn tại. Nếu file không tồn tại, thì tạo một file mới để ghi        |
| a+   | Mở file trong để đọc và append. Con trỏ file tại cuối nếu file đã tồn tại. Nếu không tồn tại thì tạo một file mới để đọc và ghi         |

## Nguồn
http://vietjack.com/python/file_io_trong_python.jsp

