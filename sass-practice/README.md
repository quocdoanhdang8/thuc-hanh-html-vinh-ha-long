# Thực hành cài đặt SASS bằng npm & SASS CLI

## 1. Kiểm tra Node.js và npm

```bash
node -v
npm -v
```

Nếu chưa có Node.js, cài từ trang chính thức của Node.js rồi mở lại Terminal/PowerShell.

## 2. Cài SASS

Cài toàn cục:

```bash
npm install -g sass
sass -v
```

Hoặc cài theo dự án này:

```bash
npm install
npx sass --version
```

## 3. Biên dịch một file SCSS sang CSS

```bash
sass scss/styles.scss css/styles.css
```

Hoặc dùng npm script:

```bash
npm run build
```

## 4. Chế độ watch

```bash
sass scss/styles.scss css/styles.css --watch
```

Hoặc:

```bash
npm run watch
```

Khi chỉnh sửa `scss/styles.scss`, file `css/styles.css` sẽ được cập nhật tự động.

## 5. Biên dịch nhiều file SCSS cùng lúc

```bash
sass scss/:css/ --watch
```

Hoặc:

```bash
npm run watch:all
```

Biên dịch một lần toàn bộ thư mục:

```bash
npm run build:all
```

Trong bài có hai ví dụ:

- `scss/styles.scss` → `css/styles.css`
- `scss/components.scss` → `css/components.css`

## 6. Nếu PowerShell chặn script npm

Ưu tiên cách ít nới lỏng quyền hơn:

```powershell
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

Sau đó mở lại PowerShell và thử lại `npm` / `sass`.

## 7. Cấu trúc bài

```text
sass-practice/
├── package.json
├── README.md
├── scss/
│   ├── styles.scss
│   └── components.scss
└── css/
    ├── styles.css
    └── components.css
```

Bài thực hành thể hiện: biến SCSS, mixin, nesting, `&:hover`, biên dịch một file, chế độ `--watch`, và biên dịch theo thư mục.
