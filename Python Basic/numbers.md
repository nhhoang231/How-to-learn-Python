# Number
---
## Tổng quan
Kiểu dữ liệu Number lưu trữ các giá trị số. Chúng là các kiểu dữ liệu `immutable` - kiểu dữ liệu không thay đổi, các thay đổi về giá trị của kiểu dữ liệu số này sẽ tạo ra một đối tượng được cấp phát mới.

VD:
```python
var1 = 1
var2 = 10
```
Có thể xóa đối tượng = lệnh `del`

```python
del var1[,var2[,var3[....,varN]]]]
```

__Các kiểu hỗ trợ:__
- Kiểu int: kiểu số nguyên không có dấu thập phân.
- Kiểu long: là các số nguyên không giới hạn kích cỡ, được theo sau bởi một chữ l hoặc chữ L.
- Kiểu float: số thực với dấu thập phân. Kiểu này cũng có thể được viết ở dạng số mũ của 10 với E hoặc e như (2.5e2 = 2.5 x 102 = 250).
- Kiểu số phức: là trong dạng a + bJ, với a và b là số thực và J (hoặc j) biểu diễn căn bậc hai của -1. Phần thực là a và phần ảo là b. Nói chung, số phức không được sử dụng nhiều trong lập trình Python.

## Chuyển đổi kiểu số trong Python
Python tự hỗ trợ cơ chế này nhưng có thể thực hiện = tay.

__Các phương thức cơ bản:__
- Để chuyển đổi số x thành số thuần nguyên, `int(x)`.
- Để chuyển đổi số x thành số long,  `long(x)`.
- Để chuyển đổi số x thành số thực, `float(x)`.
- Để chuyển đổi số x thành số phức với phần thực là x và phần ảo là 0, `complex(x)`.
- Để chuyển đổi số x và y thành số phức với phần thực là x và phần ảo là y, `complex(x, y)`.

## Nguồn
http://vietjack.com/python/number_trong_python.jsp

