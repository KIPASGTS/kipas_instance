# KIPAS native updates

Source dan build berada di KIPAS_CLIENT. Repo ini hanya menyimpan artefak rilis.

- Channel: `channels/ob55-arm64-v1.json`
- Library: `libuwr_redirect.so` (arm64-v8a)
- Manifest ditandatangani RSA-SHA256; public key ditanam ke APK.
- Library disimpan berdasarkan SHA-256 dan diverifikasi sebelum dimuat.
- Build: `./build.sh`; library saja: `./build.sh --lib-only`.
- Private key dan source tidak diunggah ke repo ini.
