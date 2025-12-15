# B5 — Scanner, Parser và Symbol Table

Thư mục này chứa bài tập tuần 5: xây dựng các thành phần cơ bản của **một trình biên dịch nhỏ** gồm scanner, parser và symbol table.

## Nội dung chính

- `charcode.c`, `charcode.h` — hỗ trợ mã ký tự cho scanner
- `reader.c`, `reader.h` — đọc mã nguồn theo từng ký tự
- `scanner.c`, `scanner.h` — scanner (tách token)
- `token.c`, `token.h` — định nghĩa và xử lý token
- `parser.c`, `parser.h` — parser kiểm tra cú pháp
- `symtab.c`, `symtab.h` — bảng ký hiệu (biến, hàm, ...)
- `error.c`, `error.h` — xử lý lỗi
- `debug.c`, `debug.h` — hỗ trợ debug (nếu có)
- `main.c` — chương trình chính
- `Makefile` — biên dịch trên Unix / MinGW
- `tests/` — các file kiểm thử `.kpl`

## Mục tiêu

- Chuyển mã nguồn thành token bằng scanner
- Kiểm tra cú pháp và xây dựng cấu trúc trung gian bằng parser
- Lưu trữ thông tin định danh bằng symbol table

## Hướng dẫn nhanh (Windows PowerShell)

```powershell
cd .\B5
make         # hoặc dùng gcc trực tiếp nếu không có make
# Ví dụ: gcc *.c -o main.exe
.\main.exe tests\example1.kpl
```

## Kiểm thử & ghi chú

- Các file ví dụ nằm trong `tests/` (`example*.kpl`)
- Khi lỗi biên dịch, nên kiểm tra `charcode.c` và `reader.c` trước
- Trên Windows không có `make`, có thể dùng GCC (MinGW/MSYS2) hoặc Visual Studio Developer Command Prompt
- Thêm `README.md` này vào commit sau khi hoàn thành bài tập

