# 🌐 Static Website di NodeMCU ESP8266 (HTML + CSS)

Proyek ini menunjukkan cara membuat dan meng-host **website statis (HTML + CSS)** langsung dari **NodeMCU ESP8266**, tanpa perlu hosting eksternal. Website akan disimpan di memori internal (LittleFS) dan ditampilkan saat IP device diakses melalui browser.

---

## 📦 Fitur

- ✅ Web server menggunakan ESP8266
- ✅ File HTML dan CSS disimpan di LittleFS
- ✅ Tampilan modern, responsive, dan ringan
- ✅ Cocok untuk UI sederhana proyek IoT

---

## 🛠️ Tools & Library

- Arduino IDE (v2.x)
- Board: ESP8266 (NodeMCU)
- Library: `ESP8266WiFi`, `ESP8266WebServer`, `LittleFS`
- Plugin: **ESP8266 LittleFS Data Upload Tool**

---

## 🧾 Struktur File

```
nodemcuweb/
├── nodemcuweb.ino         <-- File utama Arduino
├── data/                  <-- Folder khusus untuk file web (akan di-upload ke LittleFS)
│   ├── index.html         <-- Halaman utama website
│   └── style.css          <-- Styling tampilan web
└── README.md              <-- Dokumentasi proyek
```

---

## 🚀 Cara Upload File HTML & CSS ke LittleFS

### 1. Install Plugin LittleFS untuk Arduino IDE 2.x

- Unduh dari sini: [ESP8266 LittleFS Plugin](https://github.com/earlephilhower/arduino-esp8266littlefs-plugin/releases)
- Ekstensi file: `.vsix`
- Langkah:
  - Buka folder:  
     `C:\Users\<username>\.arduinoIDE\`
  - Buat folder bernama `plugins` (jika belum ada)
  - Pindahkan file `.vsix` ke dalam folder `plugins`
  - Restart Arduino IDE

### 2. Upload File ke LittleFS

- Pastikan folder `data/` berisi file `index.html` dan `style.css`
- Di Arduino IDE, tekan `Ctrl+Shift+P`
- Cari dan pilih:  
  **"Upload LittleFS to Pico/ESP82666"**
- Tunggu hingga proses upload selesai

📖 Referensi lengkap untuk pasang plugin:  
👉 https://randomnerdtutorials.com/arduino-ide-2-install-esp8266-littlefs/

---
