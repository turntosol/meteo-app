# Weather App - Hệ thống WebGIS Dự báo Thời tiết

**Weather App** là một ứng dụng WebGIS hiện đại được xây dựng để cung cấp dữ liệu khí tượng trực quan và dự báo thời tiết chính xác. Dự án tận dụng sức mạnh của **Django REST Framework** ở phía backend và **Next.js** ở frontend để mang lại trải nghiệm người dùng nhanh chóng và mượt mà.

## 🔗 Liên kết Dự án
* **Website (Production):** [https://meteo-app-coral.vercel.app/](https://meteo-app-coral.vercel.app/)

## 🚀 Tính năng chính
* **Bản đồ thời tiết:** Hiển thị vị trí và dữ liệu từ các trạm khí tượng (theo tỉnh thành) trên nền bản đồ tương tác.
* **Dự báo chi tiết:** Xem dự báo thời tiết theo giờ, theo ngày (7 ngày và 16 ngày).
* **Quản trị hệ thống:** Giao diện Admin cho phép quản lý tài khoản người dùng, cấu hình các lớp dữ liệu (layers), 
* **Tối ưu hóa dữ liệu:** Sử dụng Supabase để lưu trữ và truy vấn dữ liệu nhanh chóng.

## 🛠️ Công nghệ sử dụng
* **Frontend:** Next.js, Tailwind CSS, Leaflet (hiển thị bản đồ).
* **Backend:** Django, Django REST Framework.
* **Database:** PostgreSQL (Hosted on **Supabase**).
* **Deployment:** Vercel (Frontend), Railway.app (Backend).

## 💻 Hướng dẫn chạy dự án (Local Development)

### 1. Cấu hình Backend (Django)
Yêu cầu: Đã cài đặt Python 3.x.
```bash
# Truy cập thư mục backend
cd backend

# Khởi tạo và kích hoạt môi trường ảo
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Cài đặt các thư viện cần thiết
pip install -r requirements.txt

# Cấu hình biến môi trường trong file .env (Sử dụng Connection String từ Supabase)
# Chạy migration để đồng bộ database
python manage.py migrate

# Khởi chạy server
python manage.py runserver
```
### 2. Cấu hình Frontend (Next.js)
```bash
# Truy cập thư mục frontend

# Cài đặt dependencies
npm install

# Chạy ứng dụng ở chế độ phát triển
npm run dev
```
