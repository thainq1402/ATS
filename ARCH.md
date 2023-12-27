# Tìm hiểu về lớp mô hình ARCH/GARCH/TARCH

## ARCH 
- Nhắc lại kiến thức:
    + AR model: giá trị hiện tại sẽ phụ thuộc vào $p$ giá trị trước đó cái mà giá trị $p_h$ tương quan mạng với giá trị hiện tại
- Mô hình ARCH: giá trị phương sai hiện tại sẽ dựa vào %p_h% giá trị sai số bình phương (SSE) với các hệ số  $\alpha$ ( sai số là khoảng cách giữa giá trị quan sát và giá trị dự báo của mô hình khác)
![Alt text](<Mô hình ARCH - Kaggle.png>)
- Nếu sự biến động volatility có xu hướng tạo thành thì những cái bình phương sai số này (large square errors) sẽ gây ra phương sai lớn (large variance)
- Sử dụng $\textbf{ACF và PACF}$ để chọn các tham số
- ARCH(1) giả sử chuỗi đã cho làm chuỗi dừng ngoại trừ sự thay đổi của $\textbf{phương sai}$
