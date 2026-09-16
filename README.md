\# BÀI THỰC HÀNH GIT



\## Bài 1: Khởi tạo Repository và commit đầu tiên



Đã thực hiện:

\- Khởi tạo Git repository.

\- Tạo index.html, style.css và notes.txt.

\- Đưa index.html và style.css vào Staging Area.

\- Giữ notes.txt ở trạng thái untracked.

\- Thực hiện commit: "Initial commit: add html and css".



\### Câu hỏi tư duy

Staging Area là vùng trung gian giúp lựa chọn chính xác những thay đổi sẽ được đưa vào commit. Nếu không có Staging Area thì việc commit sẽ khó kiểm soát hơn và dễ đưa nhầm các thay đổi chưa hoàn thiện vào lịch sử Git.



Minh chứng được lưu trong thư mục: `evidence/bai-1`.



\---



\## Bài 2: Commit nhiều lần và xem lịch sử



Các commit đã thực hiện:

\- Initial commit: add html and css

\- Update html content

\- Add javascript file

\- Update style and notes



Đã sử dụng `git log --oneline` và `git show` để kiểm tra lịch sử và nội dung commit.



Minh chứng được lưu trong thư mục: `evidence/bai-2`.



\---



\## Bài 3: Checkout và Reset



Đã thực hiện:

\- Checkout về commit "Add javascript file".

\- Quan sát trạng thái detached HEAD.

\- Quay trở lại nhánh chính.

\- Thử nghiệm reset soft, mixed và hard.



\### So sánh các loại reset



| Loại reset | Repository | Staging Area | Working Directory |

|---|---|---|---|

| --soft | Lùi commit | Giữ nguyên | Giữ nguyên |

| --mixed | Lùi commit | Bỏ staging | Giữ nguyên |

| --hard | Lùi commit | Xóa thay đổi staging | Xóa thay đổi trong Working Directory |



\### Câu hỏi tư duy

Nếu code đã được push lên GitHub và nhiều người đang cùng làm việc thì không nên tùy tiện dùng `git reset --hard` kết hợp force-push vì có thể làm thay đổi lịch sử chung và ảnh hưởng công việc của thành viên khác. Trong trường hợp cần hoàn tác commit đã chia sẻ, có thể sử dụng `git revert` để tạo một commit mới đảo ngược thay đổi.



Minh chứng được lưu trong thư mục: `evidence/bai-3`.



\---



\## Bài 4: Kết nối Remote GitHub



Đã thực hiện:

\- Tạo repository `git-basic-practice` trên GitHub.

\- Kết nối repository local với remote `origin`.

\- Kiểm tra bằng `git remote -v`.

\- Push lịch sử commit lên GitHub.



Minh chứng được lưu trong thư mục: `evidence/bai-4`.



\---



\## Bài 5: Clone, Pull và Push



Đã thực hiện:

\- Clone repository về một thư mục riêng.

\- Kiểm tra remote mặc định và lịch sử commit.

\- Tạo file about.txt, commit và push lên GitHub.

\- Tạo thay đổi trực tiếp trên GitHub.

\- Pull thay đổi từ GitHub về local.

\- Kiểm tra commit mới bằng `git log --oneline`.



\### Câu hỏi

`git pull` thực chất là sự kết hợp của:



`git fetch` + `git merge`



Minh chứng được lưu trong thư mục: `evidence/bai-5`.

