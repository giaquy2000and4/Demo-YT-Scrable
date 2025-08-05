
# YouTube Video Info Extractor

**YouTube Video Info Extractor** là một công cụ dòng lệnh được viết bằng Python giúp bạn trích xuất thông tin video và phụ đề tiếng Việt từ một hoặc nhiều liên kết YouTube.

---

##  Tính năng

- Trích xuất tiêu đề, ID, thời lượng và URL của video YouTube
- Tự động tải và làm sạch phụ đề tiếng Việt (cả tự tạo và thủ công)
- Lưu kết quả thành file `youtube_results.json`
- Xuất phụ đề và thông tin video vào thư mục `subtitles/`
- Tương tác qua menu giao diện dòng lệnh thân thiện
- Tự động kiểm tra và cài đặt `yt-dlp` nếu chưa có

---

##  Yêu cầu

- Python 3.6+
- Gói `yt-dlp`

> Lưu ý: Script sẽ tự động kiểm tra và cài đặt `yt-dlp` nếu cần.

---

##  Cách sử dụng

### 1. Chạy chương trình

```bash
python3 title_sub.py
````

### 2. Các tùy chọn trong menu

1. **Chọn file chứa danh sách URL**
   (Một file `.txt` với mỗi dòng là một liên kết YouTube)

2. **Nhập URL trực tiếp**

3. **Xem kết quả trước đó**
   (Đọc từ `youtube_results.json` nếu tồn tại)

4. **Xuất tất cả phụ đề thành file txt**
   (Xuất từ kết quả trước đó nếu có)

5. **Thoát chương trình**

---

##  Kết quả

* Tập tin JSON: `youtube_results.json`
* Thư mục: `subtitles/`

  * `sub.txt`: chứa phụ đề tiếng Việt đã làm sạch
  * `info.txt`: chứa thông tin video cơ bản

---

## 📄 Cấu trúc file input (ví dụ)

```txt
https://www.youtube.com/watch?v=dQw4w9WgXcQ
https://youtu.be/abcdEFGhijk
```

> Hỗ trợ cả định dạng `youtube.com`, `youtu.be`, `embed`, v.v.

---

##  Ghi chú

* Chương trình xử lý lỗi và URL không hợp lệ một cách thân thiện
* Phụ đề sẽ được lọc bỏ các timestamp, thẻ HTML và ký tự đặc biệt
* Đảm bảo máy tính có kết nối internet để tải phụ đề

---


