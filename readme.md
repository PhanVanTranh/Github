## **✨ Phần 01 Git config**

Set config
```bash
git config --global user.name  "Name"
git config --global user.email "Email"
```

Get config

```bash
git config --global user.name
git config --global user.email
```
## **✨ Phần 02 Creating/Clone repo**

Tạo git trên máy tính cục bộ (Client)

```bash
git init
```

Liên kết client với Repo github

```bash
git remote add origin git_url
git remote -v
```
Clone repo về máy tính
```bash
git clone git_url
```

Chỉ lấy các file mới trên repo về máy tính

```bash
git pull origin master
```

Đẩy các file từ máy tính lên Repo github

```bash
git push origin master
```

## **✨ Phần 03 Staging**

Check status

```bash
git status
```

Thêm file vào Repi github

```json
"git add FILE_NAME" # chỉ add các file cần
```
```bash
git add .         # add tất cả các file"
```

Xóa file

```json
"git rm --cached FILE_NAME"
```

## **✨ Phần 04 Committing**

Hiển thị tất cả các commits chi tiết

```bash
git log
```

Hiển thị tất cả các commits trong một dòng

```bash
git log --oneline
```
```bash
git log --oneline -n
```

Tạo commit

```bash
git commit -m "comment"
```

## **✨ Phần 05 Git stash**

* Đang code dở file main.cpp
* Cần chuyển sang nhánh khác để sửa bug gấp

Lưu vào stash

```bash
git stash save -m "comment"
```

Lấy ra toàn bộ stash

```bash
git stash list
```

Khôi phục stash gần nhất và xóa khỏi danh sách

```bash
git stash pop
```

Khôi phục stash gần nhất nhưng không xóa khỏi danh sách

```bash
git stash apply
```

Xóa một stash

```bash
git stash drop stash@{0} # Xóa stash cụ thể (thay số 0 bằng vị trí stash bạn muốn xóa)
```

Xóa mọi stash

```bash
git stash clear   # Xóa vĩnh viễn TOÀN BỘ các stash đang có
```

## **✨ Phần 06 Git ignore**

```text
Ex:
.env
/Floder
*.txt
```


