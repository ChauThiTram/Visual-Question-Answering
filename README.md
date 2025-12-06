# Visual-Question-Answering

## Giới thiệu
Dự án xây dựng hệ thống VQA có khả năng trả lời câu hỏi tiếng Việt dựa trên nội dung hình ảnh đầu vào.
Ví dụ:
* **Input:** Ảnh quả táo + Câu hỏi "Đây là quả gì?"
* **Output:** "Quả táo"

## Kiến trúc Mô hình
Mô hình sử dụng kiến trúc **Encoder-Decoder**:
1.  **Image Encoder:** Sử dụng **CNN (ResNet18)** để trích xuất đặc trưng thị giác từ hình ảnh.
2.  **Question Encoder:** Sử dụng mạng **LSTM** để mã hóa câu hỏi và hiểu ngữ nghĩa.
3.  **Fusion & Classifier:** Kết hợp hai vector đặc trưng để dự đoán câu trả lời.

## Công nghệ
* **Framework:** PyTorch
* **NLP Tools:** Underthesea (Tokenization tiếng Việt)
* **Computer Vision:** Torchvision, Pillow
