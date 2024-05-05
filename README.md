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
4. Buat container nginx
   ```
   docker images
   docker pull nginx:latest
   docker ps
   docker ps -a
   docker run -p 5000:80 nginx
   ```
5. cek pada host 
   http://localhost:5000/
6. Remove container
   ```
   docker rm [container id]
   ```

Buatlah Dockerfile dengan base Image adalah python:3.8 dan file index.py di dalam folder www dengan tulisan "Hello world". Atur direktori di /var/www/html serta definisikan port 5003. Setelah itu, cobalah akses pada port 5003
```
sudo mkdir /var/www
sudo mkdir /var/www/html
cd /var
sudo nano Dockerfile
cd www
sudo nano index.py
```
Build di directory /var
```
docker build -t my-python-app .
docker run -p 5003:5003 my-python-app
```
localhost:5003
