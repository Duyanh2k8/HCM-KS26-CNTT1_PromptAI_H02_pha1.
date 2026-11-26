# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 04
- **Họ tên:** Nguyễn Ngọc Duy Anh
- **Lớp:** HCM-KS26_CNTT1
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** Gemini

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt vé xe ra JSON

**KET QUA AI**

```text
[
{
"ma_tuyen": "SGDL",
"ngay_di": "2026-12-22",
"ve_nguoi_lon": 2,
"ve_tre_em": 1,
"loai_cho": "giuong",
"ghi_chu": null
},
{
"ma_tuyen": "SGNT",
"ngay_di": "2027-01-02",
"ve_nguoi_lon": 3,
"ve_tre_em": 0,
"loai_cho": null,
"ghi_chu": "một người đang mang thai 6 tháng"
},
{
"ma_tuyen": "SGCT",
"ngay_di": null,
"ve_nguoi_lon": 4,
"ve_tre_em": 0,
"loai_cho": "ghe",
"ghi_chu": "bà nội đi xe lăn"
}
]
```

**Link trò chuyện:** https://share.gemini.google/RKzP80Vc7qYe

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
* **Bước 1: Tiền vé người lớn**
Đoàn đi tuyến SGDL (giá vé người lớn 320.000 đồng/vé) với số lượng 8 người lớn.
Phép tính: 8 × 320.000 = 2.560.000 đồng.
* **Bước 2: Tiền vé trẻ em (dựa theo tiêu chí độ tuổi của trẻ)**
* 3 trẻ em (6, 7 và 9 tuổi) thuộc nhóm từ 5 đến 10 tuổi, tính 75% giá vé người lớn: 3 × (320.000 × 75%) = 3 × 240.000 = 720.000 đồng.
* 1 bé 2 tuổi thuộc nhóm dưới 5 tuổi (ngồi cùng người lớn), được miễn phí: 1 × 0 = 0 đồng.
Phép tính tổng tiền vé trẻ em: 720.000 + 0 = 720.000 đồng.


* **Bước 3: Tiền vé = tiền vé người lớn + tiền vé trẻ em**
Phép tính: 2.560.000 + 720.000 = 3.280.000 đồng.
* **Bước 4: Giảm giá đoàn**
Đoàn có 8 người lớn (thỏa điều kiện từ 6 người lớn trở lên) nên được giảm 5% trên tổng tiền vé.
* Số tiền được giảm: 3.280.000 × 5% = 164.000 đồng.
* Tiền vé sau giảm: 3.280.000 - 164.000 = 3.116.000 đồng.


* **Bước 5: Phụ thu hành lý cồng kềnh**
Đoàn có 2 kiện hành lý cồng kềnh, mức phụ thu 100.000 đồng/kiện (không giảm giá).
Phép tính: 2 × 100.000 = 200.000 đồng.
* **Bước 6: Tổng tiền = tiền vé sau giảm + phụ thu**
Phép tính: 3.116.000 + 200.000 = 3.316.000 đồng.

[RESULT: 3.316.000 đồng]
```

**Link trò chuyện:** https://share.gemini.google/ApAh6MAWQwmR

### b) Kiểm tra kết quả AI

(Ghi kết luận AI đúng hay sai; nếu sai, ghi bước sai đầu tiên và kết quả đúng của bước đó – xoá dòng này)

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
"loai_su_co": "sai_loai_xe",
"so_khach": 3,
"so_chang_bi_doi": 2,
"tom_tat": "Khách đặt giường nằm cho 3 người nhưng bị đổi sang ghế ngồi cả 2 chặng."
}
```

**Link trò chuyện:** https://share.gemini.google/vvHW8chPcXzH

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
(Dán câu trả lời của AI vào đây (bấm nút Copy dưới câu trả lời) – xoá dòng này)
```

**Link trò chuyện:**
