# tugas-individu-grafkom-a-helsasp

### Nama : Helsa Sriprameswari Putri <br>
### NRP : 5025221154 <br>
### Kelas : Grafika Komputer A <br>

## Tugas Individu 1 - Membuat Program Sederhana dengan WebGL

Program sederhana yang saya buat adalah sebuah rumah dengan menggunakan dua bentuk yaitu segitiga sebagai atapnya dan segiempat sebagai body rumah dengan latar belakang biru.

Terdapat 3 Source Code yaitu : 

1. index.html : struktur dasar halaman web yang menggunakan WebGL untuk merender grafik.  Di dalam bagian <head>, terdapat tag <title> untuk memberikan judul pada halaman dan tag <link> untuk menyertakan file CSS yang berfungsi untuk styling. Pada bagian <body>, terdapat elemen <canvas> dengan id webgl-canvas yang akan digunakan oleh WebGL untuk menggambar grafik. Tag <script> menyertakan file JavaScript eksternal yang mengandung kode untuk merender grafik menggunakan WebGL.
2. style.css : mengatur elemen body dan html agar tidak memiliki margin atau padding, serta mengatur overflow sehingga tidak ada scrollbar yang muncul.
3. script.js : terdapat fungsi main()  untuk menginisialisasi WebGL dan merender sebuah gambar rumah sederhana pada kanvas HTML. Fungsi ini mulai dengan mendapatkan konteks WebGL dari elemen kanvas. Selanjutnya, dua shader (vertex dan fragment) didefinisikan dalam bentuk sumber kode GLSL, dan fungsi createShader dan createProgram digunakan untuk mengkompilasi dan menghubungkan shader-shader tersebut ke dalam program WebGL. Posisi dan warna vertiks untuk atap (segitiga) dan badan rumah (persegi panjang) ditentukan dalam buffer dan diikat ke atribut shader yang sesuai.

### Hasil Program 
![Screenshot 2024-08-30 204742](https://github.com/user-attachments/assets/5a2d81c0-0c0a-471d-b7ad-fe561cce8d93)


## Tugas Individu 2 - Implementasi 2D Translation, Rotation, Scales, Matrices dalam WebGL

Implementasi program yang saya buat adalah letter 'H' yang memiliki beberapa fungsi, yaitu X translation, Y translation, angle rotation, scale X dan scale Y.

Penjelasan kode :

1. index.html : menampilkan huruf "H" di elemen kanvas dengan menggunakan vertex dan fragment shader. User dapat menggunakan sebuah slider untuk menggunakan fungsi translasi, rotasi, dan scale pada sumbu X dan Y.
2. style.css : mengatur tampilan beberapa elemen HTML.Body tanpa margin dan canvas diperluas (full screen). #uiContainer ditempatkan  di sudut kiri atas. Elemen slider memiliki lebar tetap dan margin di sekelilingnya.
3. script.js : implementasi dari WebGL yang menggambar bentuk-bentuk 2D dengan memanfaatkan shader dan matriks transformasi untuk melakukan x y translation, angle rotation, dan x y scale. Elemen canvas pada HTML digunakan untuk menampilkan gambar, sementara WebGL digunakan untuk rendering grafis 2D.

## Hasil Program
![Screenshot 2024-09-06 210918](https://github.com/user-attachments/assets/3bac93b4-c971-4f60-8e6a-ff44ed0c3593)



## Tugas Individu 3 - 3D WebGl

## Membuat Objek 3D Geometry

### 1. Cube


Membuat bentuk cube 3D dengan warna yang berbeda - beda di tiap sisinya. Cube tersebut terdiri dari enam sisi yang diberi warna berbeda: sisi depan ungu, belakang hitam, atas merah, bawah kuning, kiri biru, dan kanan pink. Kubus berotasi secara dinamis di sumbu X, Y, dan Z. Script untuk menginisialisasi konteks WebGL, mendefinisikan geometri dan warna kubus, serta mengatur shader untuk rendering.

https://github.com/user-attachments/assets/ae4e640a-47ab-42c6-b7dc-941a1071b022
![image](https://github.com/user-attachments/assets/b0403857-d16b-4b78-8a08-c0953f01d1ac) <br>

### 2. Cone 

Membuat bentuk cone 3D dengan warna rainbow. Cone dibentuk menggunakan vertices sebagai titik-titik yang mendefinisikan posisi kerucut, termasuk pusat dasar dan titik puncak. Cone juga berotasi di sumbu xyz agar lebih menarik.

https://github.com/user-attachments/assets/f9c87fcc-e883-4aea-97eb-cea2bf819d2c
![image](https://github.com/user-attachments/assets/3574ebc0-e7f7-4e8b-8618-3549c568f3f0)



### 3. Cylinder

Membuat bentuk cylinder berwarna merah-kuning yang didefinisikan oleh radius, tinggi, dan jumlah segmen, dan melingkar. Silinder dianimasikan untuk berputar terus-menerus di sekitar sumbunya agar interaktif.

https://github.com/user-attachments/assets/15afa175-3281-487a-8547-cd05dde966f7
![image](https://github.com/user-attachments/assets/b5f845b5-8f21-4292-a246-25cafec59827)


### 4. Ball

Membuat bentuk bola / sphere 3D yang dirender menggunakan WebGL. Bola dibuat dengan radius dan dibagi menjadi grid lintang dan bujur untuk menghasilkan vertex dan warna.Bola berotasi di sumbu X Y Z. Vertex dan fragment shader menangani proses rendering, menerapkan warna gradien pada permukaan bola.

https://github.com/user-attachments/assets/650ae02e-4013-456a-85b7-00e4942a900d
![image](https://github.com/user-attachments/assets/61abaa7a-690a-4252-bcd8-eea4fd1a2d82)



### 5. Ring

Membuat ring 3D dengan menggunakan shader untuk mengatur canvas untuk rendering, menghitung posisi dan warna vertice ring, dan rotasi ring di sekitar sumbu X, Y, dan Z. Warna ring dibuat menyerupai glazed donut.

https://github.com/user-attachments/assets/d3f1d58f-51ab-4606-856b-41e299e8236f
![image](https://github.com/user-attachments/assets/2df16fd9-2626-4040-8d76-f2f93aa623d3)



## Membuat 3D Lathe 

Membuat lathe berbentuk air mancur. Dalam program terdapat beberapa fungsi. Fungsi distance untuk menerapkan jarak pada bidang. Fungsi divisions untuk menentukan seberapa halus permukaan objek 3D yang dihasilkan serta transformasi dari bentuk awal ke bentuk whole hingga bentuk lathe penuh. Serta fungsi start,end,max angle yang memungkinkan untuk rotasi lathe di sudut tertentu. Fungsi capstart dan capend juga ditambahkan untuk mengatur bentuk ujung air mancur. Terdapat fungsi triangle untuk melihat bidang air mancur berupa kerangka/garis. User juga dapat switch mode antara normal,lit,texcoords.

https://github.com/user-attachments/assets/8eb9db0b-6c94-4235-badb-a3c7e21856e2


## Applying Texture 3D

 Mengimplementasikan rendering 3D sederhana menggunakan WebGL untuk menggambar kubus dengan tekstur berupa sebuah foto dengan efek rotasi pada sumbu x y z. Program dibuat dengan menginisialisasi canvas dan konteks WebGL. Fungsi ini membuat program shader dari skrip yang ditentukan. Selain itu juga menetapkan lokasi atribut untuk posisi dan tekstur, serta matriks transformasi. Textures diambil dari URL image dan ditambahkan ke buffer setelah berhasil dimuat.
 

 ## Applying Lighting 3D

 Mengimplementasikan lighting pada cube 3D dengan webgl. Cube 3D berwarna hitam saat belum kena lighting. Lighting yang digunakan terdapat tiga warna yaitu merah, biru, dan ungu. Lighting ini mempunyai fungsi translasi sumbu x dan sumbu y yang memungkinkan lighting bergerak dari kiri ke kanan maupun atas bawa mengenai cube. Terdapat fungsi limit untuk mengatur besar kecil lighting yang mengenai cube.

 ## Animation (Rotation, Scale, Translation XYZ) 

 Mengimplementasikan animasi pada cube 3D dengan rendering webgl. Cube 3D yang dibuat memiliki warna berbeda di sisi-sisinya. Terdapat fungsi translasi X yang memungkinkan cube bergerak kiri-kanan, translasi Y yang memungkinkan kubus bergerak atas-bawah, dan translasi Z yang memungkinkan kubus bergerak sumbu z. Terdapat fungsi rotasi X,Y,Z yang membuat cube dapat berputar di sumbu X Y Z. Fungsi satu lagi adalah scalling untuk adjust ukuran kubus pada sumbu X Y Z.

## Ortographic & Perspective Camera

Menerapkan camera untuk melihat beberapa kubus yang ada. Camera dapat berfungsi untuk geser ke bagian kiri dan kanan (keyboard L untuk kiri dan R untuk kanan), bergerak maju mundur (keyboard F untuk maju dan B untuk mundur), roll ke samping kiri dan kanan (keyboard Y untuk roll kiri dan X untuk roll kanan), serta melihat dari POV atas bawah (arrow up and down). 

## Demo 3D



