## Phân tích 4 path

### 1.AI đúng (Happy Path)

Tình huống: Nhờ AI ghi nhận đã chi tiêu trà sữa 78k.

Kết quả: AI tự phân loại vào mục "Ăn uống", ghi nhận chi tiêu.

Nhận xét: Happy path xử lý tốt nhất vì dữ liệu đầu vào sạch sẽ, rõ ràng, AI chỉ cần thực hiện việc mapping.

### 2.AI không chắc (Edge case)

Tình huống: Nhờ AI chuyển tiền giúp.

Kết quả: AI không chắc, từ chối hỗ trợ.

### 3.AI sai (Fail path)

Tình huống: Nhờ AI ghi nhận "1 lít" vào khoản tiết kiệm.

Kết quả: AI không nhận ra "1 lít" là bao nhiêu tiền, ghi nhận sai thành 1 triệu

Nhận xét: Việc nhận sai giá trị chứng minh đây là path yếu nhất

### 4.Hallucination path (Ảo giác)

Tình huống: Nhờ AI ghi nhận đóng 1 tỷ tiền điện tháng 14.

Kết quả: AI cảnh báo con số 1 tỷ là có vấn đề, yêu cầu người dùng kiểm tra lại.

Nhận xét: Đây có vẻ là path yếu, vì AI chỉ nhận thấy con số 1 tỷ là phi lý và chưa nhận ra "tháng 14" không tồn tại.

## Path yếu nhất: Path 3 + 4

Khi sai, AI ghi nhận sai giá trị, không có feedback cho User confirm

Chưa nhận thấy đủ các điểm bất thường 

## Gap giữa Marketing và thực tế

### Marketing

Tự động hóa toàn bộ tác vụ, người dùng rảnh tay.

### Thực tế

Người dùng vẫn phải kiểm tra và sửa lại khá nhiều, cảm giác chưa đủ thông minh để tư vấn tài chính

