# Thuật ngữ python

### hàm
#### khác nhau giữa tham biến và đối số:
Các tham số được xác định bởi các tên xuất hiện trong một định nghĩa hàm, trong khi các đối số là các giá trị thực sự được truyền cho một hàm khi gọi nó. Các tham số xác định loại đối số nào mà một hàm có thể chấp nhận. Ví dụ, với định nghĩa hàm:
``` python
def abc(a,b,c):
    pass

abc(10,20,30)
```
Khi đó a , b, c là tham số . 10 ,20 ,30 là đối số


Tham biến(tham số) có hai phương pháp:
-  đối số từ khóa : đối số đứng trước một số nhận dạng (ví dụ name=) trong một lệnh gọi hàm hoặc được chuyển dưới dạng giá trị trong từ điển đứng trước **.
``` python
complex(real=3, imag=5)
complex(**{'real': 3, 'imag': 5})
```
- đối số vị trí : đối số không phải là đối số từ khóa. Các đối số vị trí có thể xuất hiện ở đầu danh sách đối số và hoặc được chuyển dưới dạng các phần tử của một đối số có thể lặp lại trước *
``` python
complex(3, 5)
complex(*(3, 5))
```

### thuộc tính
Một giá trị được liên kết với một đối tượng được tham chiếu bằng tên bằng cách sử dụng các biểu thức dấu chấm. Ví dụ: nếu một đối tượng o có thuộc tính a thì nó sẽ được tham chiếu là o.a

### biến lớp

Một biến được định nghĩa trong một lớp và chỉ được sửa đổi ở cấp lớp (tức là không phải trong một thể hiện của lớp).

``` python
class test:
    def __init__(self):
        self.mang = []
        
``` 
Như vậy biến mang bây giờ chỉ đc sử dụng trong class test giống biến cục bộ



Làm lun bài hồi tối đi rồi làm bài này

# dictionary

Từ điển được sử dụng để lưu trữ các giá trị dữ liệu trong các cặp key: value.

## Cú pháp

Cú pháp: 
> Dictionary = {key: value}

 Truy cập :
 > Dictionary [key]
 
 Thêm items ( items là một combo key : valua )
> Dictionary [newkey] = value
Vd 
``` python
dictCar = {
    "brand": "Honda",
    "model": "Honda Civic",
    "year": 1972
}
dictCar["color"] = "yellow"
print(dictCar)
```
## VÍ DỤ

```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)

```
> {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
## dictionary items
Các mục từ điển được sắp xếp theo thứ tự, có thể thay đổi và không cho phép trùng lặp.

Các mục từ điển được trình bày theo cặp khóa: giá trị và có thể được tham chiếu bằng cách sử dụng tên khóa.
### ví dụ :
``` python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964,
  "year": 2020
}
print(thisdict)
```
> Year 2020 sẽ ghi đè lên year 1964

# các hàm sử lí từ điển
### đo độ dài

``` python
print(len(thisdict))

```
# các loại dữ liệu cho value từ điển
>. Các kiểu dữ liệu chuỗi, int, boolean và danh sách:

``` python
thisdict = {
  "brand": "Ford",
  "electric": False,
  "year": 1964,
  "colors": ["red", "white", "blue"]
}
```

# bài tập :

### bài cơ bản

Tạo một dictionary theo mẫu

> Tên_lớp = { số_ học_sinh : value,
Sốbannam: value,
Sốbannu : value
}

In ra màn hình số bạn nam
In ra số bạn nữ
Thêm items : số bạn cao trên 1m5 
### trung bình 
# viết 1 hàm 
yêu cầu hiện thực viết hàm search_profile_with_better_score với 2 tham số:

students: là mảng chứa các từ điển, mỗi từ điển lưu thông tin của một bạn thực tập sinh:
“name”: tên của thực tập sinh
“score”: điểm môn tin học
score: là điểm số môn Tin học dùng để so sánh
Hàm “search_profile_with_better_score” trả về một mảng chứa tên của tất cả các bạn thực tập sinh có điểm môn tin học cao hơn “score”

Gợi ý: Có thể dùng hàm append() để thêm một phần tử vào trong mảng 

Ví dụ: 

Danh sách thực tập sinh cùng với điểm
``` python
students =[

{'name': 'Hoa', 'score': 8}, 

{'name': 'Lan', 'score': 9},

{'name': 'Mai', 'score': 9}, 

{'name': 'Dao', 'score': 8}

]

print(search_profile_with_better_score(students, 8))
```
Kết quả là: 
> ['Lan', 'Mai']

Bài 3
yêu cầu hiện thực hàm sort_profile_high_to_low với 1 tham số:

students: là mảng chứa các từ điển, mỗi từ điển lưu thông tin của một bạn thực tập sinh:
“name”: tên của thực tập sinh
“score”: điểm môn tin học
Hàm sort_profile_high_to_low trả về một mảng chứa tên của các bạn thực tập sinh sắp xếp theo thứ tự điểm từ cao đến thấp 

Gợi ý:

Dùng một mảng tên “result” để lưu danh sách các bạn được sắp xếp điểm từ cao xuống thấp
Tìm bạn có điểm số cao nhất trong mảng students, thêm tên bạn vào danh sách “result” bằng hàm append()
Xoá bạn có điểm số cao nhất đó ra khỏi mảng “students” bằng lệnh “remove()”
Tiếp tục tìm bạn có điểm số cao nhất tiếp theo trong mảng “students"
Lặp lại cho đến khi mảng “students” không còn phần tử nào cả thì dừng lại (dùng câu lệnh ‘while’ để kiểm tra xem students có phải là mảng rỗng hay không)
Ví dụ:

Danh sách thực tập sinh cùng với điểm
``` python
students = [

{'name': 'Hoa', 'score': 6}, 

{'name': 'Lan', 'score': 10},

{'name': 'Mai', 'score': 9},

{'name': 'Hong', 'score': 11},

{'name': 'Dao', 'score': 8},

]

print(sort_profile_high_to_low(students))
```
Kết quả là: [‘Hong’, ‘Lan’, 'Mai', ‘Dao’, ‘Hoa’]
### k biết ib anh giải thích

## bản quyền
[MIT](https://choosealicense.com/licenses/mit/)

