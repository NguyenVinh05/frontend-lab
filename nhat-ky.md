# Nhật ký học Frontend

## Ngày 3a · 15/10/2026 · Tuần 1

**Đã học:**
- Selector: tên thẻ, `.class`, `#id`, `nav a` (phần tử bên trong), `a:hover`
- Specificity: `#id` > `.class` > tên thẻ, bằng điểm thì luật viết sau thắng
- Box model: `margin` ở ngoài viền, `padding` ở trong viền, `* { box-sizing: border-box; }`

**Đã làm:**
- Thêm ô số điện thoại `type="tel"` và 2 nút radio vào form (bài tập ngày 2)
- Tạo `style.css`, gắn vào trang bằng `<link rel="stylesheet">`
- Viết CSS khối 1–4: nền tối, căn giữa bằng `max-width` + `margin: 0 auto`, menu nằm ngang, kiểu thẻ `.card`

**Gặp lỗi gì, sửa thế nào:**
- Viết CSS cho `.card` nhưng các thẻ `<article>` chưa có `class="card"`, nên thẻ chưa có nền và viền. CSS chỉ áp dụng khi selector khớp với HTML
- Để `style.css` trong thư mục `ngay 2` thay vì tạo `ngay-03-css`

**Chưa hiểu rõ:**
- (ghi câu hỏi của bạn, nếu có)

**Ngày mai (3b):** thêm `class="card"`, CSS cho form, thí nghiệm specificity, soi box model bằng DevTools

## Ngày 2 · 13/10/2026 · Tuần 1

**Đã học:**
- HTML ngữ nghĩa: `header`, `nav`, `main`, `section`, `article`, `footer` thay cho `div`
- Mỗi trang chỉ một `h1`, các cấp tiêu đề đi theo thứ tự
- Form: `label` gắn với ô nhập qua `for` và `id`, `type="email"`, `required`
- Link nhảy trong trang: `href="#ky-nang"` khớp với `id="ky-nang"`

**Đã làm:**
- Trang hồ sơ cá nhân bằng HTML thuần (thư mục `ngay 2`)
- Thêm phần "Dự án" (bài tập 1)

**Gặp lỗi gì, sửa thế nào:**
- Commit nhật ký ngày 1 khi chưa lưu file, nên commit chỉ có file rỗng. Bài học: luôn `Ctrl + S` trước khi `git add`
- File nhật ký thiếu đuôi `.md`: đổi tên thành `nhat-ky.md` bằng `git mv`

**Chưa làm xong:**
- Bài tập 2: ô số điện thoại `type="tel"` và nút chọn radio
- Bài tập 3: kiểm tra code bằng W3C Validator
- Trả lời 4 câu tự kiểm tra

**Chưa hiểu rõ:**
- (ghi câu hỏi của bạn, nếu có)

**Ngày mai:** làm nốt bài tập ngày 2, rồi sang CSS cơ bản (selector, specificity, box model)

## Ngày 1 · 12/10/2026 · Tuần 1

**Đã học:**
- Cài VS Code, cấu hình Git, nối GitHub
- Vòng làm việc: `git add` → `git commit` → `git push`
- Tạo nhánh, gộp nhánh: `git switch -c`, `git merge`

**Gặp lỗi gì, sửa thế nào:**
- Gõ cả dấu `< >` trong địa chỉ repo → phải thay bằng tên thật, xóa luôn dấu ngoặc
- Có 2 tài khoản GitHub → repo cá nhân dùng NguyenVinh05, push qua HTTPS

**Chưa hiểu rõ:**
- (ghi câu hỏi của bạn, nếu có)

**Ngày mai:** HTML ngữ nghĩa và form
