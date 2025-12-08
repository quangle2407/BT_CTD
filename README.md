# BTL / Bài tập theo tuần

Mỗi thư mục `B1`, `B2`, ... tương ứng bài tập theo từng tuần.


## Ví dụ cấu trúc

```
B1/
    main.c
    dữ liệu đầu vào + đầu ra mẫu

B2/
    nhiều file .c .h
    Makefile
    test/
```

## Cách chạy

### B1

```powershell
gcc .\B1\main.c -o .\B1\main.exe
.\B1\main.exe
```

### B2

```powershell
cd .\B2
make
.\run_tests.ps1
.\scanner.exe
```

## Cách nộp bài

* Commit vào đúng thư mục tuần
* Ghi rõ nội dung cập nhật trong commit message

---

Để xem chi tiết bài tập → đọc README.md trong từng thư mục
