# Smart Finance — APK Android

Aplikasi kewangan peribadi offline. GitHub akan membina fail APK secara automatik setiap kali kod dimuat naik.

## Kandungan

- `www/index.html` — aplikasi Smart Finance
- `assets/` — ikon dan skrin pembuka
- `capacitor.config.json` — nama dan ID aplikasi
- `.github/workflows/build-apk.yml` — arahan GitHub untuk membina APK

## Cara bina APK (kali pertama)

1. Log masuk ke github.com dan tekan **New repository**. Namakan `smart-finance`, pilih **Private**, kemudian tekan **Create repository**.
2. Dalam repo baharu, tekan **uploading an existing file**.
3. Ekstrak zip ini di komputer. Seret **semua isi folder** (bukan folder itu sendiri) ke halaman GitHub, kemudian tekan **Commit changes**.
   - Folder `.github` tersembunyi pada sesetengah komputer. Di Windows, buka View › Hidden items. Tanpa folder ini, APK tidak akan dibina.
4. Buka tab **Actions**. Proses "Bina APK Smart Finance" akan berjalan selama kira-kira 5–8 minit.
5. Apabila tanda hijau ✓ muncul, buka **Releases** di sebelah kanan halaman repo dan muat turun **SmartFinance.apk**.

Jika fail `.github` gagal dimuat naik melalui seret: tekan **Add file › Create new file**, taip nama `.github/workflows/build-apk.yml`, tampal isi fail itu, kemudian Commit.

## Pasang di telefon

1. Hantar `SmartFinance.apk` ke telefon (Google Drive, WhatsApp kepada diri sendiri, atau kabel USB).
2. Buka fail itu. Jika diminta, benarkan **Pasang aplikasi tidak diketahui** untuk aplikasi yang anda gunakan untuk membuka fail.
3. Jika Play Protect memberi amaran, tekan **Butiran lanjut › Pasang juga**. Amaran ini muncul kerana APK tidak datang dari Play Store.

## Kemas kini aplikasi

Gantikan `www/index.html` di GitHub (Add file › Upload files) dan Commit. APK baharu akan muncul di Releases. Pasang di atas versi lama dan data anda akan kekal.

## Penting tentang data

- Data disimpan dalam telefon sahaja. Jika aplikasi dinyahpasang atau data aplikasi dikosongkan, semua rekod akan hilang.
- Buat sandaran berkala melalui **Tetapan › Eksport sandaran › Salin**, kemudian simpan teks itu di tempat selamat.
- APK ini ialah versi debug untuk kegunaan sendiri. Untuk Play Store, APK perlu ditandatangani dengan kunci release.
