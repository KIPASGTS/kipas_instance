# KIPAS native updates

Source dan build berada di KIPAS_CLIENT. Repo ini hanya menyimpan artefak rilis.

- Channel: `channels/ob55-arm64-v2.json`
- Library: `libuwr_redirect.so` (arm64-v8a)
- Manifest ditandatangani RSA-SHA256; public key ditanam ke APK.
- Library ada di `libraries/kipas_client/arm64/libuwr_redirect.so`.
- APK memeriksa commit terbaru, lalu mengambil manifest dan library dari commit yang sama.
- Checking update menunggu verifikasi selesai sebelum membuka instance; gagal menampilkan Retry.
- ARM32 belum tersedia karena target native proyek ini khusus ARM64.
- Build: `./build.sh`; library saja: `./build.sh --lib-only`.
- Private key dan source tidak diunggah ke repo ini.
