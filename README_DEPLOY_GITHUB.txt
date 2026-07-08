PANDUAN REDIRECT GITHUB PAGES KE APLIKASI CAPKIN

File yang perlu diupload ke repository GitHub Pages:
- index.html
- 404.html

Target redirect saat ini:
https://script.google.com/macros/s/AKfycbz6ePJuwZYaFZSkCDe_B_3CM59ogMELoJCed8oFX73WiPyoPq6DiVSl1sTNexgx1AAhPA/exec

LANGKAH DI GITHUB

1. Buka repository GitHub yang dipakai untuk alamat:
   https://mustoniku.github.io/capkin/

2. Upload/replace file index.html dari folder ini ke root repository atau ke folder yang dipakai GitHub Pages.

3. Upload/replace file 404.html dari folder ini di tempat yang sama.

4. Buka Settings > Pages.

5. Pastikan Source mengarah ke branch dan folder yang benar, biasanya:
   Branch: main
   Folder: /root

6. Tunggu 1-3 menit, lalu buka:
   https://mustoniku.github.io/capkin/

JIKA TARGET WEB APP BERUBAH

Buka index.html, ganti URL pada bagian:
const TARGET_URL = '...';

Ganti juga URL di meta refresh, canonical, dan tombol "Buka Aplikasi".

CATATAN

- Redirect ini memakai JavaScript dan meta refresh.
- Jangan membuka Apps Script di iframe GitHub Pages karena Web App Google sering memblokir iframe.
- Cara paling aman adalah redirect langsung seperti file ini.
