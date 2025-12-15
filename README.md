# 💡Sharing-How-To-Use-Git-GitHub

Xin chào mọi người đã đến với buổi sharing của chúng mình: **Gia Khánh** và **Lam Phương**. Trong buổi sharing này bọn mình sẽ hướng dẫn các bạn sử dụng một số chức năng chính **Git** và **GitHub**. Hy vọng các bạn sẽ đón nhận nhiệt tình và áp dụng kiến thức vào các dự án sau này!😄

## 📥Tải và cấu hình Git!

1. Truy cập https://git-scm.com/install/ và tải Git về
2. Kiểm tra cài đặt Git
```bash
git --version
```
3. Cấu hình tên và email cho lần đầu
```bash
# Cấu hình tên
git config --global user.name “[Tên của bạn]”

# Cấu hình email
git config --global user.email “[Email của bạn]”

# Kiểm tra cấu hình (Bấm q để out)
git config --list
```

## 📝Các lệnh trọng ngày hôm nay bọn mình sẽ để đây nhé!

### 🔨Git Core Workflow (Local):

```bash
# Khởi tạo một local repository mới.
git init

# Kiểm tra trạng thái làm việc.
git status

# Đưa một tệp vào Staging Area.
git add [file]

# Đưa TẤT CẢ các tệp vào Staging Area.
git add .

# Ghi lại các thay đổi đã ở Staging Area vào lịch sử local repo.
git commit -m "[message]"

# Hiển thị lịch sử commits chi tiết.
git log

# Xem sự khác biệt giữa các trạng thái.
git diff
```

### 🔗Branching & Merging:

```bash
# Liệt kê tất cả các branch (nhánh) hiện có.
git branch

# Tạo một branch mới.
git branch [name]

# Chuyển đổi sang một branch khác.
git checkout [name]
# HOẶC (cho các phiên bản Git mới hơn)
git switch [name]

# Tạo branch mới và chuyển đổi sang branch đó ngay lập tức.
git checkout -b [name] = git branch [name] + git checkout [name]

# Hợp nhất (merge) các thay đổi từ branch được chỉ định vào branch hiện tại.
git merge [name]
```

### 🌐Collaboration (Remote/GitHub):

```bash
# Sao chép (clone) toàn bộ remote repository về máy.
git clone [url]

# Liệt kê các tên remote (kèm theo URL đầy đủ của chúng).
git remote -v

# Đẩy các commit cục bộ lên remote repository.
git push

# Tải (fetch) các thay đổi từ remote về local repo (KHÔNG tự động merge).
git fetch [remote-name]

# Tải các thay đổi từ remote và tự động hợp nhất vào nhánh làm việc hiện tại.
git pull = git fetch + git merge
```

### ⚙️Các bước để kết nối local repo với remote repo (lần đầu): 

```bash
# Thêm Remote URL (thường đặt tên là 'origin').
git remote add origin [URL-GitHub-repo]

# Đổi tên nhánh làm việc cục bộ thành 'main'.
git branch -M main

# Đẩy code lên Remote và thiết lập theo dõi cho lần đẩy đầu tiên.
git push -u origin main
```

## 📚Áp dụng kiến thức: Winter_Playlist ❄️
### ➡️Hướng dẫn:

1. Clone repo này về máy: https://github.com/OcKhanhVN/Sharing-How-To-Use-Git-GitHub.git
2. Tạo và chuyển sang branch mới đặt tên của bạn
3. Mở file Winter_Playlist.txt
4. Viết tên ca khúc + ca sĩ + tên của bạn giống như ví dụ mẫu trong file (1 người khoảng 5 ca khúc)
5. Commit và push branch của bạn lên GitHub
6. Tạo Pull Requests yêu cầu gộp branch của mình vào branch main
7. Comment, check review trên Pull Requests
8. Nêu các bạn bị conflict (vì cùng bài hát) thì hãy thêm tên của mình vào bên cạnh
```bash
# Ví dụ:
Mistletoe - Justin Bieber - Gia Khánh, Lam Phương
```
9. Đợi được approve và merge

## 🌟Lời Kết Thúc

**Cảm ơn tất cả các bạn** đã dành thời gian quý báu để theo dõi đến cuối bài sharing của chúng mình! 🎉

Hy vọng những kiến thức về Git và GitHub này sẽ trở thành **công cụ đắc lực 🛠️** giúp các bạn quản lý code một cách chuyên nghiệp và hiệu quả hơn trong các dự án sắp tới. 🚀

Chúc các bạn thành công và tạo ra những sản phẩm chất lượng! 💪
---
