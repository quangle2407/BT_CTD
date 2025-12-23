# B6 — Semantic Analysis

Bài tập tuần 6: **Phân tích ngữ nghĩa (Semantic Analysis)** cho ngôn ngữ **KPL**.

## Mục tiêu

Xây dựng module phân tích ngữ nghĩa để phát hiện các lỗi như:

* Khai báo biến trùng lặp
* Sử dụng biến chưa khai báo
* Kiểm tra kiểu dữ liệu
* Các quy tắc ngữ nghĩa khác

## Cấu trúc thư mục

* `semantics.c/h` — Phân tích ngữ nghĩa
* `symtab.c/h` — Bảng ký hiệu
* `parser.c/h` — Phân tích cú pháp
* `scanner.c/h` — Quét từ vựng
* `token.c/h` — Token
* `charcode.c/h` — Xử lý ký tự
* `error.c/h` — Xử lý lỗi
* `debug.c/h` — Debug
* `main.c` — Chương trình chính
* `Makefile` — Build
* `run_tests.ps1` — Chạy test
* `tests/` — File `.kpl` và kết quả mong đợi

## Cách chạy

### Biên dịch

```bash
make
```

### Chạy test

```powershell
.\run_tests.ps1
```

### Chạy với file cụ thể

```bash
./main <file.kpl>
```

## Tests

Thư mục `tests/` gồm:

* `example1.kpl` → `example6.kpl`: Chương trình mẫu
* `result*.txt`: Kết quả mong đợi
* `my_output*.txt`: Kết quả thực tế

## Lưu ý

* Cần cài **GCC / MinGW** để biên dịch
* Dùng **PowerShell** khi chạy script test trên Windows
