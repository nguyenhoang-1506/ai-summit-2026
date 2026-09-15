# Base CRM 2.0 — Prospector Pitch (AI Summit 2026)

Slide deck Keynote 1 · phân hệ **Prospector**, dựng theo Base AI Summit 2026 Keynote System.

## Chạy local

```bash
python3 -m http.server 8080
# mở http://localhost:8080
```

## Cấu trúc

| Đường dẫn | Nội dung |
|---|---|
| `index.html` | Toàn bộ deck |
| `support.js` | Điều hướng slide, build steps |
| `_ds/` | Design system: tokens, stage, bundle |
| `assets/` | Logo Base, icon các app |
| `shots/` | Ảnh chụp màn hình sản phẩm |

## Video demo

Video demo (`shots/demo.mp4`) **chưa** nằm trong repo — copy file vào `shots/` trước khi trình chiếu, hoặc đổi tweak `videoSrc` trong deck sang đường dẫn khác.

## Deploy

Repo này là static site — bật GitHub Pages ở nhánh `main`, thư mục root.

## Deploy lên Vercel

1. [vercel.com/new](https://vercel.com/new) → Import repo `ai-summit-2026`
2. Framework Preset: **Other** · Build Command: để trống · Output Directory: để trống (root)
3. Deploy

Site là static thuần, không cần build step. Mỗi lần push lên `main`, Vercel tự deploy lại.
