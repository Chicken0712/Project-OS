Hướng Dẫn Chạy Chương Trình
Sử dụng: <tên_chương_trình> [TÙY CHỌN]

Tùy chọn:
  -h, --help                          Hiển thị hướng dẫn sử dụng
  -d, --drive <ổ đĩa>                 [BẮT BUỘC] Chỉ định ổ đĩa (ví dụ: F:)
  -r, --recover                       [TÙY CHỌN] Khôi phục tập tin đã xóa
  -a, --analyze                       [TÙY CHỌN] Phân tích tập tin bị lỗi hoặc hỏng (tốn thời gian)
  -l, --no-log                        [TÙY CHỌN] Tắt ghi nhật ký danh sách tập tin bị xóa
🔹 Cách hoạt động
Khi sử dụng --recover hoặc --analyze, nếu tìm thấy tập tin đã xóa, chương trình sẽ yêu cầu bạn chọn tập tin muốn khôi phục.

Nếu chỉ dùng --drive, chương trình chỉ tìm tập tin bị xóa mà không thực hiện khôi phục.

💡 Ví dụ sử dụng
🔹 Khôi phục tập tin:

Tool --drive F: --recover
➡ Chương trình sẽ hiển thị danh sách các tập tin đã xóa và yêu cầu bạn chọn tập tin để khôi phục.

🔹 Khôi phục và phân tích tập tin đã xóa:

Tool --drive F: --recover --analyze
➡ Chương trình sẽ kiểm tra tập tin bị lỗi trước khi khôi phục (chỉ hỗ trợ FAT32, chưa áp dụng cho NTFS).

🚀 Cách chạy chương trình
Cách 1: Sử dụng file thực thi có sẵn
Tải file .exe từ thư mục bin của repository.

Mở Command Prompt (CMD):

Nhấn Win + R, nhập cmd, rồi nhấn Enter.

Di chuyển đến thư mục chứa file .exe:

cd duong_dan_den_bin
(Thay duong_dan_den_bin bằng đường dẫn thật của thư mục chứa file thực thi).

Chạy chương trình với các tùy chọn phù hợp:

<ten_file_thuc_thi>.exe [TÙY CHỌN]
(Thay <ten_file_thuc_thi> bằng tên file .exe, ví dụ: Tool.exe hoặc Toolx86.exe).

Cách 2: Biên dịch chương trình từ mã nguồn
Tải mã nguồn từ GitHub:

git clone https://github.com/Chicken0712/Project-OS
cd KhoiLoveAlice
Mở dự án bằng Visual Studio:

Mở file .sln trong thư mục gốc của dự án.

Chỉnh cấu hình build:

Đặt chế độ Release để có hiệu suất tốt hơn.

Đặt chuẩn C++ thành C++20 hoặc mới hơn:

Nhấp chuột phải vào project > Chọn Properties

Trong Configuration Properties > General, đặt C++ Language Standard thành ISO C++20 Standard (/std:c++20).

Biên dịch chương trình:

Chọn Build > Build Solution từ menu của Visual Studio hoặc nhấn Ctrl + Shift + B để biên dịch.

Nếu biên dịch thành công, file thực thi sẽ nằm trong thư mục:

<Project_Directory>\x64\Release\Tool.exe
(hoặc x86\Release\Toolx86.exe nếu build ở chế độ x86).

Sau đó, mở Command Prompt (CMD) và chạy chương trình như hướng dẫn ở trên.
