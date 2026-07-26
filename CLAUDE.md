# Public — bản GitHub Pages

Thư mục này là repo GitHub Pages: `github.com/Khaduyadv/Dashboard` → https://khaduyadv.github.io/Dashboard/

## Không sửa tay `index.html`

`index.html` được **sinh tự động** bởi `Script/capnhat_bcqt.py` (hàm `publish_public()`),
kèm theo `git add -- index.html` → commit → push. Mọi sửa tay ở đây sẽ bị ghi đè ở lần chạy sau.

Muốn cập nhật dashboard: chạy script ở thư mục cha, đừng thao tác trong này.
Muốn đổi giao diện: sửa `Script/dashboard_template.html`, giữ nguyên chuỗi `__DATA__`.

## Chỉ can thiệp thủ công khi push thất bại

Giữ nguyên định dạng commit của script: `Cập nhật dashboard YYYY-MM-DD`, đẩy lên `origin main`.
Nếu gặp file khoá `.git/index.lock` hoặc `.git/HEAD.lock` còn sót lại, xoá rồi thử lại
(thường do một tiến trình git/đồng bộ khác đang giữ file — xem OneDrive, VS Code, antivirus).

## Lưu ý

Repo đang ở chế độ public — số liệu ngân sách, doanh thu gian hàng và tên nhân sự
trong `index.html` ai có link đều xem được.

Quy trình đầy đủ: `../CLAUDE.md` và `../Script/HUONG DAN.md`.
