# NT101.Q21 - NHÓM 7

## Đồ án môn học An toàn mạng máy tính

![C#](https://img.shields.io/badge/C%23-WinForms-blue)
![RSA](https://img.shields.io/badge/Cryptography-RSA-green)
![Playfair](https://img.shields.io/badge/Cryptography-Playfair-orange)
![License](https://img.shields.io/badge/License-Educational-red)

---

## 👥 Thành viên nhóm

| Họ và tên        | MSSV     | Vai trò     |
| ---------------- | -------- | ----------- |
| Đinh Võ Gia Huy  | 24520656 | Trưởng nhóm |
| Nguyễn Hoàng Phú | 24521358 | Thành viên  |
| Huỳnh Cao Kỳ     | 24520923 | Thành viên  |

---

## 📖 Giới thiệu đồ án

Đồ án được thực hiện trong khuôn khổ môn học **NT101.Q21 - An toàn mạng máy tính** tại Trường Đại học Công nghệ Thông tin - ĐHQG TP.HCM.

Mục tiêu của đề tài là nghiên cứu và triển khai các kỹ thuật bảo mật cơ bản trong lĩnh vực mật mã học, đồng thời xây dựng các tài liệu học tập trực quan giúp sinh viên tiếp cận các công cụ giám sát an ninh mạng.

Đề tài gồm hai phần:

### Phần A - Phát triển ứng dụng mật mã

Xây dựng ứng dụng **CryptoAppForNC_PHK** bằng C# WinForms hỗ trợ:

* Mã hóa và giải mã bằng thuật toán Playfair Cipher.
* Mã hóa và giải mã bằng thuật toán RSA.
* Sinh khóa RSA tự động.
* Hiển thị ma trận khóa Playfair.
* Giao diện trực quan, dễ sử dụng.

### Phần B - Video bài giảng

Xây dựng chuỗi video hướng dẫn sử dụng các công cụ giám sát an ninh mạng:

* Netstat
* TCPView
* CurrPorts
* Process Viewer

---

## 🚀 Chức năng chính

### 🔐 Playfair Cipher

* Tạo ma trận khóa 5x5 từ từ khóa.
* Chuẩn hóa dữ liệu đầu vào.
* Mã hóa văn bản theo Playfair.
* Giải mã văn bản theo Playfair.
* Hiển thị trực tiếp ma trận khóa.

### 🔑 RSA Cryptosystem

* Sinh khóa RSA từ các tham số p, q, e.
* Tính toán:

  * n = p × q
  * φ(n)
  * d bằng thuật toán Euclid mở rộng.
* Mã hóa văn bản bằng khóa công khai.
* Giải mã văn bản bằng khóa bí mật.
* Hỗ trợ Auto Key phục vụ kiểm thử.

### 🎓 Video học tập

* Hướng dẫn sử dụng Netstat.
* Hướng dẫn sử dụng TCPView.
* Hướng dẫn sử dụng CurrPorts.
* Hướng dẫn sử dụng Process Viewer.
* Minh họa các tình huống kiểm tra và giám sát hệ thống thực tế.

---

## 🛠️ Công nghệ sử dụng

| Thành phần         | Công nghệ                    |
| ------------------ | ---------------------------- |
| Ngôn ngữ lập trình | C#                           |
| Framework          | .NET WinForms                |
| Thư viện           | System.Numerics (BigInteger) |
| IDE                | Microsoft Visual Studio      |
| Công cụ kiểm thử   | CrypTool                     |

---

## 📂 Cấu trúc dự án

```text
.
├── CryptoAppForNC_PHK/
│   ├── Forms/
│   │   ├── Main.cs
│   │   ├── PlayFair.cs
│   │   └── RSA.cs
│   ├── Resources/
│   └── Program.cs
│
├── Videos/
│   ├── Bai1.mp4 (Netstat & Fport)
│   ├── Bai2.mp4 (TCPView & Currport)
│   ├── Bai3.mp4 (Process Viewer)
│
└── README.md
```

---

## ⚙️ Cài đặt

### Yêu cầu

* Windows 10/11
* .NET Framework
* Microsoft Visual Studio 2022 trở lên

### Clone Repository

```bash
git clone https://github.com/<username>/<repository>.git
```

### Chạy chương trình

Mở solution bằng Visual Studio và thực hiện:

```bash
Build -> Build Solution
```

Sau đó:

```bash
F5
```

hoặc

```bash
Ctrl + F5
```

---

## 📘 Hướng dẫn sử dụng

### Playfair

1. Chọn **Playfair** từ màn hình chính.
2. Nhập khóa (Key).
3. Nhấn **Generate Matrix**.
4. Nhập văn bản cần xử lý.
5. Chọn:

   * Encrypt
   * Decrypt
6. Kết quả hiển thị tại vùng Output.

### RSA

1. Chọn **RSA** từ màn hình chính.

2. Nhập:

   * p
   * q
   * e

   hoặc nhấn **Auto Key**.

3. Nhập văn bản cần mã hóa hoặc giải mã.

4. Chọn:

   * Encrypt
   * Decrypt

5. Kết quả hiển thị tại Output.

---

## 🧪 Kiểm thử

Ứng dụng được kiểm thử bằng cách đối chiếu kết quả với phần mềm CrypTool.

### Playfair

* Kiểm tra mã hóa.
* Kiểm tra giải mã.
* So sánh kết quả với CrypTool.

### RSA

* Kiểm tra sinh khóa.
* Kiểm tra mã hóa.
* Kiểm tra giải mã.
* Đối chiếu với CrypTool.

---

## 📊 Kết quả đạt được

* Hoàn thành ứng dụng mật mã Playfair và RSA.
* Thực hiện chính xác các chức năng mã hóa và giải mã.
* Kết quả trùng khớp với CrypTool.
* Hoàn thành chuỗi video hướng dẫn công cụ giám sát an ninh mạng.
* Củng cố kiến thức về mật mã học và an toàn thông tin.

---

## 🎯 Hướng phát triển

* Bổ sung thuật toán AES.
* Bổ sung thuật toán ECC.
* Hỗ trợ chữ ký số.
* Nâng cấp giao diện lên WPF hoặc Web Application.
* Tích hợp lưu trữ và quản lý khóa.

---

## 👨‍🏫 Giảng viên hướng dẫn

**ThS. Tô Nguyễn Nhật Quang**

---

## 📄 License

Dự án được phát triển phục vụ mục đích học tập và nghiên cứu trong môn học **NT101.Q21 - An toàn mạng máy tính** tại Trường Đại học Công nghệ Thông tin - ĐHQG TP.HCM.
