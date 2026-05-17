# Card Optimizer VN - Final Test Package

Gói này gồm 2 bản:

## 1) pwa/
Dùng để test nhanh trên iPhone như app.

Cách dùng nhanh:
1. Upload toàn bộ thư mục `pwa` lên Netlify, Vercel, GitHub Pages hoặc hosting bất kỳ.
2. Mở link bằng Safari trên iPhone.
3. Bấm Share → Add to Home Screen.
4. App sẽ nằm ngoài màn hình chính như app.

File chính: `pwa/index.html`

## 2) capacitor/
Dùng để bọc thành app iOS thật bằng Capacitor/Xcode.

Trên máy Mac:
```bash
cd capacitor
npm install
npx cap add ios
npx cap open ios
```

Sau đó trong Xcode:
1. Vào Signing & Capabilities.
2. Đăng nhập Apple ID.
3. Chọn iPhone thật.
4. Bấm Run để cài test trên máy.

Muốn đưa lên TestFlight:
1. Trong Xcode chọn Product → Archive.
2. Distribute App → App Store Connect.
3. Vào App Store Connect → TestFlight để thêm tester.

Lưu ý:
- Upload TestFlight cần Apple Developer Program.
- Dữ liệu app hiện lưu trong localStorage. Trước khi đổi máy/xóa cache nên dùng nút Backup JSON trong app.
- OCR dùng thư viện online nên lần đầu cần internet.
