# Responsive Grid - Refactor CSS sang SASS

Bài tập được tái cấu trúc từ mã nguồn mẫu `codegym-vn/responsive-grid`.

## Những phần đã refactor

- Tách toàn bộ CSS và inline style ra khỏi HTML.
- Dùng biến SASS cho màu sắc, chiều cao, độ rộng và opacity.
- Dùng mixin cho cột lưới và panel.
- Dùng nesting với modifier và component con.
- Chia SCSS thành các partial theo `abstracts`, `base`, `layout`.
- Giữ lại bố cục responsive 12 cột của bài mẫu.

## Cấu trúc

```text
responsive-grid-sass/
├── index.html
├── package.json
├── css/
│   └── main.css
└── scss/
    ├── main.scss
    ├── abstracts/
    │   ├── _variables.scss
    │   └── _mixins.scss
    ├── base/
    │   └── _reset.scss
    └── layout/
        └── _grid.scss
```

## Chạy bài

```bash
npm install
npm run build
```

Theo dõi thay đổi SCSS:

```bash
npm run watch
```

Mở `index.html` trên trình duyệt và thay đổi kích thước cửa sổ để kiểm tra grid responsive.
