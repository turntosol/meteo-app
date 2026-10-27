# Weather App - Hệ thống WebGIS Dự báo Thời tiết

**Weather App** là một ứng dụng WebGIS hiện đại được xây dựng để cung cấp dữ liệu khí tượng trực quan và dự báo thời tiết chính xác. Dự án tận dụng sức mạnh của **Django REST Framework** ở phía backend và **Next.js** ở frontend để mang lại trải nghiệm người dùng nhanh chóng và mượt mà.

## Key Features
* **Bản đồ thời tiết:** Hiển thị vị trí và dữ liệu từ các trạm khí tượng (theo tỉnh thành) trên nền bản đồ tương tác.
* **Dự báo chi tiết:** Xem dự báo thời tiết theo giờ, theo ngày (7 ngày và 16 ngày).
* **Quản trị hệ thống:** Giao diện Admin cho phép quản lý tài khoản người dùng, cấu hình các lớp dữ liệu.  
* **Tối ưu hóa dữ liệu:** Sử dụng Supabase để lưu trữ và truy vấn dữ liệu nhanh chóng.

## Tech Stack
* **Frontend:** Next.js, Tailwind CSS, Leaflet.
* **Backend:** Django, Django REST Framework.
* **Database:** PostgreSQL.
* **Deployment:** Vercel, Railway.app.

## Local Development

### 1. Cấu hình Backend (Django)

#### Truy cập thư mục backend
```bash
cd backend
```

#### Khởi tạo và kích hoạt môi trường ảo
```bash
python -m venv venv
venv\Scripts\activate
```

#### Cài đặt các thư viện cần thiết
```bash
pip install -r requirements.txt
```

#### Cấu hình biến môi trường trong file .env

#### Chạy migration để đồng bộ database
```bash
python manage.py migrate
```

#### Khởi chạy server
```bash
python manage.py runserver
```

### 2. Cấu hình Frontend (Next.js)

#### Truy cập thư mục frontend

#### Cài đặt dependencies
```bash
npm install
```

#### Chạy ứng dụng ở chế độ phát triển
```bash
npm run dev
```
