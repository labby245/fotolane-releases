<div align="center">

<img src="img/icon.png" width="96" alt="Fotolane">

# Fotolane

**Penyiap foto acara otomatis** — oleh Labstory Studio

Ribuan foto acara siap unggah tanpa perlu ditunggui.

Android · macOS · Windows

[Instagram @labstory.studio](https://www.instagram.com/labstory.studio/)

</div>

---

Foto langsung dari kamera ukurannya puluhan MB — terlalu besar untuk diunggah,
dan harus dipecah per 2000 foto per folder. Mengerjakannya manual setelah acara
bisa memakan berjam-jam.

Fotolane mengerjakan itu sendiri: **1000 foto diperkecil dalam sekitar 41
detik** (±41 ms per foto, diukur di Mac Apple Silicon; di HP dan laptop
Windows lebih lambat, tergantung perangkatnya).

Foto aslimu **tidak pernah diubah atau dihapus**: hasilnya selalu ditulis ke
folder baru di sampingnya. Satu-satunya pengecualian adalah opsi Kamera USB
"Simpan foto asli" kalau kamu matikan sendiri (lihat di bawah).

---

## 1. Auto Resize — jalan sendiri selama acara

<img src="img/auto-resize.png" width="620" alt="Tab Auto Resize">

Pilih folder, tekan **Mulai mengawasi**, lalu biarkan. Setiap foto baru yang masuk
langsung diperkecil dan dipisah ke folder `ganjil` dan `genap`.

- Bisa mengawasi **folder tanggal hari ini** di dalam folder pilihanmu, atau
  **langsung folder itu sendiri**.
- Setelah **2000 foto**, folder lanjutan dibuat otomatis: `ganjil-2`,
  `ganjil-3`, dan seterusnya.
- Hanya foto yang **masuk setelah tombol Mulai ditekan** yang diproses. Foto
  lama yang sudah ada di folder itu dilewati.
- Foto yang masih separuh tersalin dari kamera **ditunggu sampai selesai**,
  jadi tidak ada hasil yang rusak setengah jadi.
- **Layar boleh dimatikan** — prosesnya tetap jalan.

### Kamera USB — langsung dari kamera

Pilih sumber **Kamera USB**, colok kamera dengan kabel, tekan **Mulai mengawasi**, lalu
memotret seperti biasa. Setiap jepretan langsung masuk lewat kabel, diperkecil,
dan dipisah ke `ganjil` / `genap`.

- Foto asli disimpan di folder `Foto Asli`; hasilnya di folder tanggal hari
  ini, yang berganti sendiri lewat tengah malam.
- Nama file mengikuti nomor kamera, dan kartu memori tetap menyimpan salinan
  (kalau kamera menyimpan ke kartu).
- Hanya JPEG yang diambil; RAW tetap di kartu. Sony lewat PC Remote: atur
  "RAW+J PC Save Image" ke JPEG saja (kalau ada di menunya), kalau tidak
  RAW ikut terkirim lewat kabel lalu dibuang.
- Kabel tercabut? Fotolane menyambung lagi sendiri, dan foto yang dijepret
  selagi kabel lepas ikut diambil dari kartu. Ini sudah dicoba dengan kamera
  asli untuk LUMIX dan Canon; Nikon memakai cara yang sama tapi belum diuji.
  Fujifilm, dan Sony kecuali beberapa model baru di macOS, tidak mengambil
  foto yang dijepret selagi kabel lepas: foto itu hanya ada di kartu kalau
  kamera menyimpan ke kartu.
- Opsi **Simpan foto asli di perangkat ini**: matikan bila yang ingin
  disimpan hanya hasilnya (di `ganjil` / `genap`). Foto asli dihapus hanya
  kalau hasilnya sudah ada **dan** kamera menyimpan salinannya ke kartu.
  Foto tanpa kartu (PC000001…) dan foto yang gagal diolah tidak pernah
  dihapus.
- **macOS:** LUMIX, Canon, Nikon, Sony, Fujifilm (Sony lama seperti a7 III,
  a9, a6000–a6600 lewat mode PC Remote).
  **Windows:** LUMIX, Canon, Nikon, Sony (mode PC Remote), Fujifilm.
  Fotolane tidak memasang driver apa pun.
  **Android:** LUMIX, Canon, Nikon, Sony (mode PC Remote), dengan kabel USB-C
  pendek (maksimal 1 m).
- Fujifilm hanya untuk model yang didukung SDK Fujifilm: X-H2, X-H2S, X-T5, X-T4, X-T3, X-S20, X-S10, X-M5, X-Pro3, dan GFX (100 II, 100S II, 100S, 100, 100RF, 50S II, 50S, 50R, ETERNA 55). Model lain
  (mis. seri X100, X-E, X-T30) tidak ada di daftar SDK, jadi belum didukung.
- Merek lain (OM System / Olympus, Pentax / Ricoh, Leica, Sigma) belum bisa
  lewat kabel. Pakai Auto Resize dengan folder kartu memori.
- Model yang sudah diuji dengan kamera asli: lihat daftar di bawah.
- Tekan **Berhenti** sebelum mencabut kabel.

### Kamera yang sudah diuji

| Merek | Model | macOS | Windows | Android |
|---|---|:---:|:---:|:---:|
| LUMIX | S5IIX (DC-S5M2X) | ✅ | ✅ | ✅ |
| Canon | EOS R50 V | ✅ | ✅ | ✅ |
| Nikon | belum diuji dengan kamera asli | | | |
| Sony | belum diuji dengan kamera asli | | | |
| Fujifilm | belum diuji dengan kamera asli | | | belum didukung |

Kameramu belum ada di daftar? Model LUMIX, Canon, dan Nikon lain kemungkinan
besar jalan karena satu merek memakai protokol yang sama, tapi belum
dijamin. Sony dan Fujifilm bergantung pada daftar model SDK pabrikannya (lihat
di atas). **Coba dulu selama masa coba (500 foto)** sebelum membeli. Setelah kameramu tersambung, tekan
**Kamera ini lancar? Kabari kami** di bawah status Auto Resize, dan kameramu
kami tambahkan ke daftar ini. Kalau tidak mau tersambung, tekan **Kamera
tidak tersambung? Kabari kami**.

## 2. Foto — proses sekaligus

<img src="img/foto.png" width="620" alt="Tab Foto">

Untuk foto yang sudah terkumpul. Pilih satu file atau satu folder, tekan
**Proses foto**, selesai. Pemisahan ganjil/genap juga tersedia di sini.

Setelah selesai, ringkasan menunjukkan berapa foto yang berhasil dan berapa
ruang yang dihemat. Kalau ada file yang gagal (misalnya rusak), cukup tekan
**Coba lagi** — hanya file itu yang diproses ulang.

## 3. Video

<img src="img/video.png" width="620" alt="Tab Video">

- **Potong & perkecil** — ambil beberapa detik pertama, dijamin di bawah batas
  ukuran (bawaan: 3 detik, 720p, di bawah 15 MB).
- **Ubah ke MP4** — video utuh, kualitas asli dipertahankan, di bawah 85 MB.

## Hal kecil yang memudahkan

- **Seret & lepas** file atau folder langsung ke jendela app (Mac & Windows).
- **Notifikasi saat selesai**, lengkap dengan suara — bisa dimatikan di
  Pengaturan.
- **Mode gelap** dan pilihan **bahasa Indonesia / English**, langsung dari
  bagian atas layar.

---

## Struktur folder hasil

Dengan **Auto Resize**, hasil ditulis di dalam folder sumbernya:

```
Folder Acara/
└── 2026-09-23/              ← folder tanggal (dipilih otomatis)
    ├── DSC_0011.jpg         ← foto asli, tidak disentuh
    ├── DSC_0012.jpg
    ├── ganjil/              ← maks 2000 foto
    │   ├── DSC_0011.jpg
    │   └── DSC_0013.jpg
    ├── ganjil-2/            ← dibuat otomatis saat "ganjil" penuh
    └── genap/
        ├── DSC_0012.jpg
        └── DSC_0014.jpg
```

Dengan tab **Foto**, hasil masuk ke folder `resize/` di samping foto sumber:

```
Folder Foto/
├── DSC_0011.jpg
└── resize/
    ├── ganjil/
    └── genap/
```

Ganjil atau genap ditentukan dari **angka terakhir pada nama file**, bukan dari
urutan. Jadi hasilnya tidak berubah walau isi folder bertambah.

---

## Unduh

Ambil versi terbaru di **[halaman Releases](../../releases/latest)**, lalu
pilih satu berkas sesuai perangkatmu:

| Perangkat | Berkas yang diunduh | Syarat |
|---|---|---|
| HP / tablet **Android** | `Fotolane-…-arm64.apk` | Android 7.0 ke atas, 64-bit |
| **Mac** | `Fotolane-….dmg` | macOS 12 ke atas, **Apple Silicon** (M1 atau lebih baru) |
| **Windows** | `Fotolane-Setup-….exe` | Windows 10 / 11, 64-bit (prosesor Intel / AMD) |

### Persyaratan

Cek dulu sebelum membeli; masa coba 500 foto bisa dipakai untuk memastikan
semuanya jalan di perangkatmu.

- **Mac Intel belum didukung.** Kompresi foto/video dan kamera USB di
  Fotolane untuk Mac saat ini hanya jalan di Mac Apple Silicon (M1, M2, M3,
  M4, dan seterusnya). Cek di menu Apple → *About This Mac*: tertulis
  "Chip Apple M…", bukan "Processor Intel".
- **Prosesor & RAM (laptop / PC):** disarankan 4 core dan RAM 8 GB.
  Laptop 2 core (mis. Intel Celeron / Pentium, AMD Athlon) tetap bisa
  dipakai tapi lebih lambat; Fotolane otomatis memproses lebih sedikit foto
  sekaligus di laptop seperti itu.
- **Ruang penyimpanan:** sekitar 1 GB untuk app, ditambah ruang untuk foto.
  Foto asli ikut disimpan kecuali opsi *Simpan foto asli di perangkat ini*
  dimatikan (hasil kompresi hanya ±2% dari ukuran aslinya).
- **Android:** Android 7.0 ke atas, 64-bit (hampir semua HP / tablet sejak
  2017). Untuk kamera USB, perangkat harus mendukung USB OTG; pakai kabel
  USB-C data, maksimal 1 m.
- **Kamera USB:** pakai kabel data (bukan kabel khusus mengisi daya), matikan
  Wi-Fi kamera, dan cek [daftar kamera yang sudah diuji](#kamera-yang-sudah-diuji).

### Catatan pemasangan

**Android** — karena tidak lewat Play Store, Android akan bertanya sekali soal
"instal dari sumber ini"; izinkan. Saat pertama dipakai, app meminta izin
**"Akses semua file"**. Izin itu dipakai untuk membaca folder fotomu dan
menulis folder hasil di sebelahnya — tanpa itu app tidak bisa menyimpan hasil
di tempat yang kamu pilih. App tidak mengirim apa pun ke mana pun.

**Mac** — kalau muncul peringatan bahwa app tidak bisa dibuka, klik kanan ikon
app lalu pilih **Buka**.

**Windows** — kalau muncul layar biru SmartScreen, klik **Info selengkapnya →
Tetap jalankan**.

---

## Harga

| | |
|---|---|
| Tab **Foto** & **Video** | Gratis selamanya |
| **Auto Resize** | Gratis untuk **500 foto pertama** |
| Lisensi penuh | **Rp 400.000, sekali bayar**, untuk **2 perangkat** (mis. laptop + HP/tablet), termasuk **update 1 tahun** |
| Perpanjangan update | **Rp 150.000 per tahun**, opsional. Tanpa perpanjangan, versi yang sudah kamu punya tetap jalan selamanya |

Pakai kamera USB? Coba dulu dengan kameramu selama masa coba sebelum membeli
(lihat [kamera yang sudah diuji](#kamera-yang-sudah-diuji)).

Cara membeli:

1. Tekan **Aktifkan** di bagian atas layar, lalu **Buka halaman beli**.
   Halaman [apps.labstory.id/produk/fotolane](https://apps.labstory.id/produk/fotolane)
   terbuka dengan kode perangkatmu sudah terisi.
2. Bayar dengan **QRIS** di halaman itu.
3. Setelah pembayaran dikonfirmasi, kunci tampil di halaman pembayaran dan
   dikirim ke email-mu.
4. Tempel kunci (atau seluruh isi email kuitansi) di jendela **Aktifkan**,
   lalu tekan **Aktifkan** — selesai.

**Perangkat kedua** gratis: daftarkan kode perangkatnya di halaman
pembayaranmu (tautannya ada di email kuitansi), lalu tempel kunci yang
muncul di perangkat itu. Jangan membeli lagi.

Ada pertanyaan sebelum membeli? Kirim email ke **hello@labstory.id**.

Lisensi berlaku untuk semua versi yang rilis sampai setahun sesudah kamu
membeli. Sebelum menawarkan update ke versi di luar masa itu, app memberi
tahu dulu. Perpanjang dari **Pengaturan → Perpanjang update**: halaman
[perpanjangan di apps.labstory.id](https://apps.labstory.id/produk/fotolane/perpanjang)
terbuka dengan kuncimu sudah terisi. Tempel juga kunci perangkat keduamu
supaya satu pembayaran memperpanjang keduanya. Lisensi yang dibeli sebelum
13 Oktober 2026 tetap mendapat semua update.

---

## Update otomatis

Cukup pasang sekali. App memeriksa sendiri apakah ada versi baru, lalu
menawarkannya lewat kotak di tengah layar — tinggal klik Unduh. Tidak perlu
kembali ke halaman ini lagi.

---

## Pertanyaan yang sering muncul

**Foto asli saya aman?**
Aman. App hanya membaca foto asli dan menulis hasilnya ke folder baru. Tidak
ada yang ditimpa atau dihapus.

**Seberapa kecil hasilnya?**
Bawaannya sisi terpanjang 1441 piksel dengan kualitas 92 — foto kamera biasanya
jadi beberapa ratus KB. Angka ini bisa diubah di **Pengaturan**.

**Ada foto yang ukurannya tidak berubah, kenapa?**
Berarti foto itu sudah lebih kecil dari batas. App tidak pernah memperbesar
foto, dan meng-encode ulang justru bisa membuat berkasnya lebih besar — jadi
foto seperti itu disalin apa adanya.

**Format apa saja yang didukung?**
JPG, JPEG, PNG, WebP, BMP, dan TIFF. **HEIC belum didukung** — kalau kameramu
atau iPhone menyimpan dalam HEIC, ubah dulu setelannya ke JPEG.

**Metadata foto ikut hilang?**
Tidak. Informasi kamera dan orientasi foto tetap terjaga.

**Perlu internet?**
Tidak. Semua diproses di perangkatmu sendiri. Internet hanya dipakai saat
memeriksa pembaruan.

**Auto Resize boros baterai?**
Selama mengawasi, app menjaga prosesor tetap aktif supaya tidak berhenti saat
layar mati — perkiraan beberapa persen baterai per hari. Yang jauh lebih boros
adalah layar yang dibiarkan menyala, jadi pilihan itu sengaja dimatikan secara
bawaan.

---

<div align="center">

Dibuat oleh **Labstory Studio Semarang**

[Instagram @labstory.studio](https://www.instagram.com/labstory.studio/)

<sub>Aplikasi ini dibuat mandiri oleh sesama fotografer dan tidak berafiliasi
dengan, atau didukung secara resmi oleh, platform mana pun.</sub>

</div>
