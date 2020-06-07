# Virtual Environment trong Python
---
## Tổng quan
Virtual Environment hiểu cở bản môi trường ảo. Hỗ trợ tạo, thiết lập một môi trường ảo, cho phép cài đặt thêm các packages của Python mà không làm ảnh hưởng đến những package gốc đã được cài đặt sẵn trên Python.

VD: Muốn thử nghiệm với Django 1.8 trong khi trên hệ thống đang cài đặt Django 1.4 LTS.

Công cụ tạo ra `Virtual Environment` trên Python là `virtualenv`. virtualenv tạo ra một thư mục chứa tất cả những thứ cần thiết (executables, libraries).

## Cài đặt Virtual Environment
__Sử dụng pip:__
```python
pip install virtualenv
```

## Tạo Virtual Environment
__Cú pháp:__
```python
$ virtualenv [project_name]
```
__Có thể tạo một Virtual Environment mà không có các packages đã được cài đặt sẵn__
> Trong trường hợp thiết lập lại

```python
virtualenv --no-site-packages [project_name]
```
## Sử dụng Virtual Environment
Khởi động Virtual Environment bằng câu lệnh:
```python
$ source [project_name]/bin/activate
```

## Thoát khỏi Virtual Environment
__Cú pháp:__
```python
deactivate
```

## Nguồn
https://kipalog.com/posts/Gioi-thieu-Virtual-Environment-trong-Python
http://huyvq.com/blog/tao-moi-truong-lam-viec-ao-voi-virtualenv

