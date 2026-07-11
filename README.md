# ytconvextension

Chrome extension sederhana untuk export cookies YouTube menjadi file `cookies.txt` format Netscape yang bisa dipakai oleh `yt-dlp` dan `pytube`.

## Fitur

- Mengambil cookies YouTube dan Google dari browser yang sedang login.
- Menyimpan hasil export dengan nama `cookies.txt`.
- Format output kompatibel dengan `yt-dlp --cookies cookies.txt` dan penggunaan cookie file di `pytube`.
- Tampilan popup rapi, ringan, dan fokus pada satu fungsi.

## Cara install manual

1. Buka `chrome://extensions`.
2. Aktifkan **Developer mode**.
3. Klik **Load unpacked**.
4. Pilih folder repository ini.
5. Login ke YouTube di browser yang sama.
6. Klik icon extension, lalu pilih **Download cookies.txt**.

## Contoh pemakaian

```bash
yt-dlp --cookies cookies.txt "https://www.youtube.com/watch?v=VIDEO_ID"
```

Untuk `pytube`, berikan file `cookies.txt` ke workflow downloader yang mendukung cookie file.
