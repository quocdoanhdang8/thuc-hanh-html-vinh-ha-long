# Landing Page SASS Refactor

Bài tập tái cấu trúc CSS của Landing Page đã làm trước đó sang SASS.

## Cấu trúc

- `index.html`: giao diện Landing Page giữ nguyên nội dung MyBrand.
- `scss/abstracts/_variables.scss`: biến màu sắc, breakpoint, spacing, radius.
- `scss/abstracts/_mixins.scss`: mixin flex, section spacing, card, responsive.
- `scss/base/_base.scss`: reset và style nền tảng.
- `scss/layout/_header.scss`: header/navigation.
- `scss/layout/_content.scss`: hero, services, testimonials.
- `scss/layout/_footer.scss`: footer.
- `scss/main.scss`: file SASS tổng.
- `css/main.css`: CSS đã biên dịch.

## Các kiến thức SASS đã áp dụng

- Variables
- Nesting
- Mixins
- `@use`
- `@content` trong responsive mixin
- Tách partial theo module

## Chạy bài

```bash
npm install
npm run build
```

Watch mode:

```bash
npm run watch
```

Sau khi build, mở `index.html` trên trình duyệt để kiểm tra giao diện.
