# 🩺 Hệ Thống Chẩn Đoán Y Khoa AI (Advanced Medical Diagnosis System)

<div align="center">
  <p><b>Dự án được nghiên cứu và phát triển bởi nhóm DaTai 🚀</b></p>
  
  [![Framework](https://img.shields.io/badge/Frontend-Vanilla_JS_|_HTML5_|_CSS3-blue.svg)](#)
  [![AI-Engine](https://img.shields.io/badge/AI_Core-TensorFlow.js_|_Gemini_2.0_Flash-orange.svg)](#)
  [![License](https://img.shields.io/badge/License-MIT-green.svg)](#)
</div>

---

## 📝 Giới Thiệu Chung

**Hệ Thống Chẩn Đoán Y Khoa AI** là một ứng dụng web y tế thông minh tích hợp Trí tuệ Nhân tạo hiện đại, hệ thống suy luận logic lâm sàng (Expert System) và giao diện Glassmorphism đỉnh cao. Hệ thống được thiết kế nhằm hỗ trợ bác sĩ và bệnh nhân trong việc thu thập sinh hiệu, khai báo triệu chứng, phân tích hình ảnh cận lâm sàng và đề xuất phác đồ điều trị an toàn, tối ưu.

📌 **Giao diện chính của hệ thống:**
![Giao diện chính](https://github.com/qkhanh6386/YKhoa/blob/main/README.md) *(Thay thế bằng link ảnh thực tế của bạn tại đây)*

---

## ✨ Các Tính Năng Nổi Bật

### 1. 🗂️ Quản Lý Hồ Sơ Bệnh Án Điện Tử (EMR)
*   **Định danh Y tế:** Khai báo thông tin bệnh nhân, phân loại độ tuổi tự động (Nhi khoa, Thành niên, Lão khoa), ghi nhận giới tính và tiền sử bệnh lý nền.
*   **Kiểm tra Tương tác Thuốc:** AI tự động phát hiện các tương tác thuốc nguy hiểm (Ví dụ: *Corticoid + NSAID*, *Paracetamol + Rượu*) và đưa ra cảnh báo dị ứng mạnh.
*   **Đồng bộ Smartwatch:** Lấy chỉ số sinh hiệu (Huyết áp, Nhịp tim, Đường huyết, SpO2) chỉ với **1-click** thông qua giả lập kết nối thiết bị đeo.
*   **Lịch sử Khám Bệnh:** Lưu trữ cục bộ an toàn (`localStorage`), hỗ trợ xóa hồ sơ và **Xuất Báo Cáo EMR ra file CSV** chuyên nghiệp.

### 2. 🔍 Khảo Sát Lâm Sàng & Động Cơ Suy Luận (Inference Engine)
*   **Phân nhóm Triệu chứng Sinh động:** Hơn 100+ triệu chứng được phân loại khoa học theo các nhóm chuyên khoa: Thần kinh, Tai Mũi Họng, Mắt, Hô hấp - Tim mạch, Tiêu hóa - Gan mật, Thận niệu, Cơ xương khớp & Da liễu.
*   **Động Cơ Suy Luận Kép (Hybrid Inference):**
    *   **Forward Chaining (Suy luận tiến):** Định lượng tổng trọng số của triệu chứng kết hợp tuổi tác, giới tính và bệnh nền để đưa ra chẩn đoán sơ bộ.
    *   **Backward Chaining (Suy luận lùi):** Tự động "hỏi vặn" và gợi ý các triệu chứng còn thiếu khi phát hiện nguy cơ cao của các bệnh lý nguy kịch, giúp loại trừ tối đa rủi ro bỏ sót bệnh.

### 3. 📸 Trung Tâm Cận Lâm Sàng & Phân Tích Hình Ảnh (Computer Vision)
*   **AI Phân Tích Hình Ảnh (TensorFlow.js + MobileNet):** Cho phép quét phim X-quang phổi, tổn thương da liễu hoặc siêu âm khối u bằng mạng nơ-ron tích chập (CNN) chạy **hoàn toàn ở Client-side** (offline, bảo mật dữ liệu).
*   **AI OCR & NLP Xét Nghiệm:** Đọc hiểu các chỉ số xét nghiệm từ file PDF hoặc ảnh chụp sinh hóa máu, tự động phân tích và đưa ra lời khuyên y khoa hữu ích.

### 4. 🤖 Trợ Lý Bác Sĩ AI & Chatbot Gemini
*   **Phân tích Bệnh sử tự động (Voice & Text NLP):** Bệnh nhân có thể mô tả triệu chứng bằng văn bản hoặc giọng nói (Web Speech API). AI tự động phân tích ngữ nghĩa và tự động tick chọn các triệu chứng y khoa tương ứng trên hệ thống.
*   **Tư vấn Hỏi đáp sau Chẩn đoán:** Chatbot AI tích hợp **Google Gemini API** (`gemini-2.0-flash`) sẵn sàng giải thích bệnh lý, trả lời câu hỏi và tư vấn chuyên sâu theo đúng ngữ cảnh của bệnh án hiện tại.

### 5. 📞 Tính Năng Hỗ Trợ Chăm Sóc Sức Khỏe
*   **Sơ đồ Suy luận AI (Decision Tree):** Hiển thị trực quan tiến trình và logic đưa ra kết luận của AI.
*   **Đặt lịch Theo dõi (Follow-up):** Đăng ký SMS nhắc nhở lịch uống thuốc tự động.
*   **Khám bệnh Từ xa (Telemedicine):** Giả lập cuộc gọi Video Call độ phân giải cao kết nối trực tiếp với Bác sĩ chuyên khoa.

---

## 🛠️ Công Nghệ Sử Dụng

Hệ thống được tối ưu hóa để vận hành mượt mà, nhẹ nhàng và không cần backend phức tạp:

| Thành phần | Công nghệ sử dụng |
| :--- | :--- |
| **Front-end UI/UX** | HTML5 Semantic, Vanilla CSS3 (Custom Properties, Flexbox, CSS Grid, Glassmorphism) |
| **Logic Core** | Modern JavaScript (ES6+, Async/Await, Web APIs) |
| **AI & Machine Learning** | TensorFlow.js & MobileNet (Phân tích hình ảnh ngoại tuyến) |
| **NLP & Chatbot** | Google Gemini API (`gemini-2.0-flash`) |
| **Hỗ trợ & Tiện ích** | Web Speech API (Nhận diện giọng nói), Google Translate API, Local Storage API, Window Print |

---

## 🚀 Hướng Dẫn Cài Đặt & Chạy Dự Án

Dự án được xây dựng thuần túy bằng HTML/CSS/JS, không phụ thuộc vào các bước build phức tạp của Node.js, giúp bạn triển khai cực kỳ dễ dàng theo 2 cách:

### Cách 1: Chạy nhanh (Không cần cài đặt)
1. Tải toàn bộ mã nguồn của kho lưu trữ này về máy tính.
2. Mở file `index.html` trực tiếp bằng trình duyệt (Double-click) hoặc sử dụng extension **Live Server** trong VS Code để khởi chạy.

### Cách 2: Cấu hình đầy đủ với Gemini API Key
Để kích hoạt toàn bộ sức mạnh của tính năng *Nhận diện giọng nói NLP* và *Trợ lý Bác sĩ AI*:
1. Đăng ký và lấy khóa API miễn phí từ [Google AI Studio](https://aistudio.google.com/).
2. Trên giao diện ứng dụng, bấm vào biểu tượng **⚙️ Cài đặt** ở góc trên menu trái.
3. Dán khóa API của bạn vào và bấm **Lưu**. Khóa sẽ được lưu trữ an toàn, bảo mật trong `localStorage` trên trình duyệt cá nhân của bạn.

---

## 📂 Cấu Trúc Thư Mục Dự Án

```markdown
├── index.html            # Giao diện chính của ứng dụng và các Modals UI
├── app.js                # Xử lý các sự kiện DOM, điều phối UI, tích hợp TensorFlow & APIs
├── style.css             # Hệ thống CSS variables, Glassmorphism, Dark mode & Responsive
├── inferenceEngine.js    # Động cơ suy luận lâm sàng (Forward & Backward Chaining)
├── knowledgeBase.js      # Cơ sở tri thức (Triệu chứng, Luật chẩn đoán, Phác đồ & Modifier)
└── README.md             # Tài liệu hướng dẫn dự án
🔒 Tuyên Bố Miễn Trừ Trách Nhiệm (Disclaimer)
⚠️ QUAN TRỌNG: Hệ thống này được phát triển hoàn toàn cho mục đích giáo dục, nghiên cứu công nghệ và hỗ trợ định hướng sơ bộ. Mọi thông tin chẩn đoán, phác đồ điều trị và cảnh báo thuốc từ AI chỉ mang tính chất tham khảo và không thay thế cho ý kiến chuyên môn, chẩn đoán hay chỉ định y khoa từ bác sĩ hoặc chuyên gia y tế có chứng chỉ hành nghề.

<div align="center">
<i>Chúc bạn có những trải nghiệm tuyệt vời với ứng dụng! Nếu thấy dự án hữu ích, hãy tặng <b>1 ⭐ Star</b> để ủng hộ nhóm phát triển nhé! 💖</i>
</div>
