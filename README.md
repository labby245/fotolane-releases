# Fotoyu Resize — rilis

Repo ini **hanya berisi berkas rilis** aplikasi Fotoyu Resize. Source
code-nya ada di repo terpisah yang private.

Kenapa dipisah: fitur auto-update di dalam app mengambil manifest rilis
**tanpa autentikasi**, dan aset rilis GitHub mewarisi visibilitas repo-nya.
Menaruh rilis di repo private berarti app tidak bisa mengunduhnya sama
sekali; menyelipkan token ke dalam app bukan jalan keluar, karena app yang
dibagikan bisa dibongkar siapa saja.

## Unduhan

Ambil berkas untuk platformmu dari
[rilis terbaru](../../releases/latest):

| Berkas | Platform |
|---|---|
| `FotoyuResize-<versi>-arm64.apk` | Android (tablet/HP arm64) |
| `FotoyuResize-<versi>.dmg` | macOS |
| `FotoyuResize-Setup-<versi>.exe` | Windows |
| `latest.json` | dibaca app untuk mengecek update — bukan untuk diunduh manual |

## Verifikasi berkas

`latest.json` memuat sha256 tiap berkas. App memverifikasinya sendiri
sebelum menawarkan pemasangan; untuk memeriksa manual:

```bash
shasum -a 256 FotoyuResize-<versi>-arm64.apk    # macOS / Linux
certutil -hashfile FotoyuResize-Setup-<versi>.exe SHA256   # Windows
```
