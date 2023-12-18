# ATS
Chuỗi Thời Gian 

# Mô hình ARCH/GARCH

## 1.ARCH-AutoRegressive Conditional Heteroskedasticity 
(Heteroskedasticity mang ý nghĩa các biến nhiễu (có điều kiện) có phân phối với phương sai không cố định)
Dịch thô : Lớp phương trình có phương sai thay đổi theo tự hồi quy
- link :https://www.investopedia.com/terms/a/autoregressive-conditional-heteroskedasticity.asp

### Tổng quan
- Mô hình thống kê sử dụng trong tài chính định lượng để nghiên cứu sự biến động (volatility) của lợi nhuận ( dispersion - dựa trên các lợi nhuận trong quá khứ)
    + https://www.youtube.com/watch?v=Li95a2biFCU&t=47s
    + link: https://www.investopedia.com/terms/v/volatility.asp
- Thường sử dụng để ước lượng các rủi ro 
- Mô hình có điều kiện do sử dụng  các giá trị từ quá khứ
- Work bezt for the high frequency data (hourly,daily,monthly...)
- So với các mô hình khác 
    + ARCH cho phép kết hợp độ biến động (volatility - nhiễn ?) thay đổi theo thời gian 
    + Thực hiện được trên cả chuỗi dừng và không dừng 
### Giải thích:
- phenomenon of volatility clustering: 1 khoảng thời gian nào đó trong chuỗi thời gian, biên độ lợi nhuận giao động mạnh hơn so với các khoảng thời gian còn lại,
- Heteroskedasticity:Phần dư không có phương sai cố định

### Sử dụng 
- Sử dụng cho các chuỗi có khoảng thời gian có phương sai tăng hoặc giảm 
- Sử dụng sau khi đã fit được mô hình ARMA 

### Mô hình
- Bao gồm 2 phương trình:
    + Phương trình trung bình Y_t = /Muy_t +u_t
    + Phương trình phương sai 

### Các đặc tính của mô hình
    - Tính ổn định của mô hình 
    - Chuỗi chuẩn hoá (- trung bình)/ độ lệch chuẩn 
    - Ước lượng với giả định với phân phối nào thì phần dư cũng phải tuân theo pp đó 
    - 

### Demo 
    + Link: https://www.youtube.com/@ritvikmath


## 2.GARCH 
Mô hình chỉnh sửa bổ sung các yếu tố liên quan tới HÀM TRUNG BÌNH (Bổ sung thêm thành phần rủi ro và phương sai vào ptrinh trung bình)

### Mô hình

### Các đặc tính của mô hình

## 3.Cách chọn bậc của mô hình PACF

## 4.Ước lượng mô hình

### 4.1
    - 

### 4.2

### 4.3


## 5. Kiểm định mô hình như thế nào 

## 6.Cách deploy mô hình 

## 7.So sánh 2 mô hình 
