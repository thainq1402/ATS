# Note các kiến thức cơ bản


# Các kiến thức về PACF,COV,....
- Cov(X,u) = 0 -> Không tương quan

# Heteroiskedasticity
- heteroskedasticity is when the variance of the underlying distribution used to construct our time series changes as a function of time.
- Common appearance: timeseries whose variance increase with time
- Biến đổi Box-Cox làm cho phân phối dữ liệu trở nên chuẩn hơn (che giấu Heteroiskedasticity)
- Phương sai của bước $X_t$ dựa vào phương sai của bước $X_{t-1}$

# Volatility Clustering
- 

# Mô hình ARCH/GARCH/ TARCH 
- Mô hình hoá những phương sai của những biến động đó - volatility
- Mô hình này không dự báo xấp xỉ các giá trị ước lượng.
- Lớp mô hình này sẽ  capture cái kì vọng ( phương sai ) của nhiễu từ mô hình khác.
- Để dự báo thị trường tài chính chúng ta sẽ sử dụng ARCH và GARCH sau khi đã áp dụng các mô hình khác như ARIMA.

# Giá trị kiểm định 
- Giá trị thống kê - $\chi^2$
# P-value
- là 1 số liệu thống kê được sử dụng trong các mô hình để đánh giá mức độ hỗn loạn của các giả thuyết không đúng và dữ liệu quan sát
- Trong kiểm định thống kê , $\textbf{P-Value}$ là xác suất quan sát được 1 giá trị thống kê (1 giả thuyết) 


# Các thông số của mô hình 
### Phần 1: Thông tin tổng hợp
- AIC, BIC, HQIC các chỉ số đo lường hiệu quả của mô hình. Thấp là chỉ số tốt
### Phần 2: Thông tin ước lượng
- ar.L1 ... ar.Ln: Các hệ số của thành phần phân phối hồi quy (AR) tương ứng các lag
- sigma2: Phương sai của thành phần ngẫu nhiên không dự đoán. ( Nhiễu )
### Phân 3: Kiểm định: Tương quan, Phương sai thay đổi, Kiểm địng về pp chuẩn
- Ljung-Box (L1) (Q):  Kết quả kiểm định cho phần dư, kiểm tra tính không tương quan cho phần dư. Ở đây không tương quan cho lag = 1
- Jarque-Bera (JB): Kiểm định phân phối cho phần dư (Kiểm định về phân phối chuẩn)

Trong mô hình ARIMA ước lượng hệ số của AR sẽ được tiến hành bằng phương pháp "Hợp lý cực đại (Maximum likelihood)". 
P >|z|: kiểm định giả thuyết bác bỏ giải thuyết H0 rằng trung bình hệ số = 0 ?
Các mô hình có P-value khá to -> Không ảnh hưởng đến biến phụ thuộc (vni['Price'])

# Chưa hiểu 
