# Ecom Mastery Academy — bản đã khoá

Sổ tay tiếng Việt của bốn khoá học, **đã mã hoá**. Repo này chỉ chứa bản mã,
không chứa nội dung dạng chữ thường.

Mở tại: **https://thekizzz.github.io/ecom-mastery-academy/**

Cần mật khẩu để mở. Không có mật khẩu thì mọi file ở đây chỉ là chuỗi base64
vô nghĩa.

## Trong này có gì

| Khoá | Module | Bài |
|---|---:|---:|
| Evolve | 53 | 393 |
| Zakaria ECOM Masterclass | 32 | 127 |
| E-com MRR Mastery | 26 | 101 |
| Agentic Vibe Working | 1 | 5 |

Nhập mật khẩu một lần là đi được cả bốn khoá — chúng dùng chung một khoá mở
trong phiên làm việc.

Mỗi khoá còn một repo riêng chạy song song, cho những đường link đã gửi đi
trước khi có trang tổng này.

## Cách khoá

- PBKDF2-SHA256, 600.000 vòng lặp, salt ngẫu nhiên riêng cho từng trang
- AES-256-GCM
- Giải mã ngay trên trình duyệt bằng Web Crypto — không tải thư viện ngoài,
  không gọi server
- Mật khẩu nhớ trong `sessionStorage`, đóng tab là mất, không ghi xuống đĩa

## Giới hạn — nói thẳng

- Ai có mật khẩu đều có thể chuyển cho người khác.
- Bản mã nằm công khai, nên về lý thuyết có thể thử mật khẩu offline không giới
  hạn. 600.000 vòng PBKDF2 làm việc đó rất chậm và tốn kém, nhưng không loại
  trừ được.
- Một mật khẩu mở cả bốn khoá, nên mật khẩu lộ là lộ cả bốn — đây là cái giá
  của việc chỉ phải nhập một lần.
- Muốn chặt hơn thì cần host kiểm tra danh tính phía server (Cloudflare Access
  có gói free tới 50 người), hoặc GitHub Pro để dùng Pages trên repo private.

Bản gốc dạng chữ thường không nằm ở đây và không bao giờ được commit vào đây.
