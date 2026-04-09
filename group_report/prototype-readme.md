### **Mô tả prototype**
 Nột trợ lý ảo AI (AI Agent) hỗ trợ người dùng tư vấn và tự động đặt lịch khám bệnh tại hệ thống bệnh viện Vinmec. Trợ lý này tương tác với người dùng qua giao diện dòng lệnh (CLI), có khả năng thu thập triệu chứng, tìm chi nhánh bệnh viện gần nhất, tra cứu lịch trống của bác sĩ theo chuyên khoa và tiến hành đặt lịch hẹn một cách hoàn toàn tự động.

### **Level**
- **Working** (Prototype có thể hoạt động thực tế với logic đặt lịch đẩy đủ thông qua Terminal/CLI và UI Streamlit).

### **Link prototype**
- **GitHub repo:** `https://github.com/MDuckkk/Z1-C401-Day06.git`

### **Tools và API đã dùng**
- **LLM & API:** OpenAI API (Sử dụng model `gpt-4o-mini` để suy luận và hiểu ngôn ngữ tự nhiên).
- **AI Framework:** LangChain và LangGraph (dùng StateGraph để quản lý luồng hội thoại và gọi công cụ).
- **External API:** OpenStreetMap (Nominatim API) dùng để chuyển đổi địa chỉ thành tọa độ (Geocoding) nhằm hỗ trợ việc tính toán khoảng cách.
- **Database:** SQLite (lưu trữ và tra cứu thông tin bác sĩ, chuyên khoa, lịch làm việc, và các chi nhánh dựa trên file `vinmec.sqlite`).
- **Custom Tools đã xây dựng:** Lấy vị trí người dùng (`get_nearest_branch`), tra cứu chuyên khoa (`get_all_specialties`), tư vấn bác sĩ phù hợp theo ca/ngày (`get_suitable_availibility_doctor`), và đặt lịch hẹn khép kín (`book_appointment`).

### **Phân công: AI làm gì**
Bảo: Spec, Slides, Gather data từ VinMec demo cho các team khác 
Tuấn Anh: Skeleton cho project và custom tools, demo cho các team khác
Nguyên: custom tools, review các team khác 
Đức: custom tools, database, demo cho các team khác
Huân: custom tools, database, review các team khác
Thắng: custom tools, review các team khác
