
Hai hướng chính thử nghiệm:

1. Sử dụng dữ liệu lịch sử giao dịch từ Kaggle rồi gán nhãn “churn”

1.1 Dùng dữ liệu 2 tháng (tháng 10 và 11)

1.1.1 Gán nhãn churn và chia theo các tiêu chí:

1.1.1.1 Chia theo số lượng user:

Dùng các tập user gồm: 1 user xuất hiện nhiều nhất, top 5, 10, 20, 30, 2000 user.

1.1.1.2 Chia theo nhóm A, B, C, D dựa vào số lần xuất hiện:

A: >100 lần

B: >30 lần

C: >5 lần

D: còn lại

Mỗi nhóm được huấn luyện mô hình riêng.

1.1.1.3 Chia dữ liệu theo tuần:

Gán nhãn churn nếu user không xuất hiện trong 7 ngày tiếp theo của tháng 10.

1.1.1.4 Dùng toàn bộ dữ liệu 2 tháng với 4 thuật toán:

XGBoost, LSTM, TCN, N-BEATS

1.1.2 Dữ liệu 6 tháng (10/2019 – 3/2020)
Gán nhãn churn bằng cách xem user có xuất hiện ở tháng tiếp theo không (bỏ tháng 4/2020).

1.1.2.1 Thử với 3 thuật toán: XGBoost, LSTM, N-HITS

1.1.2.2 Hướng chính – Thử với: XGBoost, LSTM, TFT

2. Dùng dữ liệu đã có nhãn churn, tạo sinh thêm bằng GANs
Tạo dữ liệu tổng cộng 10GB bằng mô hình GANs để bổ sung dữ liệu huấn luyện.
