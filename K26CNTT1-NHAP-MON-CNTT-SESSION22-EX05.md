


**Quy trình 3 bước tra cứu bắt buộc** (để tự xử lý 80% vấn đề)

-   **Bước 1 — Googling**: copy nguyên văn lỗi trong dấu `"..."`, dùng `site:stackoverflow.com` / `site:github.com/.../issues`, lọc "trong vòng 1 năm", ưu tiên docs chính thức. Quy tắc: mở ít nhất 2 kết quả.
-   **Bước 2 — Community Search**: tìm trong Slack/Notion/wiki nội bộ trước (rất có thể anh chị khác đã gặp), rồi GitHub Issues (tab _Closed_) và forum chính thức.
-   **Bước 3 — AI Translation**: dùng AI để _dịch & giải thích_ lỗi, gợi ý nguyên nhân — **không phải lấy lệnh chạy mù**. Mọi lệnh `sudo`/`docker prune` do AI đưa ra đều phải kiểm chứng (nối với báo cáo IPO bạn làm ở bài trước).
-   Kèm **điều kiện escalate**: xong 3 bước mà chưa được → điền template → đăng `#support` → on-call phản hồi 30 phút.

**2. Bug Report Template — 4 mảnh ghép Context / Expected / Actual / Log**

-   Mỗi trường có gợi ý điền cụ thể (phiên bản Docker, lệnh nguyên văn, `docker logs`, `lsof -i :port`, đoạn `docker-compose.yml`…).
-   Có ô "Đã hoàn thành 3 bước tra cứu? (link kết quả)" — chặn người hay nhờ vả trước khi tự tìm.
-   Mọi trường trống = báo cáo bị trả lại.

**3. Ví dụ mẫu đã điền sẵn** — case "Port conflict 8080" (Postgres.app chiếm cổng), để thành viên nhìn vào là biết điền thế nào.

**4. Quy tắc vận hành nhóm** — đăng vào `#support` thay vì nhắn riêng, sau khi fix xong phải comment lại kết luận để tổng hợp vào wiki "Lỗi đã gặp" (chính là cơ sở dữ liệu giúp 80% vấn đề sau này tự giải quyết ở Bước 2).
