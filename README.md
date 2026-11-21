# StudyHub — Hệ thống Quản lý Học tập Nhóm Đại học

Ứng dụng hỗ trợ sinh viên đại học lập kế hoạch môn học, chia việc nhóm, theo dõi deadline và lưu trữ tài liệu học tập tập trung.

## Tính năng chính
- **Quản lý môn học & lịch trình:** Tạo môn học, theo dõi lịch học, lịch thi và nhắc nhở hạn nộp bài.
- **Làm việc nhóm:** Tạo nhóm theo môn, phân công nhiệm vụ (To-do, In Progress, Done) và theo dõi tiến độ từng thành viên.
- **Kho tài liệu chung:** Đính kèm link tài liệu, slide bài giảng, biên bản họp nhóm và ghi chú theo từng chủ đề.
- **Thông báo & nhắc việc:** Cảnh báo deadline sắp tới và cập nhật thay đổi công việc trong nhóm.

## Công nghệ sử dụng
- **Frontend:** React / Next.js / Tailwind CSS *(thay đổi theo thực tế)*
- **Backend:** Node.js / Express *(hoặc Spring Boot / FastAPI)*
- **Database:** PostgreSQL / MongoDB *(hoặc MySQL)*
- **Công cụ khác:** Git, GitHub Actions, Docker

## Cấu trúc thư mục
```text
studyhub/
├── client/          # Mã nguồn giao diện người dùng
├── server/          # Mã nguồn API và xử lý nghiệp vụ
├── docs/            # Tài liệu đặc tả, thiết kế CSDL, slide báo cáo
└── README.md
```

## Hướng dẫn cài đặt và chạy dự án

### 1. Yêu cầu môi trường
- Git
- Node.js `>= 18.x` *(hoặc ngôn ngữ/runtime tương ứng)*
- Cơ sở dữ liệu đã cài đặt hoặc chạy qua Docker

### 2. Clone repository
```bash
git clone https://github.com/<ten-to-chuc-hoac-username>/studyhub.git
cd studyhub
```

### 3. Cấu hình biến môi trường
Tạo file `.env` từ file mẫu (nếu có) và cập nhật thông tin kết nối:
```bash
cp server/.env.example server/.env
```
Các biến cần thiết:
- `PORT=5000`
- `DATABASE_URL=...`
- `JWT_SECRET=...`

### 4. Cài đặt phụ thuộc và khởi chạy
**Backend:**
```bash
cd server
npm install
npm run dev
```

**Frontend:**
```bash
cd client
npm install
npm run dev
```

## Thành viên nhóm

| Họ và tên | MSSV | Vai trò / Phụ trách | GitHub |
| :--- | :--- | :--- | :--- |
| Nguyễn Duy Tân | 2451160825 | Trưởng nhóm, Backend, CSDL | @tanne55 |
| Nguyễn Hữu Quyết | 2451160819 | Frontend, UI/UX | @huuquyetnguyen |
| Nguyễn Hữu Hồng Sơn | 2451160823 | Kiểm thử, Tài liệu | @Hson2509 |
| Cao Thanh Tùng | 2451160846 | Triển khai, Vận hành | @tung-debug |

## Đóng góp và quy ước làm việc
- Tạo branch mới từ `main` theo cú pháp: `feat/ten-tinh-nang` hoặc `fix/ten-loi`.
- Viết commit ngắn gọn, rõ nghĩa (ví dụ: `feat: thêm tính năng tạo task nhóm`).
- Tạo Pull Request và nhờ ít nhất 1 thành viên review trước khi merge.

## Giấy phép
Dự án phục vụ mục đích học tập và nghiên cứu môn học tại trường đại học.
