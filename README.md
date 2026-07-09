ĐỀ BÀI
Hệ thống Quản lý Lớp học Trực tuyến


[Bài tập] Hệ thống Quản lý Lớp học Trực tuyến

 

1. Mục tiêu
Thiết kế ERD cho hệ thống đa vai trò người dùng (User Role)
Phân tích quan hệ đa tầng (Users – Courses – Enrollment – Assessments)
Tư duy chuẩn hóa dữ liệu, tách bảng hợp lý cho hệ thống có quy mô lớn
 

2. Mô tả
Một nền tảng học trực tuyến (như Coursera hoặc Udemy) cần quản lý:

Người dùng (User): mã người dùng, họ tên, email, mật khẩu, vai trò (student/instructor/admin)
Khóa học (Course): mã khóa, tên, mô tả, cấp độ, giá, ngày phát hành
Danh mục khóa học (Category): mã danh mục, tên danh mục
Giảng viên (Instructor): là một loại User, có thêm thông tin học vị, chuyên môn
Đăng ký học (Enrollment): lưu việc học viên tham gia khóa học nào, ngày đăng ký, trạng thái (đang học, hoàn thành, hủy)
Bài học (Lesson): mã bài học, tiêu đề, nội dung, thời lượng, thuộc khóa học
Bài kiểm tra (Quiz): mã quiz, tiêu đề, số câu hỏi, thuộc bài học nào
Kết quả (Result): mã kết quả, điểm, ngày làm, thuộc về học viên nào và quiz nào
 

Yêu cầu:

Xác định tất cả thực thể, thuộc tính, khóa chính, khóa ngoại
Thể hiện các mối quan hệ chính:
Một giảng viên có thể dạy nhiều khóa học
Một khóa học thuộc về một danh mục
Một khóa học có nhiều bài học, mỗi bài học có thể có quiz
Một học viên có thể học nhiều khóa học → mối quan hệ n–n (Enrollment)
Một học viên có thể làm nhiều quiz, mỗi lần làm có một Result riêng
Vẽ sơ đồ ERD đầy đủ với các ký hiệu:
(1–n), (n–n)
Khóa chính (PK), khóa ngoại (FK)
Ghi chú vai trò (Student, Instructor nếu chung bảng User)
(Optional): Đề xuất thêm bảng Payment hoặc Certificate để mở rộng hệ thống
