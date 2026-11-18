# Multi-Step Traffic Volume Forecasting and License Plate Recognition Using Deep Learning

## Giới thiệu

Project cuối kỳ Deep Learning của nhóm 3 gồm hai bài toán:

- **Task 2 — Dự báo lưu lượng xe:** dùng LSTM Encoder–Decoder với Attention để dự báo lưu lượng xe tại 5 mốc liên tiếp.
- **Task 3 — Nhận dạng biển số:** dùng CNN Encoder và LSTM Decoder để đọc chuỗi ký tự từ ảnh vùng biển số.

## Dữ liệu

- **Task 2:** [Metro Interstate Traffic Volume](https://archive.ics.uci.edu/dataset/492/metro+interstate+traffic+volume). Cột mục tiêu là `traffic_volume`. Đặt file CSV tại `data/raw/task2/Metro_Interstate_Traffic_Volume.csv`.
- **Task 3:** [Taiwan License Plate Recognition](https://huggingface.co/datasets/EZCon/taiwan-license-plate-recognition). Dùng `xywhr` để cắt vùng biển số và `license_number` làm nhãn. Đặt dữ liệu đã tải hoặc giải nén trong `data/raw/task3/`.

Dữ liệu gốc không được theo dõi trong Git.

## Cấu trúc repo

```text
.
├── data/raw/                       # Dữ liệu gốc cục bộ (không đưa lên Git)
├── report/                         # Báo cáo
├── task2_traffic_forecasting/      # Task 2
└── task3_plate_recognition/        # Task 3
```

- [Notebook khung Task 2](task2_traffic_forecasting/traffic_forecasting_outline.ipynb)
- [Notebook khung Task 3](task3_plate_recognition/license_plate_recognition_outline.ipynb)

## Cách chạy

Hiện repo mới có notebook khung, chưa có mã huấn luyện, file cấu hình môi trường hoặc framework được chốt. Mở notebook tương ứng bằng Jupyter hoặc VS Code để bổ sung phần triển khai; cài đặt môi trường và thư viện phù hợp sau khi nhóm thống nhất framework.
