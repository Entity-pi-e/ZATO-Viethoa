# Z.A.T.O. // I Love the World and Everything In It — Bản Việt hóa

Bản Việt hóa không chính thức cho visual novel **Z.A.T.O. // I Love the World and Everything In It** (bản Steam, Windows).

> Bạn cần sở hữu game bản quyền trên Steam. Bản Việt hóa chỉ chứa các file đã dịch, không chứa dữ liệu game gốc.

## Tải về

👉 Vào mục **[Releases](../../releases/latest)** và tải file `VietHoa_x.x.zip` mới nhất.

## Nội dung đã dịch

- Toàn bộ thoại 3 chương: Ira, Marina, Asya
- Giao diện, menu, phần cài đặt
- Các hình ảnh có chữ trong game

## Cách cài

1. Tắt game, giải nén file zip và chạy `VietHoa_x.x.exe`.
2. Bộ cài tự tìm game trên Steam. Bấm **Next → Install → Finish**.
3. Mở game từ Steam.

**Đã cài bản Việt hóa của nhóm khác?** Xóa thư mục `game` trong thư mục cài game, rồi trên Steam chọn *Properties → Installed Files → Verify integrity of game files* để tải lại bản gốc, sau đó mới cài.

Hướng dẫn đầy đủ và cách xử lý sự cố: xem [`HuongDan.txt`](HuongDan.txt).

## Gỡ bản Việt hóa

**Settings → Apps → Installed apps**, tìm *Z.A.T.O. … - Việt hóa* và bấm **Uninstall**. Game trở về tiếng Anh gốc.

## Về cảnh báo virus

Một vài phần mềm diệt virus có thể báo nhầm vì file cài không có chữ ký số trả phí. Các phần mềm lớn (Windows Defender, Kaspersky, ESET, BitDefender…) đều báo sạch. Kết quả kiểm tra: [VirusTotal]([link VirusTotal]).

Chỉ tải bản Việt hóa từ trang Releases của kho này.

## Báo lỗi dịch

Mở một [Issue](../../issues) hoặc liên hệ: [Fanpage / Discord của nhóm]

## Dành cho người làm bản dịch

Thư mục [`CongCu`](CongCu) chứa công cụ dùng để đóng gói bản Việt hóa:

| File | Công dụng |
| --- | --- |
| `tao_banva.py` | So sánh thư mục game gốc và thư mục đã dịch, chỉ lấy các file đã sửa (bỏ qua save, cache, file giải nén từ `.rpa` chưa sửa) |
| `VietHoa.iss` | Script [Inno Setup](https://jrsoftware.org/isinfo.php) tạo bộ cài: tự tìm game trên Steam, sao lưu file gốc, có trình gỡ cài đặt |

Cách dùng:

```
python tao_banva.py --goc "<thư mục game Steam sạch>" --dich "<thư mục bản dịch>"
```

Sau đó mở `VietHoa.iss` bằng Inno Setup 6.4+ / 7 và bấm **Build → Compile**.

## Ghi công

- Game gốc: Z.A.T.O. // I Love the World and Everything In It — mọi quyền thuộc về tác giả. Hãy ủng hộ tác giả bằng cách mua game trên Steam.
- Bản dịch: [Tên nhóm dịch]
- Bộ cài tạo bằng [Inno Setup](https://jrsoftware.org/isinfo.php).
