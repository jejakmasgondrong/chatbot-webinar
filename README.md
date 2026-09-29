# Chatbot Webinar Eintio

Chatbot sederhana (satu file HTML, tanpa backend) yang menjawab pertanyaan tentang webinar Eintio.

## Jalankan

Buka `index.html` di browser. Ctrl+Shift+I → Console untuk cek log.
Atau dari terminal:

```bash
xdg-open /media/gondrong/DATA/Workspace/Eintio/chatbot-webinar/index.html
```

## Test

Tambah `?test=1` di URL → 13 case routing dijalankan, hasil di console (`PASS semua case`).

## Edit jawaban

Semua balasan ada di `INTENTS` (`index.html`). Tiap intent punya `id`, `match` (regex), `replies[]` (diputar), dan `followUp[]` opsional. `route()` mengembalikan intent yang cocok pertama, `replyTo()` merakit jawabannya. Urutan penting: tambah intent spesifik sebelum `webinar` supaya tidak ketangkap yang umum.

Isi sumber: `ground-doc.md` (transcript percakapan yang jadi dasar).

`jadwal` harus di atas `webinar`, karena "kapan webinarnya dimulai?" mengandung kata "webinar" — first-match akan ambil yang lebih dulu.

## Deploy

Static file — upload ke hosting mana saja (Vercel/Netlify/GitHub Pages) tanpa build step.
