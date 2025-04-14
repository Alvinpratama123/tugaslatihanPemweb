# analisi docker  
docker di gunakan untuk penyimpanan atau terminal dengan kapasitas penyimpanan yang sangat besar di dalam docker ada nama server nginx dan port yang kita buat dan ada database nya juga sudah tersedia di docker 
5w1h 
saya menggunakan docker karna dia bisa meyimpan webserver dan data bases dalam 1 terminal
apa aja yang terlibat ada wsl utuk mengakses web server ke dalam docker 
apa aja yang terjadi sering terjadi eror akibat jaringan 
cara mengatasi nya ya itu kita siapa kan internet yang sangat besar 
dan akses 

kelebihan docker 
Startup container hanya dalam hitungan detik
Aplikasi yang dikemas dalam container Docker bisa dijalankan di Windows, macOS, atau Linux tanpa perlu konfigurasi ulang 
kekurangan dari docker 
memakan memory atau ram terlalu besar 
harus berjalan di linux jiga ingin maksimal

# analisis wsl
wsl atau windos system for linux ini adalah alat untuk mengubungkan suatu sofware ke sofware lain nya melalu terminal ubuntu ini juga sering di gunakan untuk melihat folder buat folder atau hapus folder juga bisa juga build docker antara docker dan vscode 

kelebihan
Cocok untuk Developer & DevOps
Bisa jalankan Docker, Git, Node.js, Python, PostgreSQL, MySQL, dll. seperti di Linux asli.
WSL gratis dan langsung didukung Microsoft.
kekurangan nya
membutuhkan akses internet yang cukup besar seperti build docker dengan performa internet lebah sering terjadi valid

# analisis navicat 
navicat bisa di gunakan untuk membuat relasi atau membuat database dan membuat user dan membuat password dan membuat table dan membuat index dan membuat view dan membuat trigger cara meyambukan nya kita bisa bikin folder laravel filament lalu kita masukan api nya dan port nya  dan untuk mengubungkan database ke database lain nya

kelebihan navicat
Bisa bikin query tanpa harus coding manual
menghubungkan api ke vscode mudah dan mudah di pahami 
Mempermudah migrasi database dari satu server ke server lain.

kekurangan nya adalah 
navicat sofware berbayar dan cukup sulit untuk mencari crak dari navicat
Di beberapa kasus, Navicat bisa terasa lambat, terutama saat membuka banyak koneksi database sekaligus.

# analisis pembuatan web
bikin folder melalu wsl buat folder mkdir pemweb cd pemweb mkdir pert1 cd pert1 buat lagi mkdir koding lalu cd koding buat docker compose yml env lalu build untuk menghubung docker 
lau bikin nginx.conf untuk membaca webserver dan melacak atau mengetahui file html ada di mana

buat src bikin index html lalu coba jika berhasil buka docker ceke name server atau containel masuk ke dalam di bawah name containel ada port 80 80 klik akan menuju browser dengan lockalhost lalu bikin file baru  nama nya div.html lalu buat paragraf untuk menjalankan nya bukan browser localhos/div.html ini fungsi dari nginx untuk membara location src

kelebihan pembuatan web
koding mudah di pahamin dan akses ke browser mudah di akses 
apa lagi kalo kita menggunakan tool yang efektif bisa jauh lebih efisien

kekurangan 
kadang akses atau koding banyak taypo hingga akses di localhos eror


# analisis extensen 
1.auto closs tag fungsi nya untuk menutup coding atau css
2.auto rename tag fungsi nya untuk mengganti koding atau mengubah nya 
3.auto complaite tag untuk melengkapi koding html atau css yang kurang atau lupa

kelebihan dari auto closs tag
tidak perlu menutup tag secara manual akan ada di perbaikan 
kekurangan 
Terkadang, saat mengetik tag baru lalu menghapusnya, tag penutup tetap tertinggal, sehingga kode jadi berantakan.
kelebihan auto rename tag
tidak perlu edit atau nutup tag secara manual
kekurangan
 Jika ada banyak elemen dengan tag yang sama, Auto Rename Tag bisa mengubah lebih dari yang diinginkan.


# analisis vscode sitem
menggunakan vscode sistem agar gambang untuk mengakses melalui linux
kelebihan
Bisa menambahkan berbagai plugin/extension untuk mendukung bahasa atau framework tertentu
kekurangan
 Jika terlalu banyak extension yang aktif, VS Code bisa menggunakan RAM cukup besar, terutama di PC/laptop dengan RAM 4GB ke bawah.

# analisis html dasar
1.div untuk mebuat lembar text baru pada html
2.img untuk mebuat gambar baru pada html
3.a untuk membuat link baru pada html
4.p untuk membuat paragraf baru pada html
5.h1 untuk membuat judul baru pada html
6.ul untuk membuat urutan pada html
kelebihan
gratis Tidak perlu lisensi atau membayar untuk menggunakan HTML.
kekurangan
Tidak bisa membuat animasi, efek hover, atau tombol interaktif tanpa bantuan JavaScript atau CSS.

# alalisis akses folder latihan pada server nginx
membuat folder di luar src dan nama naya latihan di dalam nya kita isi dengan 
nama file home.html 
nama profile.html

nah kita perlu akses atau beri location yang mau di akses di docker dan di nginx
di docker di tambahkan ini  - ./latihan:/usr/share/nginx/latihan
di nginx di tambah kan ini    location /latihan {
        alias /usr/share/nginx/latihan/;
        index index.html index.htm home.html;
        try_files $uri $uri.html $uri/ =404;
    }

    kelebihan 
    server di luar scr bisa di panggil menggunaka nginx dan tidak menumpuk di dalam src
    kekurang nya
    kadang lockasi tidak terdeteksi atau pun banyak kesalah dalam pemanggilan seperti menaru koding di tempat yang berbeda