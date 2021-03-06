# Laporan Praktikum Pertemuan ke 6 tentang Docker

Deploying Your First Docker Container
1. Mencari docker image dengan nama redis pada docker hub, dengan perintah `docker search redis`.
![](img/1.png)
2. Kemudian menjalankan image redis tersebut, dengan perintah `docker run -d redis`, -d digunakan agar image redis berjalan pada background.
![](img/2.png)
3. Melihat container yang sudah running, dengan perintah `docker ps`.
![](img/3.png)
4. Untuk melihat detail dari suatu container seperti IP Address, digunakan perintah `docker inspect (nama dari container / id container)`.
![](img/4.png)
5. Untuk melihat log dari sebuah container yang running, digunakan perintah `docker logs (nama dari container / id container)`.
![](img/5.png)
6. Perintah di bawah ini digunakan untuk menjalankan image redis:latest pada background dengan nama redisHostPort yang dapat diakses menggunakan port 6379.
![](img/6.png)
7. Sama dengan nomer 6 hanya saja namanya adalah redisDynamic.
![](img/7.png)
8. Untuk melihat daftar mapping port, digunakan perintah `docker port (nama container) (port container)`.
![](img/8.png)
9. Ketikkan `docker ps`, dapat melihat list container yang jalan.
![](img/9.png)
10. Perintah di bawah ini, digunakan untuk menjalankan image yang disertai dengan persisten volume.
![](img/10.png)
11. Perintah di bawah ini digunakan untuk menjalankan container ubuntu dengan command ps.
![](img/11.png)
12. Perintah di bawah ini digunakan untuk masuk ke dalam container ubuntu.
![](img/12.png)

Create Nginx Static Web Server
1. Membuat Dockerfile, Dockerfile dibuat untuk membuat image. Di dalam Dockerfile ini, diawali dengan base image yang ditandai dengan `FROM`.
![](img/13.png)
2. Untuk membuat image dari Dockerfile menggunakan perintah `docker built -t (nama image) .`, -t digunakan untuk tag.
![](img/14.png)
3. Untuk melihat daftar image yang ada menggunakan printah `docker images`
![](img/15.png)
4. Menjalankan docker images agar menajadi container.
![](img/16.png)
5. Mengakses hasil dari container tersebut dengan perintah `curl`.
![](img/17.png)

Building Container images
1. Membuat Dockerfile dengan base image nginx:1.11-alpine
![](img/18.png)
2. Build image dengan nama my-nginx-latest:latest
![](img/19.png)
3. Menjalankan image
![](img/20.png)
4. Mengakses docker
![](img/21.png)
5. Melihat daftar container yang jalan.
![](img/22.png)
