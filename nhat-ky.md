# Nhật ký học Frontend

## Ngày 7 · 20/10/2026 · Tuần 2

**Đã học:**
- Flexbox: `display: flex` đặt ở phần tử **cha**, các con tự xếp hàng
- Trục chính dùng `justify-content`, trục phụ dùng `align-items`, khoảng cách giữa các con dùng `gap`
- `flex: 1` cho các con chia đều bề ngang

**Đã làm (thư mục `ngay-07-flex`):**
- Bọc tên và dòng giới thiệu vào `div class="ten"`
- Menu `nav ul` chuyển sang `display: flex`
- Viết CSS cho `.hang-the` và `.hang-the .card`

**Gặp lỗi gì, sửa thế nào:**
- Header chưa có `display: flex; justify-content: space-between; align-items: center;` nên tên và menu chưa nằm hai bên
- Thẻ `div` bọc các card kỹ năng chưa có `class="hang-the"`, nên CSS `.hang-the` không áp dụng, card chưa nằm ngang. Lại là lỗi "CSS có nhưng HTML không khớp" giống ngày 3
- Khối cũ `nav li { display: inline-block; }` chưa xóa

**Ngày mai:** sửa 3 lỗi trên, học `flex-wrap`, Flexbox Froggy màn 13–24, dựng thành phần header có menu

## Ngày 6 · 19/10/2026 · Tuần 2

**Đã học:**
- Đơn vị: `px` cố định, `rem` theo cỡ chữ gốc (1rem = 16px), `%` theo phần tử cha
- Cỡ chữ nên dùng `rem` để người dùng phóng to được
- Biến CSS: khai báo trong `:root { --ten: giá-trị; }`, dùng bằng `var(--ten)`

**Đã làm (thư mục `ngay-06-bien-css`):**
- Gom 7 màu vào biến (`--mau-nen`, `--mau-the`, `--mau-chu`, `--mau-chinh`...), thay 13 chỗ mã màu bằng `var()`
- Đặt khối `:root` ở đầu file

**Gặp lỗi gì, sửa thế nào:**
- Màu giống nhau nhưng khác ý nghĩa thì không dùng chung biến: `#111` vừa là nền trang vừa là chữ trên nút, chỉ thay chỗ nền trang
- VS Code không cho lưu vì file trên ổ đĩa đã bị sửa từ bên ngoài. Cách xử lý: `Ctrl + Shift + P` → **Revert File** để tải lại bản mới
- Chưa làm: đổi `margin-bottom` và `border-radius` của card sang `var(--khoang-cach)`, `var(--bo-goc)`; thử đổi `--mau-chinh` sang màu khác

## Ngày 5 · 17/10 → 19/10/2026 · Tuần 1

**Đã làm:** sửa lỗi trong `ngay-04-form`, tạo thư mục `ngay-05-bai-tap`

**Gặp lỗi gì, sửa thế nào:**
- `class="card>` thiếu dấu nháy đóng ở 3 thẻ, nên class không được nhận. Dấu hiệu: code phía sau đổi màu bất thường trong VS Code
- Một thẻ `<article >` chưa có class
- Khối `.btn:hover` bị trộn nội dung của khối `footer`, làm nút phình to khi rê chuột. Tách lại thành hai khối
- Lời commit ghi "đã xóa CSS thí nghiệm" nhưng thực tế chưa xóa. Bài học: chạy `git diff --staged` xem lại trước khi commit

**Chưa làm:** 3 bài tập (menu có nền khi rê chuột, ô nhập đổi viền khi `:focus`, ảnh bo tròn) và 4 câu tự kiểm tra

## Ngày 4 · 15/10/2026 · Tuần 1

**Đã học:**
- CSS cho form: `label { display: block; }`, ô nhập `width: 100%`, `font: inherit`
- Specificity trong thực tế: `fieldset input` (2 thẻ) mạnh hơn `input` (1 thẻ) nên ghi đè được `width: 100%` cho radio
- Trạng thái `:hover` cho nút, `cursor: pointer`
- DevTools: tab Styles, luật bị gạch ngang là luật đã thua

**Đã làm:** thư mục `ngay-04-form`, CSS cho form, nút, fieldset; thí nghiệm "luật nào thắng" với 3 màu orange, lime, hotpink

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
