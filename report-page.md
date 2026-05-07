# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Tìm hiểu và cài đặt các khái niệm cơ bản trong lý thuyết thông tin và mật mã học: tính giá trị Entropy (độ bất định), độ dư thừa thông tin (Redundancy) của một chuỗi và thuật toán Euclid mở rộng để tìm nghịch đảo modulo.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Chỉ có 1 ký tự lặp lại nên độ bất định bằng 0, độ dư thừa tối đa. |
| abcd | 2 | 6 | Các ký tự xuất hiện với xác suất đều nhau (1/4), entropy bằng log2(4) = 2. |
| hello world | 2.845 | 5.155 | Chuỗi có độ phân bố ký tự đa dạng hơn nên entropy tăng lên |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Qua bài lab này, em đã hiểu rõ hơn về mối quan hệ tỷ lệ nghịch giữa Entropy và Redundancy
