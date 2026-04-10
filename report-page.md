# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Mục tiêu của bài lab là làm quen với cách tính entropy và redundancy của chuỗi ký tự, đồng thời hiểu cách tìm nghịch đảo modulo bằng thuật toán Euclid mở rộng. Qua đó, em củng cố kiến thức về lý thuyết thông tin và số học ứng dụng trong mật mã.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy theo công thức log2(N) - H(X).
- Hoàn thiện hàm mod_inverse() bằng extended_euclid().
- Chạy thử trên nhiều test case để kiểm tra kết quả.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Chuỗi chỉ có 1 ký tự lặp lại nên entropy bằng 0, độ dư thừa rất cao |
| abcd | 2 | 6 | Các ký tự xuất hiện đều nhau nên entropy cao hơn |
| hello world | 2.8454 | 5.1546 | Phân bố ký tự không đều, entropy ở mức trung bình |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Qua bài lab, em hiểu rõ hơn cách tính entropy, redundancy và nghịch đảo modulo bằng thuật toán Euclid mở rộng. Khó khăn lớn nhất là ban đầu chưa quen với cách áp dụng công thức vào code, nhưng sau khi thử nhiều ví dụ em đã hiểu bài hơn.
