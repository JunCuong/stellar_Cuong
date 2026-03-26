Tên Dự Án: Soroban Micro-Paywall
https://stellar.expert/explorer/testnet/tx/33b08c7677773ff95da2a7ee834d4825101b4de54c4581d4c54e0519f3419fc2
<img width="1385" height="182" alt="image" src="https://github.com/user-attachments/assets/b7adf2c5-d738-499b-8e28-d22328537021" />


Mô tả: Giải pháp thanh toán vi mô (micro-transaction) trên mạng lưới Stellar/Soroban dành cho nền kinh tế sáng tạo (Creator Economy), cho phép tác giả thu phí người dùng để mở khóa nội dung ẩn (bài viết, video).

🚀 Chức Năng Hiện Tại (MVP)
Dự án hiện tại là một Smart Contract cốt lõi tập trung vào một giao dịch on-chain duy nhất để xử lý thanh toán:

Cấu hình ban đầu (init): Thiết lập ví nhận tiền của tác giả, loại token chấp nhận (XLM/USDC) và mức giá cố định cho nội dung.

Mở khóa nội dung (unlock_article): Thực hiện giao dịch chuyển token trực tiếp từ người đọc sang tác giả. Trạng thái "đã mua" của người dùng đối với article_id cụ thể được lưu vĩnh viễn trên chuỗi (persistent storage).

Kiểm tra quyền (has_access): Hàm đọc dữ liệu (read-only) cho phép ứng dụng kiểm tra on-chain xem ví người dùng đã trả phí chưa, từ đó quyết định mở khóa hay tiếp tục che nội dung.

Triển khai Testnet: Contract đã được biên dịch và có thể tương tác đầy đủ thông qua Stellar CLI trên mạng Testnet.

🔮 Tương Lai Làm Gì
Xây dựng Frontend dApp: Phát triển giao diện web (React/Next.js) tích hợp ví Freighter/Albedo, biến các dòng lệnh CLI thành một nút bấm "Thanh toán" trực quan cho người dùng cuối.

Định giá động (Dynamic Pricing): Nâng cấp contract để tác giả có thể cài đặt mức giá khác nhau cho từng ID bài viết.

Mô hình Đăng ký (Subscription): Mở rộng tính năng để hỗ trợ thanh toán gia hạn theo tháng/năm thay vì chỉ mua đứt từng bài.

Triển khai Mainnet: Đưa hệ thống lên mạng chính thức và tích hợp các stablecoin (USDC) để giao dịch bằng giá trị thực.
