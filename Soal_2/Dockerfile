# Menggunakan python:3.8 sebagai base image
FROM python:3.8

# Membuat direktori /var/www/html di dalam image
WORKDIR /var/www/html

# Menyalin file index.py ke dalam folder www di dalam image
COPY www/index.py ./www/

# Menginstal Flask
RUN pip install flask

# Membuka port 5003
EXPOSE 5003

# Menjalankan file index.py saat container dijalankan
CMD ["python", "./www/index.py"]
