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
    + https://www.investopedia.com/terms/v/volatility.asp
    + https://machinelearningmastery.com/develop-arch-and-garch-models-for-time-series-forecasting-in-python/
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


### Các đặc tính của mô hình
- Tính ổn định của mô hình 
- Chuỗi chuẩn hoá (- trung bình)/ độ lệch chuẩn 
- Ước lượng với giả định với phân phối nào thì phần dư cũng phải tuân theo pp đó
### Demo 
+ Link: https://www.youtube.com/@ritvikmath
### Paper 
+ Link: https://sci-hub.se/10.1080/096031000416433

### Ưu điểm 
- so với các phương pháp khác ARCH hay GARCH tốt hơn do có thể dự báo với những chuỗi có phương sai thay đổi 
### Nhược điểm 
- Cần qua nhiều bước xử lý 
    + Cần 1 bước biến đổi nếu chuỗi không dừng 
    + Cần tiềm hiểu nhiều hơn so với những kiến thức đã học do đây là lớp mô hình làm việc với phương sai thay đổi 
- Cần phải áp dụng các mô hình ARMA,AR,MA trước đó



## 2.GARCH 
Mô hình chỉnh sửa bổ sung các yếu tố liên quan tới HÀM TRUNG BÌNH (Bổ sung thêm thành phần rủi ro và phương sai vào ptrinh trung bình)

### Mô hình

### Các đặc tính của mô hình

### Deploy mô hình
+ Link:https://www.kaggle.com/code/wangqiyuan/value-at-risk-estimation-using-garch-model


## 3.Cách chọn bậc của mô hình PACF

## 4.Ước lượng mô hình

### 4.1 Xác định mô hình fit best cho chuỗi thời gian (vd như ARMA,AR,MA)
- Vẽ ACF, PACF -> xác định bậc của AR và MA -> Kiểm định giả thuyết xem nó có ý nghĩa thống kế hay không
    + Keyword: P value, nghiệm nằm trong đường tròn đơn vị 
    + phân phối chuẩn -> Không
    + tính nghịch đảo và nhân quả 
- Phần dư
- kiểm tra phần dư  xem có tương quan không 
- Thống kê kiểm định của phương trình trung bình

    Bước 1: Xác định mô hình trung bình (xem có suất hiện AR MA hay không)
    Bước 2: Kiểm tra hiệu ứng ARCH 
    Bước 3: Kiểm định mô hình


### 4.2

### 4.3


## 5. Kiểm định mô hình như thế nào 

### Metric để đánh giá mô hình 
- RMSE


## 6.Cách deploy mô hình 

## 7.So sánh 2 mô hình 
