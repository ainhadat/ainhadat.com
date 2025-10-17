# AI NHÀ ĐẤT - Demo (Next.js + Tailwind)

## Mục đích
Bản demo này là giao diện **AI NHÀ ĐẤT** (Tiếng Việt) — trang **danh sách nhà đất có bộ lọc**.
Dùng để deploy lên **Vercel** hoặc host trên bất kỳ nơi nào hỗ trợ Next.js.

## Hướng dẫn nhanh (trên máy của bạn)
1. Giải nén `ainhadat-web.zip`.
2. Mở terminal ở thư mục project.
3. Cài Node.js (>=18).  
4. Chạy:
   ```bash
   npm install
   npm run dev
   ```
   Mở http://localhost:3000 để xem.

## Đưa lên GitHub & Vercel (bước ngắn gọn)
1. Tạo repo GitHub (ví dụ: `ainhadat.com`) và upload toàn bộ file (kéo thả hoặc dùng git):
   ```bash
   git init
   git add .
   git commit -m "Initial commit - AI NHA DAT demo"
   git branch -M main
   git remote add origin https://github.com/yourname/yourrepo.git
   git push -u origin main
   ```
2. Vào https://vercel.com → New Project → Import từ GitHub → chọn repo vừa push → Deploy (mặc định Next.js).
3. Sau khi deploy, vào Project Settings → Domains → Add `ainhadat.com`. Vercel sẽ hiển thị 2 bản ghi DNS cần thêm cho domain.  
   - Thông thường bạn cần thêm:
     - A record: `@` → `76.76.21.21`
     - CNAME: `www` → `cname.vercel-dns.com`
   - Nhưng hãy **luôn dùng chính xác** giá trị Vercel hiển thị trong dashboard.
4. Vào trang quản lý domain (Mắt Bão) → DNS → Thêm 2 bản ghi trên.
5. Chờ vài phút → Vercel sẽ cấp SSL → site hoạt động trên `https://ainhadat.com`.

## Ghi chú
- Đây là demo front-end; tính năng AI/chatbot chưa được tích hợp backend. Để thêm chatbot, cần một server function hoặc service chạy LLM (OpenAI...) và endpoint.
- Bạn có thể chỉnh nội dung trong `pages/index.js` và thêm route chi tiết.

----
