# Cú pháp Python
---
## Định danh (identifier) trong Python
Một định danh `(identifier)` là một tên được sử dụng để nhận diện một biến, một hàm, một lớp, hoặc một đối tượng.

Một định danh bắt đầu với một chữ cái từ A tới Z hoặc từ a tới z hoặc một dấu gạch dưới (_) được theo sau bởi 0 hoặc nhiều ký tự, dấu gạch dưới hoặc các chữ số (từ 0 tới 9).

> Python không hỗ trợ các Punctuation char chẳng hạn như @, $ và % bên trong các định danh.

Python là một ngôn ngữ lập trình phân biệt chữ hoa - chữ thường, do đó Thanh và thanh là hai định danh khác nhau.

Một số qui tắc nên được sử dụng trong khi đặt tên các định danh:
- Một định danh là một dãy ký tự hoặc chữ số.

- Không có ký tự đặc biệt nào được sử dụng (ngoại trừ dấu gạch dưới) như một định danh. Ký tự đầu tiên có thể là chữ cái, dấu gạch dưới, nhưng không được sử dụng chữ số làm ký tự đầu tiên.

- Từ khóa không nên được sử dụng như là một tên định danh (phần dưới sẽ trình bày về khác từ khóa này).

- Tên lớp bắt đầu với một chữ cái hoa. Tất cả định danh khác bắt đầu với một chữ cái thường.

- Bắt đầu một định danh với một dấu gạch dưới đơn chỉ rằng định danh đó là private.

- Bắt đầu một định danh với hai dấu gạch dưới chỉ rằng định danh đó thực sự là private.

- Nếu định danh cũng kết thúc với hai dấu gạch dưới, thì định danh này là một tên đặc biệt được định nghĩa bởi ngôn ngữ (ví dụ như __init__ chẳng hạn).

## Dòng lệnh và độ thụt dòng lệnh trong Python
Python không cung cấp các dấu ngoặc ôm ({}) để chỉ các khối code cho định nghĩa lớp hoặc hàm hoặc điều khiển luồng. Các khối code được nhận biết bởi độ thụt dòng code `(indentation)` trong Python và đây là điều bắt buộc.

Số khoảng trống trong độ thụt dòng là biến đổi, nhưng tất cả các lệnh bên trong khối phải được thụt cùng một số lượng khoảng trống như nhau.

Ví dụ:
```python
if True:
  print "True"
else:
  print "False"

if True:
  print "Answer"
  print "True"
else:
  print "Answer"
  print "False"
```

## Các lệnh trên nhiều dòng trong Python
Python cho phép sử dụng ký tự \ để chỉ rõ sự liên tục dòng.
```python
total = item_one + \
        item_two + \
        item_three
```
Các lệnh được chứa bên trong các dấu ngoặc [], {}, hoặc () thì không cần sử dụng ký tự \.
```python
days = ['Monday', 'Tuesday', 'Wednesday',
          'Thursday', 'Friday']
```
## Trích dẫn trong Python
Python chấp nhận trích dẫn đơn ('), kép (") và trích dẫn tam (''' hoặc """) để biểu thị các hằng chuỗi, miễn là các trích dẫn này có cùng kiểu mở và đóng.
```python
word = 'word'
sentence = "This is a sentence."
paragraph = """This is a paragraph. It is
made up of multiple lines and sentences."""
```

## Comment trong Python
Python hỗ trợ hai kiểu comment đó là comment đơn dòng và đa dòng.

Trong Python, một dấu #, mà không ở bên trong một hằng chuỗi nào, bắt đầu một comment đơn dòng. Tất cả ký tự ở sau dấu # và kéo dài cho đến hết dòng đó thì được coi là một comment và được bỏ qua bởi trình thông dịch.
```python
# First comment
print "Hello, Python!" # second comment

name = "Madisetti" # This is again comment
```

Python cũng hỗ trợ kiểu comment thứ hai, đó là kiểu comment đa dòng được cho bên trong các trích dẫn tam
```python
#single line comment  
print "Hello Python"  
"""This is
multiline comment"""
```

## Các lệnh đa dòng trên một dòng đơn trong Python
Dấu chấm phảy (;) cho phép xuất hiện nhiều lệnh trên một dòng đơn.
```python
import sys; x = 'foo'; sys.stdout.write(x + '\n')
```

## Các nhóm lệnh đa dòng (còn được gọi là suite) trong Python
Một nhóm các lệnh đơn, mà tạo một khối code đơn, được gọi là suite trong Python. Các lệnh phức hợp như if, while, def, và class cần một dòng header và một suite.

Các dòng header bắt đầu lệnh (với từ khóa) và kết thúc với một dầu hai chấm (:) và được theo sau bởi một hoặc nhiều dòng để tạo nên một suite.

VD:
```python
if expression :
   suite
elif expression :
   suite
else :
   suite
```

## Nguồn
http://vietjack.com/python/cu_phap_python_co_ban.jsp
