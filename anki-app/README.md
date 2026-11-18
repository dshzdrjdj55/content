# Nhớ Lâu – ứng dụng thẻ nhớ kiểu Anki

Mở `index.html` trong trình duyệt là dùng được (dữ liệu lưu trong trình duyệt; dùng menu → Xuất dữ liệu để sao lưu).
`app.html` là cùng nội dung, không có khung `<html>`, dùng để đăng lên Claude Artifact (dữ liệu đồng bộ theo tài khoản).

Lịch ôn theo thuật toán SM-2 của Anki: bước học 1m/10m, tốt nghiệp 1 ngày, Easy 4 ngày,
độ dễ ban đầu 250%, Again −20%, Hard ×1.2 (−15%), Easy ×1.3 (+15%), học lại 10m khi quên, ngày mới lúc 4h sáng.
Mọi thông số chỉnh được trong "Giới hạn" của từng bộ thẻ.

## Ảnh và âm thanh
- Thẻ dùng ký hiệu như Anki: `[img:…]` và `[sound:…]`. Nút "+ Ảnh" / "+ Âm thanh" dưới ô nhập, hoặc dán ảnh trực tiếp.
- Menu → "Nhập bộ thẻ Anki (.apkg)": đọc cả định dạng cũ (collection.anki2/anki21) và mới (anki21b, nén zstd), kèm media và (tuỳ chọn) tiến độ học.
- Trên Artifact: ảnh lưu vào kho file của artifact, âm thanh lưu trong cơ sở dữ liệu tài khoản (chia nhỏ). Bản `index.html` mở trực tiếp lưu media trong IndexedDB của trình duyệt.
