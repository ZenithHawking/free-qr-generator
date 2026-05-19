<div align="center">

<img src="icon.png" alt="Free QR Generator" width="96" height="96">

# Free QR Generator

**Web tạo mã QR mã nguồn mở — đẹp, miễn phí, chạy 100% trên trình duyệt.**

![License: MIT](https://img.shields.io/badge/License-MIT-d4a017.svg)
![Client-side](https://img.shields.io/badge/100%25-Client--side-success.svg)
![No backend](https://img.shields.io/badge/No-Backend-blue.svg)
![Single file](https://img.shields.io/badge/Single-File-orange.svg)

[**🌐 Live demo — qr.vansao.com**](https://qr.vansao.com)

</div>

---

## Giới thiệu

Một web app tạo mã QR **mã nguồn mở**, gói gọn trong **một file `index.html` duy nhất**. Không backend, không tracking, không lưu dữ liệu — mọi tác vụ chạy bằng JavaScript trên trình duyệt của bạn.

Bản demo chính thức đang chạy tại [qr.vansao.com](https://qr.vansao.com) (thương hiệu *Vạn Sao QR*). Bạn có thể **fork và self-host** bản của riêng mình chỉ với vài bước.

## Tính năng

- **6 loại mã QR**: URL · WiFi · vCard · Văn bản · Email · Số điện thoại
- **12 template thẩm mỹ**: Classic, Gold, Dark, Ocean, Royal, Rose, Forest, Sunset, Mint, Midnight, Cherry, Neon
- **Tùy chỉnh sâu**: màu sắc, gradient, kiểu dot, kiểu góc, mức sửa lỗi
- **Gắn logo** thương hiệu vào giữa mã QR
- **Khung viền & nhãn chữ** ("QUÉT MÃ", tùy chỉnh nội dung và màu)
- **6 mockup scene** để xem trước: Poster · Frame · Desk · Card · Menu · Phone
- **Lịch sử** lưu cục bộ trong trình duyệt (`localStorage`)
- **Xuất PNG / SVG** chất lượng cao
- **Dark mode** và giao diện responsive

## Triết lý

> *"Xử lý trên trình duyệt, không lưu trữ dữ liệu lên server."*

Mọi tác vụ — sinh mã, ghép logo, render mockup, xuất file — đều chạy bằng JavaScript phía client. Không có request nào gửi dữ liệu của bạn đi đâu cả.

## Công nghệ

- **HTML + CSS + Vanilla JS** — không build step, không framework
- [`qr-code-styling`](https://github.com/kozakdenys/qr-code-styling) — thư viện render QR
- **Bootstrap 5** + **Phosphor Icons** + **Google Fonts** (Playfair Display, DM Sans)
- Canvas API cho mockup và composite logo

## Sử dụng

Chỉ cần mở `index.html` bằng trình duyệt bất kỳ. Không cài đặt, không cấu hình, không cần internet (sau lần tải CDN đầu tiên).

## Self-host / Deploy

Đây là static site thuần — deploy được lên **bất kỳ** static host nào:

- **GitHub Pages** — bật Pages từ Settings, chọn nhánh `main`
- **Cloudflare Pages / Netlify / Vercel** — kết nối repo, build command để trống
- **Server tự host** — copy 4 file vào thư mục web root

```
index.html · icon.png · robots.txt · sitemap.xml
```

> 💡 Nhớ sửa `<link rel="canonical">`, các `og:url`, `og:image` và `sitemap.xml` để trỏ về domain của bạn.

## Cấu trúc

```
free-qr-generator/
├── index.html      # Toàn bộ ứng dụng (HTML + CSS + JS)
├── icon.png        # Favicon & Open Graph image
├── robots.txt
└── sitemap.xml
```

## Đóng góp

Pull request luôn được chào đón. Mọi đề xuất tính năng phải tôn trọng nguyên tắc cốt lõi: **không gửi dữ liệu người dùng ra server**.

## License

[MIT](LICENSE) — bạn có thể dùng, sửa, deploy thương mại tự do.

Live demo *Vạn Sao QR* © [Vạn Sao](https://vansao.com)
