# Changelog / Nhật ký Cập nhật

All notable changes to **RustTube** (Windows 11 64-bit Edition) are documented in this file.

---

## [v1.3.5] — 2026-11-26

### 🇻🇳 Tiếng Việt
- **Bộ định tuyến Link Hệ thống Windows 11 (Smart Link Router — Mở thẳng từ Zalo, Discord, Messenger, Mail...):** Đăng ký chuẩn `RustTube` vào **Windows 11 Default Apps** (`StartMenuInternet` + `RustTubeHTM`). Khi bấm bất kỳ link video YouTube nào từ ứng dụng khác (kể cả link bọc qua `l.messenger.com` / `l.facebook.com`), Windows mở thẳng video trong **RustTube** mà không bật tab trình duyệt; mọi link trang web khác được bộ định tuyến nhân Rust chuyển thẳng sang trình duyệt thật của bạn (Chrome / Edge / Cốc Cốc / Brave / Firefox) trong `< 2ms`.

### 🇬🇧 English
- **Windows 11 System-Wide Smart Link Router:** Registers **RustTube** in Windows 11 Default Apps (`StartMenuInternet` + `RustTubeHTM`) so clicking any YouTube link in external apps (Zalo, Discord, Messenger, Telegram, Mail, Office — including social redirect wrappers) opens directly inside RustTube with zero browser tabs, while forwarding all non-YouTube URLs straight to your chosen browser in `< 2ms`.

---

## [v1.3.4] — 2026-11-26

### 🇻🇳 Tiếng Việt
- **Đăng nhập YouTube trực tiếp ngay trong App (Khắc phục triệt để lỗi Cookie DPAPI v20):** Tích hợp cửa sổ đăng nhập WebView2 chính chủ ngay trong RustTube, tự động lưu cookie phiên cục bộ mà không cần đóng Chrome/Edge, không cần cài tiện ích phụ và miễn nhiễm hoàn toàn với khoá App-Bound Encryption (`v20`) trên Windows 11.
- **Watch Sheet kéo thả trực tiếp 60 FPS kiểu YouTube Mobile:** Giữ Trang chủ hiển thị sống động ngay bên dưới trang Xem; khi nhấn kéo video đang phát xuống (hoặc kéo MiniPlayer ngược lên), khung video thu phóng liên tục theo ngón tay/chuột đồng bộ thời gian thực với nền Trang chủ và hiệu ứng Ambient Light mà không khựng hay dừng phát.
- **Khử trùng lặp video đề xuất & Giới hạn spam kênh tổng hợp:** Bổ sung bộ lọc dấu vân tay tiêu đề kết hợp giới hạn tối đa số video mỗi kênh và chống xếp cạnh nhau trên Trang chủ, Thịnh hành và cột Đề xuất.
- **Tự mở Link YouTube thẳng trong App:** Hỗ trợ giao thức `rusttube://`, bắt link trực tiếp trong phần mô tả/bình luận, dán vào thanh Tìm kiếm, bấm `Ctrl+V` toàn cục hoặc gợi ý nhanh từ Clipboard kèm Bookmark chuyển 1 chạm từ trình duyệt.

### 🇬🇧 English
- **Built-in Native WebView2 YouTube Sign-In (Zero DPAPI v20 Errors):** Sign in to Google/YouTube directly inside RustTube without closing Chrome/Edge, installing extensions, or hitting Chromium 127+ App-Bound Encryption (`DPAPI`) blocks on Windows 11.
- **YouTube-Mobile 2-Layer Watch Sheet & Live 60 FPS Synchronized Video Drag:** Keep the Home/Browse grid alive underneath Watch; dragging the playing video downward (or pulling the MiniPlayer upward) smoothly interpolates the live video, Ambient Light fade, and Home reveal at 60 FPS with harmonic spring physics.
- **Smart Recommendation Deduplication & Channel Diversity:** Eliminates near-identical compilation re-uploads via normalized title fingerprinting, enforces per-channel caps, and spaces out same-creator videos.
- **Direct In-App YouTube Link Handling:** Registered `rusttube://` Windows protocol, in-app description/comment link interception, Search bar & global `Ctrl+V` URL paste, smart Clipboard detection pill, and 1-click browser Bookmarklet.

---

## [v1.3.3] — 2026-11-26

### 🇻🇳 Tiếng Việt
- **Gộp thanh tiêu đề Frameless Liquid Glass chuẩn Windows 11 (`48px`):** Loại bỏ thanh tiêu đề hệ điều hành chồng chéo phía trên, tích hợp nút điều khiển cửa sổ (`─ □ ✕`) + bo góc tròn DWM gốc của Windows 11, gộp kính lúp & gợi ý phím `/` vào trong ô tìm kiếm và mở rộng thêm `42px` không gian hiển thị kèm hiệu ứng Ambient Light tràn sát mép trên.

### 🇬🇧 English
- **Unified 48px Frameless Windows 11 Liquid Glass Titlebar & Header:** Merged OS titlebar and app header into a single `48px` frosted glass bar with native Windows 11 DWM rounded corners, integrated search capsule (`🔍` + `/` shortcut badge), quick language/theme toggles, and native-style caption buttons (`─ □ ✕`).

---

## [v1.3.2] — 2026-11-26

### 🇻🇳 Tiếng Việt
- **Tinh chỉnh nút Thu nhỏ MiniPlayer 60 FPS:** Giữ thao tác thu nhỏ / phóng to mượt 60 FPS thuần bằng nút bấm (`⌄` góc trên trái, nút MiniPlayer dưới thanh điều khiển và phím tắt `I`) để tránh trượt chuột nhầm khi đang xem trên máy tính.

### 🇬🇧 English
- **Refined Button-Driven 60 FPS MiniPlayer Morphing:** Streamlined MiniPlayer transitions to clean button triggers (`⌄` top-left chevron, bottom-dock MiniPlayer button, and `I` shortcut) to prevent accidental mouse drags on desktop.

---

## [v1.3.1] — 2026-11-26

### 🇻🇳 Tiếng Việt
- **Hiển thị đầy đủ Ảnh bìa (Thumbnail) ở MiniPlayer khi bật Chỉ nghe âm thanh:** Sửa lỗi mất ảnh bìa khi thu nhỏ trình phát ở chế độ Audio-Only và tự động dự phòng ảnh `hqdefault` sắc nét cho mọi video.

### 🇬🇧 English
- **Audio-Only MiniPlayer Cover Art Fix:** Fixed missing thumbnail cover art when minimizing the player in Audio-Only mode, with automatic `hqdefault` fallback support.

---

## [v1.3.0] — 2026-11-26

### 🇻🇳 Tiếng Việt
- **Cử chỉ kéo thu nhỏ & Hiệu ứng chuyển cảnh 60 FPS (Pull-to-MiniPlayer FLIP):** Hỗ trợ nhấn giữ chuột kéo trực tiếp khung video xuống góc phải dưới (hoặc kéo ngược từ MiniPlayer lên) kèm nút thu nhỏ `⌄` góc trên trái và nút MiniPlayer dưới thanh điều khiển — chuyển cảnh mượt mà 60 FPS không khựng hình.

### 🇬🇧 English
- **Interactive Pull-to-MiniPlayer Gesture & 60 FPS FLIP Morphing:** Drag the video downward to dock smoothly into the bottom-right MiniPlayer (or drag upward to expand), paired with dedicated top-left `⌄` and player-dock MiniPlayer buttons.

---

## [v1.2.9] — 2026-11-26

### 🇻🇳 Tiếng Việt
- **Thanh Chip Liquid Glass tự thích ứng:** Nút chủ đề trên Trang chủ dùng hiệu ứng kính mờ phản quang đồng bộ và tự động thay đổi thể loại + ghim Kênh/Nghệ sĩ yêu thích theo dữ liệu xem cục bộ (hoặc nhận diện vùng theo IP khi không dùng Cookie).
- **Bộ đệm Trang chủ thông minh & Header tinh gọn:** Chuyển qua lại giữa Cài đặt / Thư viện và Trang chủ tức thì (`0ms`, không bị tự làm mới gây giật); dời Logo sát góc trái và giữ cố định cột điều hướng gọn.
- **Ambient Light tràn toàn cửa sổ:** Nâng cấp chiếu ánh sáng thời gian thực qua lớp Portal kết hợp DirectComposition GPU Pyramid Blur — ánh sáng tràn mượt dưới cả Header và Sidebar kính mờ.
- **Chế độ Offline & Tự động kết nối lại:** Tích hợp trình phát `.mp4` / `.mp3` ngoại tuyến ngay trong ứng dụng; chia thông báo mất mạng thông minh cho 2 trường hợp (đang mở cửa sổ App vs đang chạy nền dưới System Tray Windows 11); tự nối lại đúng giây đang xem khi có mạng lại; đề xuất tải dự phòng MP4/MP3 khi xem lâu phòng hờ mất điện.
- **Cài đặt hệ thống mới & Sao lưu JSON:** Tuỳ chỉnh độ mờ kính (Liquid Glass Opacity), hành vi đóng cửa sổ (`System Tray` / `Thoát hẳn`), khởi động cùng Windows 11, tải nhanh 1 chạm (`MP4 1080p` / `MP3 320kbps`) và Sao lưu / Khôi phục thư viện ra tệp `.json`.

### 🇬🇧 English
- **Adaptive Liquid Glass Topic Chips:** Home category bar dynamically adapts to your local watch & like history (pinning favorite genres and creators) with IP-based regional cold-start support.
- **Instant Home Feed Cache & Streamlined Header:** Zero-reload switching between Settings/Library and Home; cleaner top-left brand header paired with a fixed compact Liquid Glass navigation rail.
- **Full-Window Unclipped Ambient Light:** Upgraded to a viewport Portal + DirectComposition GPU Pyramid Blur so real-time video light refracts seamlessly beneath the frosted Header and Sidebar.
- **Built-in Offline Mode & Smart Auto-Reconnect:** Play local `.mp4` and `.mp3` files directly inside RustTube without Internet; distinct offline notifications for Foreground (Liquid Glass pill) vs Background System Tray (native Windows 11 toast); seamless timestamp auto-resume when back online; proactive power/network-outage backup download prompt.
- **Overhauled Windows 11 Settings & JSON Backup:** Added System/Dark/Light theme sync, Liquid Glass opacity slider, Close-to-Tray vs Exit toggle, Launch at Windows Startup, 1-click Quick Download (`MP4 1080p` / `MP3 320kbps`), and `.json` Library Backup & Restore.

---

## [v1.2.8] — 2026-11-25
- Integrated real-time video-synced **Ambient Light for YouTube™** (`⚙️ AL` player dock menu + `[G]` shortcut).
- Responsive CSS Container-Query player control dock preventing button overlap on narrow split-screen windows.

## [v1.2.7] — 2026-11-25
- Streamlined core VOD & Music experience by removing Live/Shorts/Subscriptions clutter.
- Standardized **Windows 11 (64-bit)** exclusive hardware architecture.

## [v1.2.6] — 2026-11-25
- Restored pure Windows 11 DirectComposition D3D11VA hardware-decoded playback up to **4K/8K 60FPS** and dropped legacy 32-bit builds.

## [v1.2.5] — 2026-11-25
- Added Autoplay Queue, Subtitles `CC` (with Vietnamese auto-translation), Video Chapters, Theater Mode, Audio-Only Mode, Sleep Timer, and Return YouTube Dislike.
