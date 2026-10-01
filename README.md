# MILKI LAUNCHER — Mirror Data Client SA-MP (Android)

Mirror resmi **data client SA-MP** untuk aplikasi Android **MILKI LAUNCHER**.
Data ini diunduh otomatis oleh launcher saat pemain pertama kali masuk server
(fonts, file `SAMP/`, `texdb/samp.*`, `texdb/samp.img`).

## Mengapa repo ini ada?

Sebagai **jalur unduhan mandiri**: launcher tidak bergantung pada satu domain
pihak ketiga. Jika sumber utama tidak tersedia, launcher tetap dapat mengunduh
data dari repo ini — sehingga pemain selalu bisa main.

## Isi

| | |
|---|---|
| `samp_list.json` | Daftar 32 berkas + ukuran + URL unduh (format launcher) |
| `data/` | 32 berkas data client SA-MP (±167 MB, sebagian via Git LFS) |

## Cara kerja di launcher

Backend MILKI LAUNCHER membaca `samp_list.json` dari repo ini
(`raw.githubusercontent.com/pixellabbo-spec/milki-launcher-data/main/samp_list.json`)
dan mengirimkannya ke aplikasi sebagai `samp_list_url`. Aplikasi mengunduh
setiap berkas dari URL `raw.githubusercontent.com` di repo ini.

## Pembaruan data

1. Timpa/ubah berkas di `data/`.
2. Jalankan ulang generator `samp_list.json` (ukuran dihitung dari berkas aktual).
3. Commit & push.

---
© MILKI1557 — MILKI LAUNCHER
