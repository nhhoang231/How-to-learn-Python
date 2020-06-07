# Vòng lặp trong Python
---
## Các vòng lặp trong Python
`Vòng lặp while`: lặp đi lặp lại một lệnh hoặc một nhóm lệnh trong khi một điều kiện đã cho là TRUE. Nó kiểm tra điều kiện trước khi thực thi phần thân của vòng lặp.

`Vòng lặp for`: lặp qua các item của bất kỳ dãy nào như một list hoặc một string.

`Lồng vòng lặp`: có thể sử dụng một hoặc nhiều vòng lặp bên trong bất kỳ vòng lặp while, for hoặc do…while nào.

## Các lệnh điều khiển vòng lặp trong Python
`Lệnh break`: kết thúc lệnh vòng lặp và truyền trình thực thi tới lệnh ngay sau vòng lặp đó.

`Lệnh continue`: làm cho vòng lặp nhảy qua phần còn lại của thân vòng lặp và tự động kiểm tra lại điều kiện của nó trước khi lặp lại vòng mới.

`Lệnh pass`: được sử dụng khi một lệnh là cần thiết theo cú pháp, nhưng bạn lại không muốn bất cứ lệnh hoặc code nào được thực thi.

## WHILE LOOP
### Cú pháp
```python
while bieu_thuc:
   cac_lenh
```
VD:
```python
count = 0
while (count < 9):
   print 'So thu tu cua ban la:', count
   count = count + 1

print "Good bye!"
---
var = 1
while var == 1 :  # Lenh nay tao mot vong lap vo han
   num = raw_input("Hay nhap mot so  :")
   print "So da nhap la: ", num

print "Good bye!"
```
### WHILE ELSE
Python cho phép sử dụng lệnh else kết hợp với một vòng lặp. Khi else được sử dụng với một vòng lặp while, thì lệnh else được thực thi khi điều kiện là false.
VD:
```python
count = 0
while count < 5:
   print count, " la nho hon 5"
   count = count + 1
else:
   print count, " la khong nho hon 5"

KQ:
0 la nho hon 5
1 la nho hon 5
2 la nho hon 5
3 la nho hon 5
4 la nho hon 5
5 la khong nho hon 5
```

## FOR
### Cú pháp
```python
for bien_vong_lap in day_sequense:
   cac_lenh
```
Nếu một dãy `day_sequense` gồm một danh sách các biểu thức, nó được ước lượng đầu tiên. Sau đó, item đầu tiên trong dãy được gán cho biến vòng lặp bien_vong_lap. Tiếp theo, các khối lệnh cac_lenh được thực thi và khối lệnh này được thực thi tới khi dãy này đã được lặp xong.

VD:
```python
for letter in 'Python':     # Vi du dau tien
   print 'Chu cai hien tai :', letter

qua = ['chuoi', 'tao',  'xoai']
for qua in qua:        # Vi du thu hai
   print 'Ban co thich an :', qua

print "Good bye!"

KQ:
Chu cai hien tai : P
Chu cai hien tai : y
Chu cai hien tai : t
Chu cai hien tai : h
Chu cai hien tai : o
Chu cai hien tai : n
Ban co thich an : chuoi
Ban co thich an : tao
Ban co thich an : xoai
Good bye!
```
### Lặp qua index của dãy
VD:
```python
qua = ['chuoi', 'tao',  'xoai']
for index in range(len(qua)):
   print 'Ban co thich an :', qua[index]

print "Good bye!"
```

## LOOP IN LOOP
### Cú pháp
```python
# FOR
for bien_vong_lap in day_seq:
   for bien_vong_lap in day_seq:
      cac_lenh
   cac_lenh

# WHILE
while bieu_thuc:
   while bieu_thuc:
      cac_lenh
   cac_lenh
```

## Nguồn
http://vietjack.com/python/vong_lap_for_trong_python.jsp

