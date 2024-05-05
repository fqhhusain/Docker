# Docker
Buatlah container menggunakan base image nginx, serta definisikan port 5000 agar bisa diakses melalui localhost, dan jangan lupa untuk stop dan remove setelah berhasil

Instalasi Docker

Windows

1. Download Docker
2. Cek Versi
   ```
   docker --version
   ```
3. Periksa apakah docker sudah berjalan
   ```
   docker run hello-world
   ```

Buatlah Dockerfile dengan base Image adalah python:3.8 dan file index.py di dalam folder www dengan tulisan "Hello world". Atur direktori di /var/www/html serta definisikan port 5003. Setelah itu, cobalah akses pada port 5003
