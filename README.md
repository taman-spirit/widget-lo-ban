# Thước Lỗ Ban mini

Khách tự kiểm một kích thước cửa, giường hay bàn thờ rơi vào cung tốt hay xấu.

*[Read this in English](README.en.md)*

**Xem nó chạy thật:** https://nhatnguyet.org/widget/lo-ban

## Dán hai dòng này là xong

```html
<div data-widget="lo-ban"></div>
<script async src="https://nhatnguyet.org/embed/w.js"></script>
```

Không cần tài khoản, không cần khoá API, không mất phí.

## Nó giúp gì cho trang của bạn

Dành cho trang bất động sản, xây dựng và nội thất: khách hỏi kích thước cửa suốt quá trình thi công, và widget trả lời ngay trên trang của bạn. Widget hỏi đang đo gì rồi tự chọn đúng một trong ba thước, khách không cần biết ba thước khác nhau chỗ nào.

## Vài điều nên biết trước

- Rơi vào cung xấu thì widget chỉ luôn hai kích thước đẹp gần nhất, một nhỏ hơn một lớn hơn, kèm mức chênh. Đó mới là thứ khách cần.
- Có ba loại thước cho ba nhóm vật. Khách chỉ chọn đang đo gì, widget tự lấy đúng thước.
- Đây là quy ước đo lường truyền thống, không có cơ sở khoa học, và kích thước công trình vẫn phải theo tiêu chuẩn kỹ thuật.

## Các bước

1. Dán mã nhúng vào trang tin đăng hoặc trang sản phẩm nội thất.
2. Khách bấm chọn vật đang đo, nhập kích thước rồi bấm tra.
3. Khung hẹp thì đặt data-size compact, dải thước trực quan sẽ được bỏ đi.

## Dán vào đâu

**WordPress.** Thêm một khối *HTML tuỳ chỉnh* vào bài hoặc vào widget
*Text* ở cột bên, rồi dán cả hai dòng vào đó. Đừng dán vào trình soạn thảo
thường: nó sẽ hiện ra đúng chữ mã thay vì chạy mã.

**Wix, Squarespace, Haravan, Shopify.** Dùng khối *Nhúng mã HTML* (Embed
HTML / Custom HTML) rồi dán vào.

**Site tự viết.** Dán thẳng vào chỗ bạn muốn widget xuất hiện. Dòng
`<script>` có thể để chung một chỗ nếu bạn nhúng nhiều widget, nó chỉ cần
xuất hiện một lần trên trang.

**Ghi chú về chiều rộng.** Widget tự co theo bề ngang chỗ bạn đặt nó. Nếu chỗ ấy hẹp dưới 280px thì thêm `data-size="compact"`;
nếu là một dải ngang rộng thì `data-size="wide"`.

## Chỉnh cho hợp trang của bạn

| Thuộc tính | Giá trị | Ý nghĩa |
|---|---|---|
| `data-widget` | `lo-ban` | Bắt buộc |
| `data-theme` | light hoặc dark | Mặc định light |
| `data-accent` | #b3341f | Màu nhấn dạng hex 6 ký tự, để khớp bộ nhận diện của bạn |
| `data-lang` | vi hoặc en | Mặc định vi |
| `data-size` | compact, standard hoặc wide | Mức chi tiết theo bề ngang khung: compact bỏ bớt chi tiết phụ, wide trải ngang. Mặc định standard |

Đặt hết mọi thứ widget này nhận thì trông như sau:

```html
<div data-widget="lo-ban" data-theme="dark" data-accent="#1f6f5c" data-size="compact"></div>
<script async src="https://nhatnguyet.org/embed/w.js"></script>
```

Muốn xem tận mắt trước khi dán lên trang thật thì mở
[`vi-du/index.html`](vi-du/index.html) bằng trình duyệt, không cần cài gì.

## Vài điều xin thưa trước

- Miễn phí cho website cá nhân và doanh nghiệp, không giới hạn lượt hiển thị.
- Giữ nguyên dòng ghi nguồn ở đáy widget. Đây là điều kiện đổi lại việc dùng
  miễn phí.
- Không nhúng trên trang cờ bạc, nội dung người lớn, lừa đảo hoặc vi phạm
  pháp luật Việt Nam.
- Nội dung là tri thức dân gian và quy ước văn hoá, để tham khảo, không phải
  lời khuyên về sức khoẻ, tài chính hay pháp lý.

Bản đầy đủ: [`DIEU-KHOAN.md`](DIEU-KHOAN.md) · [https://nhatnguyet.org/widget/dieu-khoan](https://nhatnguyet.org/widget/dieu-khoan)

## Nhật Nguyệt là ai

Nhật Nguyệt (https://nhatnguyet.org) là trang tra cứu lịch pháp và văn hoá tâm linh Việt
Nam: lịch âm tính theo múi giờ nước mình, can chi, tiết khí, giờ hoàng đạo,
tử vi, phong thuỷ, và một từ điển thuật ngữ.

Có một điều chúng tôi cố giữ cho bằng được, kể cả trong một khung widget
300px: nói rõ đâu là thứ tính ra được, đâu là quan niệm dân gian.

Ngày âm lịch, can chi, tiết khí là **tính ra được**: ai chạy cùng phép tính
cũng ra cùng kết quả, và chúng tôi công bố luôn bộ dữ liệu gốc theo giấy
phép CC BY 4.0 để bạn tự đối chiếu.

Giờ hoàng đạo, cung Bát Trạch, cung thước Lỗ Ban là **quy ước văn hoá**: có
bảng tra hẳn hoi, nhưng không phải phép đo. Widget cho bạn biết bảng nói gì,
còn tin tới đâu là việc của mỗi người.

Chỗ nào các phái không thống nhất, chúng tôi nói ra chỗ ấy, thay vì lặng lẽ
chọn một bên rồi trình bày như thể chỉ có một cách.

Dữ liệu mở: [GitHub](https://github.com/taman-spirit/du-lieu-am-lich) ·
[Hugging Face](https://huggingface.co/datasets/nhatnguyet)

## Thấy gì chưa ổn?

Mở một issue ngay trong kho này. Chúng tôi có đọc.

Toàn bộ thư viện widget: [https://nhatnguyet.org/widget](https://nhatnguyet.org/widget)
