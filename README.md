# Weather-Forecast-Using-LSTM-BiLSTM-Model
Dự báo thời tiết sử dụng mô hình học máy LSTM, BiLSTM

## Tóm tắt
Dữ liệu thời tiết trong project được thu thập từ thành phố Hồ Chí Minh trong thời gian từ 1/1/2021 đến 31/5/2023, sau đó được phân tích và sử dụng hai mô hình học máy LSTM và BiLSTM, kết hợp với 3 độ đo MAE, MSE và R Squared để so sánh độ chính xác của mô hình. Kết quả thu được cho thấy mô hình LSTM cho kết quả dự đoán tốt hơn so với mô hình BiLSTM.

## Hướng dẫn sử dụng
- data:
    + data.csv: Dữ liệu thu thập thời tiết của thành phố Hồ Chí Minh.
    + data_pre.csv: Dữ liệu đã tiền xử lý từ data.csv.
    + DataNormal_Maxtemp.csv: Dữ liệu đã chuẩn hóa cho mô hình dự đoán nhiệt độ cao nhất.
    + DataNormal_Mintemp.csv: Dữ liệu đã chuẩn hóa cho mô hình dự đoán nhiệt độ thấp nhất.

- weatherforecast: Các file cần tải lên Google colab để có thể chạy được,
khi tải file xong chọn chức năng "thời gian chạy" -> "chạy tất cả" để chạy file
    + CrawlData.ipynb: File thu thập dữ liệu thời tiết từ 1/1/2021 -> 31/5/2023.
    + CrawlData_PredictFuture.ipynb: File thu thập dữ liệu thời tiết trong tháng 6/2023
    + DataPreprocessing: File tiền xử lý và chuẩn hóa dữ liệu.
    + Maxtemp_BiLSTM: File xây dựng mô hình BiLSTM cho nhiệt độ cao nhất.
    + Maxtemp_LSTM: File xây dựng mô hình LSTM cho nhiệt độ cao nhất.
    + Mintemp_BiLSTM: File xây dựng mô hình BiLSTM cho nhiệt độ thấp nhất.
    + Mintemp_LSTM: File xây dựng mô hình LSTM cho nhiệt độ thấp nhất.
    + Predict_Maxtemp: File dự đoán thời tiết tương lai cho nhiệt độ cao nhất.
    + Predict_Mintemp: File dự đoán thời tiết tương lai cho nhiệt độ thấp nhất.
   Với file Maxtemp_BiLSTM, Maxtemp_LSTM, Predict_Maxtemp cần đính kèm thêm 2 tệp data: data_pre.csv,
	DataNormal_Maxtemp.csv để chạy.
   Với file Mintemp_BiLSTM, Mintemp_LSTM, Predict_Mintemp cần đính kèm thêm 2 tệp data: data_pre.csv,
	DataNormal_Mintemp.csv để chạy.

## Lưu ý
Project mang tính chất học tập

