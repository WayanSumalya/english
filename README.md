# Ucap English

Aplikasi latihan bicara bahasa Inggris berbasis web (single-file HTML), dengan dua mode:

- **Latihan Kalimat** — dengar contoh kalimat (normal / pelan), rekam ucapanmu lewat mikrofon, dan dapatkan skor kemiripan kata-per-kata (hijau = cocok, merah = meleset).
- **Ngobrol dengan AI** — percakapan langsung (suara atau teks) dalam skenario seperti pesan kopi, wawancara kerja, check-in hotel, atau obrolan bebas, lengkap dengan koreksi kalimat dan tips dalam Bahasa Indonesia setelah setiap giliran bicara.

## Cara pakai

Buka `index.html` langsung di browser (disarankan Chrome untuk dukungan pengenalan suara terbaik). Tidak perlu build step atau server — semuanya berjalan di satu file HTML.

Fitur "Ngobrol dengan AI" memakai kemampuan Claude Artifact (`window.claude.use("sample")`), jadi paling optimal saat dibuka sebagai Claude Artifact yang dipublikasikan. Jika dijalankan sebagai file HTML biasa di luar Claude, mode latihan kalimat (drill) tetap berfungsi penuh, sementara mode ngobrol dengan AI akan menampilkan pesan bahwa fitur tersebut tidak tersedia.

## Struktur

- `index.html` — seluruh aplikasi (markup, style, dan JavaScript) dalam satu file.
