# ChemCool: Media Pembelajaran Kimia

Situs statis media pembelajaran kimia ("ChemCool") untuk materi redoks dan tata nama senyawa. Dibangun dengan HTML, CSS (Bootstrap, template Colorlib), dan JavaScript.

## Isi

- `index.html`: halaman utama.
- Halaman materi dan perangkat ajar: bahan ajar, LKS/LKPD, praktikum, pengayaan, pretest/posttest, tutorial, PowerPoint, video, RPP, dan silabus (`*.html` di root).
- Kuis pilihan ganda: `quiz.html`, `game.html`/`game.js` (soal dari `questions.json`, 10 soal per sesi), `end.html`, `highscores.html` (skor disimpan di `localStorage`).
- Flipbook HTML5 (ekspor Flip PDF Professional) di folder `bahanAjarRedoks/`, `bahanAjarTata/`, `LKPDRedoks/`, `LKPDTata/`, `LKDPRedoksII/`, `PraktikumRedoks/`, `TataNamaSenyawaII/`.
- `css/`, `sass/`, `js/`, `fonts/`, `img/`: aset template.

## Cara Menjalankan

Sajikan folder ini lewat web server statis (kuis memuat `questions.json` via `fetch`), misalnya:

```bash
python -m http.server 8000
```

lalu buka `http://localhost:8000/`.
