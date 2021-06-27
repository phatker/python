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
### k biết ib anh giải thích

## bản quyền
[MIT](https://choosealicense.com/licenses/mit/)

