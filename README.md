# 🏦 Bank Customer Churn Analysis & Prediction

## 📌 Tổng quan dự án
Dự án này phân tích hành vi rời bỏ dịch vụ (Churn) của khách hàng trong lĩnh vực ngân hàng. Dự án kết hợp sức mạnh của **Power BI** (để trực quan hóa dashboard) và **Google Colab/Python** (để xử lý dữ liệu chuyên sâu và xây dựng mô hình dự báo AI).

## 🛠 Công cụ sử dụng
- **Power BI:** Xây dựng Dashboard tương tác, đo lường các chỉ số DAX.
- **Python (Google Colab):** Xử lý dữ liệu (Data Cleaning), Feature Engineering và Machine Learning.
- **Thư viện:** Pandas, Matplotlib, Seaborn, Scikit-learn.

## 📊 Quy trình phân tích trên Notebook (Google Colab)
Trong file `Bank_Customer_Churn_Analysis.ipynb`, tôi đã thực hiện các bước:
1. **Làm sạch dữ liệu:** - Loại bỏ các bản ghi trùng lặp dựa trên `CustomerId`.
   - Xử lý các giá trị ngoại lai (Outliers) ở cột `Age` để đảm bảo dữ liệu mô hình chính xác.
2. **Feature Engineering:** - `Age Group`: Phân nhóm khách hàng (Young, Middle-aged, Senior).
   - `Balance Category`: Phân loại số dư tài khoản (Low, Medium, High).
3. **Xây dựng Model AI:**
   - Sử dụng thuật toán **Random Forest** để dự báo khả năng khách hàng rời bỏ.
   - Đánh giá model qua Accuracy, Precision và Recall.

## 📈 Trực quan hóa trên Power BI Dashboard
Dashboard cung cấp cái nhìn đa chiều thông qua:
- **Map Chart:** Tỷ lệ churn theo từng khu vực địa lý (Geography).
- **Scatter Plot:** Mối quan hệ giữa `CreditScore` và `Balance`, phân hóa theo độ tuổi.
- **Bar Chart:** Tỷ lệ churn dựa trên số lượng sản phẩm (`NumOfProducts`).
- **Slicers & Drill-down:** Cho phép lọc dữ liệu theo nhóm khách hàng và xem chi tiết cụ thể.
<img width="1305" height="785" alt="image" src="https://github.com/user-attachments/assets/37616a08-2ae3-46c9-addd-0b1534766d47" />
<img width="1306" height="788" alt="image" src="https://github.com/user-attachments/assets/04b9c4d0-59bc-491a-b9f6-e9fc5995ea3c" />

## 💡 Insights & Đề xuất
- **Phát hiện:** Nhóm khách hàng ở độ tuổi nhất định hoặc khu vực địa lý cụ thể có tỷ lệ rời bỏ cao đột biến.
- **Giải pháp:** - Đề xuất chương trình ưu đãi phí dịch vụ cho khách hàng có `Tenure` thấp.
  - Xây dựng chính sách chăm sóc riêng cho nhóm khách hàng có điểm tín dụng (`CreditScore`) thấp để giữ chân họ.

## 🚀 Cách chạy dự án
1. **Dành cho Power BI:** Mở file `.pbix` để xem dashboard tương tác.
2. **Dành cho Notebook:** Mở file `.ipynb` trên Google Colab để xem quy trình xử lý dữ liệu và huấn luyện model AI.

---
**Thực hiện bởi:** Võ Khánh Linh (LinhVK)
