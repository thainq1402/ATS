# ATS
Chuỗi Thời Gian 

# Mô hình ARCH/GARCH

## 1.ARCH-AutoRegressive Conditional Heteroskedasticity
(Heteroskedasticity mang ý nghĩa các biến nhiễu (có điều kiện) có phân phối với phương sai không cố định)
- link :https://www.investopedia.com/terms/a/autoregressive-conditional-heteroskedasticity.asp

Tổng quan
- Mô hình thống kê sử dụng trong tài chính định lượng để nghiên cứu sự biến động (volatility) của lợi nhuận ( dispersion - dựa trên các lợi nhuận trong quá khứ)
    + link: https://www.investopedia.com/terms/v/volatility.asp
- Thường sử dụng để ước lượng các rủi ro 
- Mô hình có điều kiện do sử dụng  các giá trị từ quá khứ
- Work bezt for the high frequency data (hourly,daily,monthly...)
- So với các mô hình khác 
    + ARCH cho phép kết hợp độ biến động (volatility - nhiễn ?) thay đổi theo thời gian 

Giải thích:
- phenomenon of volatility clustering: 1 khoảng thời gian nào đó trong chuỗi thời gian, biên độ lợi nhuận giao động mạnh hơn so với các khoảng thời gian còn lại,
- Heteroskedasticity:Phần dư không có phương sai cố định

### Mô hình

