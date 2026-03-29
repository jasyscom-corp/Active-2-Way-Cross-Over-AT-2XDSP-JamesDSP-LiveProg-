# AT-2XDSP — Active 2 Way Crossover LR4 DSP Processor

**AT-2XDSP** adalah preset/script **real-time DSP crossover** untuk **JamesDSP LiveProg** yang dirancang untuk membentuk karakter subwoofer yang **tight, clean, presisi, dan tetap punya rasa “glerr” di ultra-low** tanpa membuat sistem jadi gemuruh atau kehilangan kontrol.

Repo ini dibuat untuk kebutuhan praktik lapangan dan eksperimen tuning audio dengan pendekatan yang mirip sistem pro-audio: **phase-aware, crossover terkontrol, dan headroom-conscious**.

---

## Ringkasan

AT-2XDSP fokus pada tiga hal utama:

1. **Pemisahan sub dan mid yang rapi**
2. **Karakter sub yang dalam tetapi terkontrol**
3. **Proteksi transien supaya sub tidak bocor ke frekuensi atas**

Hasil yang dituju adalah suara yang terasa besar, padat, dan “hidup”, tetapi tetap nyaman didengar lama.

---

## Fitur Utama

- **LR4 crossover** untuk pemisahan sub dan mid yang lebih presisi
- **Subsonic protection** untuk menahan frekuensi ultra-rendah yang tidak perlu
- **Phase alignment** untuk membantu sub dan mid menyatu
- **All-pass compensation** untuk koreksi fase tambahan
- **Ultra Low Enhancer** untuk menambah rasa 30–45 Hz tanpa membuat sub menjadi boomy
- **Auto headroom** untuk menahan level saat output mulai terlalu padat
- **Transient guard** untuk mengurangi bocor hi-hat, clap, kick attack, dan snare body ke jalur sub
- **Mobile-oriented**: ditata agar masih masuk akal dipakai di perangkat harian, walau versi yang lebih kompleks tetap bisa berat

---

## Filosofi Suara

Proyek ini bukan sekadar “bass besar”. Tujuannya adalah:

- bass yang **terasa**
- bass yang **punya bentuk**
- bass yang **berhenti dengan rapi**
- bass yang **tidak menyapu area mid-high**

Kalau sebuah sistem hanya terdengar besar tetapi kabur, biasanya masalahnya ada di:
- overlap crossover
- phase yang tidak cocok
- kontrol transien yang lemah
- headroom yang terlalu sempit

AT-2XDSP berusaha mengatasi itu dengan pendekatan yang tetap sederhana dan efektif.

---

## Versi yang Tersedia

### V17 — Stable Core + Ultra Low Enhancer
Versi ini adalah basis yang paling aman dan paling seimbang.

**Ciri utamanya:**
- clean
- tight
- stabil
- sub tetap hidup
- cocok untuk pemakaian harian

**Karakter suara:**
- sub terasa presisi
- SPL besar tetapi tidak liar
- ultra-low masih ada rasa “glerr”
- tidak terlalu banyak proses dinamis

**Cocok untuk:**
- pengguna yang ingin hasil aman dan stabil
- perangkat dengan CPU terbatas
- tuning harian yang tidak ingin ribet

---

### V18 — Hajatan Killer / Scene-Based Mode
Versi ini dibuat untuk mengeksplorasi karakter yang lebih agresif dan lebih “lapangan”.

**Catatan penting:**
- versi ini lebih eksperimen
- bisa terasa lebih liar dibanding V17
- kalau perangkat kuat, karakter ini bisa menyenangkan
- kalau perangkat lemah, bisa terasa lebih berat

**Karakter suara:**
- lebih tebal
- lebih “ngegede”
- lebih dekat ke rasa sound lapangan
- tetap punya kontrol dasar, tetapi lebih berani

**Cocok untuk:**
- eksperimen
- perangkat yang masih punya tenaga lebih
- pengguna yang ingin karakter “hajatan” atau “festival feel”

---

### V19 — Adaptive Music Analyzer
Versi ini menambahkan analisis musik adaptif untuk membaca kecenderungan energi low, mid, dan high secara realtime.

**Catatan penting:**
- ini versi yang paling kompleks
- paling kaya fitur
- juga paling berat untuk CPU/HP tertentu

**Karakter suara:**
- lebih pintar menyesuaikan tuning
- bisa terasa sangat canggih kalau perangkat kuat
- tetapi bisa menimbulkan patah-patah jika engine atau device kewalahan

**Cocok untuk:**
- eksperimen lanjut
- perangkat yang kuat
- pengguna yang ingin eksplorasi karakter otomatis

---

### V20 — Mobile Optimized High-Quality
Versi ini dibuat untuk menyeimbangkan kualitas dan beban komputasi.

**Tujuan utama:**
- tetap terdengar high-end
- tetap clean
- tapi jauh lebih ringan dari versi yang terlalu banyak guard

**Karakter suara:**
- lebih stabil
- lebih aman dijalankan di HP
- masih punya rasa sub yang mahal
- lebih cocok untuk penggunaan harian di perangkat mobile

**Cocok untuk:**
- HP
- buffer audio menengah/besar
- pengguna yang ingin stabilitas di atas eksperimen

---

## Rekomendasi Pemakaian

Kalau kamu ingin memilih versi berdasarkan kebutuhan:

- **V17** → pilihan paling aman
- **V18** → pilihan karakter agresif
- **V19** → pilihan paling canggih, tapi paling berat
- **V20** → pilihan mobile-friendly yang paling seimbang

---

## Contoh Tuning Karakter

### Untuk sub yang lebih clean dan aman
- naikkan sedikit crossover bawah
- jangan terlalu besar di body shelf
- jaga subsonic tetap aktif
- gunakan auto headroom secukupnya

### Untuk ultra-low yang lebih terasa
- naikkan Ultra Low Enhancer sedikit
- jangan terlalu banyak body shelf
- hindari memperlebar crossover tanpa alasan

### Untuk mengurangi gemuruh
- turunkan sub-bass amount
- jangan terlalu agresif pada area 50–80 Hz
- pastikan phase align aktif

---

## Catatan Performa

Karena ini adalah DSP **real-time per sample**, beban perangkat sangat berpengaruh.

Hal yang bisa membuat audio tidak stabil:
- guard yang terlalu banyak
- analyzer yang terlalu kompleks
- buffer audio terlalu kecil
- convolver atau modul tambahan yang tidak perlu

Kalau perangkat terasa patah-patah:
- pilih versi yang lebih ringan
- matikan efek yang tidak wajib
- gunakan buffer yang lebih besar bila tersedia

---

## Instalasi

1. Install JamesDSP
2. Buka fitur **LiveProg**
3. Paste script AT-2XDSP yang ingin dipakai
4. Simpan dan aktifkan preset
5. Sesuaikan parameter sesuai sistem speaker

---

## Kebutuhan Sistem

Minimum yang disarankan:
- Android dengan JamesDSP
- CPU yang cukup stabil untuk audio realtime
- buffer audio menengah atau besar

Lebih nyaman jika:
- device tidak terlalu penuh aplikasi latar
- audio engine tidak dibebani proses tambahan
- charging dan audio berat tidak dilakukan bersamaan jika device mulai terasa berat

---

## FAQ

### Kenapa sub terasa besar tapi tetap tight?
Karena crossover, phase alignment, dan guard transien dijaga supaya sub tidak bocor ke jalur lain.

### Kenapa versi tertentu patah-patah?
Biasanya karena versi itu terlalu berat untuk device yang dipakai, bukan karena ide DSP-nya salah.

### Kenapa ada versi banyak?
Karena tiap device dan tiap kebutuhan suara berbeda. Ada versi yang aman, ada yang agresif, ada yang eksperimen.

### Kenapa ultra-low terasa lebih enak di lagu tertentu?
Karena isi rekaman berbeda. Tidak semua lagu punya energi 30–45 Hz yang sama.

---

## Kontribusi

Kalau mau mengembangkan repo ini, fokus yang paling berguna adalah:
- optimasi CPU
- perbaikan komentar parameter
- dokumentasi tuning yang lebih lengkap
- membuat versi khusus perangkat ringan
- menulis catatan perbedaan karakter antar versi

---

## Lisensi

Repo ini ditujukan untuk pembelajaran, eksperimen, dan tuning audio pribadi. Gunakan secara bertanggung jawab, terutama jika dipakai pada sistem speaker dan amplifier yang bertenaga besar.

---

## Penutup

AT-2XDSP dibuat untuk pengguna yang ingin suara bass yang **besar, jelas, dan terkontrol**.  
Bukan sekadar keras, tetapi punya bentuk, rasa, dan kontrol yang enak didengar lama.
