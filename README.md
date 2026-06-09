# Mini Game Lab

Bộ sưu tập mini game — mỗi game thể hiện một cơ chế chơi riêng.  
Chạy hoàn toàn trên **GitHub Pages** (tĩnh, không cần backend).

## Cấu trúc thư mục

```
/
├── index.html          ← Trang chủ — hiển thị danh sách game
├── admin.html          ← Trang admin (đăng nhập để quản lý game)
├── games.json          ← Dữ liệu danh sách game (tay commit)
└── games/
    ├── dogpile/
    │   └── index.html
    └── <tên-game>/
        └── index.html
```

## Quy trình thêm game mới

1. Tạo thư mục `games/<tên-game>/` và đặt file `index.html` vào.
2. Mở `admin.html` trên trình duyệt → đăng nhập.
3. Điền thông tin game → nhấn **Thêm vào danh sách**.
4. Nhấn **Tải file** để download `games.json` mới.
5. Thay thế `games.json` cũ trong repo → commit & push.

## Đổi mật khẩu admin

Mở `admin.html`, tìm dòng:

```js
const ADMIN_PASSWORD = 'minigamelab2025';
```

Đổi thành mật khẩu bạn muốn rồi commit.

## Deploy lên GitHub Pages

1. Tạo repo mới trên GitHub.
2. Push toàn bộ folder này lên branch `main`.
3. Vào **Settings → Pages → Source: Deploy from branch → main / (root)**.
4. GitHub tự build — sau ~1 phút trang sẽ live tại  
   `https://<username>.github.io/<repo-name>/`

## Games hiện có

| Game | Mechanic |
|------|----------|
| Dogpile | Merge / Physics |
