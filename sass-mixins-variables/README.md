# SASS Variables & Mixins Practice

Cấu trúc bài thực hành:

```text
sass-mixins-variables/
├── abstracts/
│   ├── _variables.scss
│   └── _mixins.scss
├── base/
│   └── _typography.scss
├── components/
│   ├── _buttons.scss
│   └── _cards.scss
├── main.scss
└── main.css
```

## Biên dịch SCSS sang CSS

```bash
sass main.scss main.css
```

Hoặc theo dõi thay đổi tự động:

```bash
sass main.scss main.css --watch
```

Bài sử dụng biến để quản lý màu sắc, font-size, padding và box-shadow; đồng thời dùng mixin `button-style` và `box-style` để giảm lặp code.
