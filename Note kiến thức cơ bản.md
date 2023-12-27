# Note các kiến thức cơ bản


# Các kiến thức về PACF,COV,....
- Cov(X,u) = 0 -> Không tương quan

# Heteroiskedasticity
- heteroskedasticity is when the variance of the underlying distribution used to construct our time series changes as a function of time.
- Common appearance: timeseries whose variance increase with time
- Biến đổi Box-Cox làm cho phân phối dữ liệu trở nên chuẩn hơn (che giấu Heteroiskedasticity)
- Phương sai của bước $X_t$ dựa vào phương sai của bước X_{t-1}
