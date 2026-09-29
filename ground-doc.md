# Ground Doc — Chatbot Webinar Eintio

Source of truth isi chatbot. Kalau mau ganti jawaban, edit di sini (lalu salin ke `chatbot.js`).

## Transcript asal

```
hai eintio ?
hai satriya

kita mau adakan webinar ?
yaa bener banget

webinar apa ?
bikin chatbot dong

siapa narsumnya ?
Mimin sambungin ke narasumbernya yaa
```

## Pertanyaan yang dijawab chatbot

| Kata kunci | Balasan bot |
|---|---|
| hai / halo / hello / hi | Salam balik + tawarkan bantuan |
| webinar | Ya, ada rencana webinar |
| apa / topik / topic | Topiknya: bikin chatbot |
| narsum / старос / pembicara / speaker | NarCOND — belum diisi |
| kontak / wa / whatsapp | 081122225804 |
| lain | Fallback |

> `NarCOND` = placeholder. Isi begitu nama narasumber sudah pasti, di `chatbot.js` (`ANSWERS.narasum`).
