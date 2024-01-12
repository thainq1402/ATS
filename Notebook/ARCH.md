# Tìm hiểu về lớp mô hình ARCH/GARCH/TARCH

## ARCH 
- Tổng quan: phương sai dựa trên bình phương sai số (sai số dự báo)
- Nhắc lại kiến thức:
    + AR model: giá trị hiện tại sẽ phụ thuộc vào $p$ giá trị trước đó cái mà giá trị $p_h$ tương quan mạng với giá trị hiện tại
- Mô hình ARCH: giá trị phương sai hiện tại sẽ dựa vào $p_h$ giá trị sai số bình phương (SSE) với các hệ số  $\alpha$ ( sai số là khoảng cách giữa giá trị quan sát và giá trị dự báo của mô hình khác)

![Alt text](<Mô hình ARCH - Kaggle.png>)

- Nếu sự biến động volatility có xu hướng tạo thành thì những cái bình phương sai số này (large square errors) sẽ gây ra phương sai lớn (large variance)
- Sử dụng $\textbf{ACF và PACF}$ để chọn các tham số
- ARCH(1) giả sử chuỗi đã cho làm chuỗi dừng ngoại trừ sự thay đổi của $\textbf{phương sai}$
- Sử dụng kết hợp vs AR hoặc ARMA
- Input: 
    + các giá trị nhiễu bình phương từ AR, ARMA..
    + 1 hàm trung bình - VD giá trị thay đổi của giá đóng cửa - 1 chuỗi thờii gian có giá trị xung quoanh mức 0.
    
## GARCH 
- Mở rộng của ARCH với cho phép phương sai phụ thuộc vào $\textbf{các giá trị lag của nó}$ và  $\textbf{các giá trị lags của phương sai}$ 
![Alt text](<Mô hình GARCH - Kaggle.png>)
    + $q$: lags của phương sai 
    + $p$: Số lag của $\textbf{Sai số của nhiễu}$

## Ljung-Box Test
- Tổng quan:
    + Kiểm tra xem giá trị tại các khoảng lag của ACF nó có gtrị về mặt thống kê hay không -> kiểm tra tính dự báo của mô hình dựa trên series
    + Cụ thể để kiểm tra giả thuyết rẳng là : 
        + $H_0$: "Không có tương quan trong hàm tự tương quan"
        + $H_1$: Tồn tại ít nhất 1 lag có tự tương quan đáng kể
    + Chọn mức ý nghĩa : 0.05
    + Thực hiện kiểm định:
        + Thu được giá trị thống kê kiểm địng từ dữ liệu (VD: chi-square)
        +  so sánh giá trị thống kê với ngưỡng quyết định (critical) dựa trên mức ý nghĩa đã chọn
    + Đưa ra qđịnh
        + Nếu thống kê vượt quá mức quy định > bỏ $H_0$ 
        + Ngược lại
- Test cho ACF
- Xác định xem chuỗi đã cho có phải nhiễu trắng hay không
- Sử dụng Ljung-Box lên $\textbf{nhiễu}$ để tìm kiếm $\textbf{tự tương quan}$
    + $H_0$: dữ liệu là độc lập và không tương quan
    + $H_a$: tồn tại tương quan
    
