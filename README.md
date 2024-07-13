# Penjelasan codingan

cv2 adalah library OpenCV yang digunakan untuk pemrosesan gambar.

matplotlib.pyplot adalah modul dari Matplotlib yang digunakan untuk membuat grafik dan visualisasi.

cv2.imread() digunakan untuk membaca gambar dari file. Gambar yang dibaca akan disimpan dalam variabel image.

fotoo.JPEG adalah nama file gambar yang akan dibaca. Pastikan file ini berada di direktori yang sama dengan script atau berikan path lengkapnya.

cv2.cvtColor() digunakan untuk mengubah ruang warna gambar.

OpenCV membaca gambar dalam format BGR (Blue, Green, Red), sementara Matplotlib menampilkan gambar dalam format RGB (Red, Green, Blue). Oleh karena itu, gambar perlu diubah dari BGR ke RGB.

plt.imshow() digunakan untuk menampilkan gambar.

plt.axis('off') digunakan untuk menghilangkan sumbu (x dan y) pada plot.

plt.title('Original Image') menambahkan judul pada plot.

cv2.imread() digunakan untuk membaca gambar dari file. Gambar yang dibaca akan disimpan dalam variabel image.

fotoo.JPEG adalah nama file gambar yang akan dibaca. Pastikan file ini berada di direktori yang sama dengan script atau berikan path lengkapnya.

cv2.IMREAD_GRAYSCALE adalah flag yang digunakan untuk membaca gambar dalam mode grayscale (hitam putih).

cv2.Canny() digunakan untuk menerapkan algoritma Canny edge detection pada gambar. Hasilnya disimpan dalam variabel edges.

Parameter pertama adalah gambar yang akan diproses.

Parameter kedua dan ketiga adalah nilai threshold untuk algoritma Canny. 100 adalah threshold rendah dan 200 adalah threshold tinggi.

plt.figure(figsize=(10, 5)) digunakan untuk membuat sebuah figure baru dengan ukuran 10x5 inci.

plt.subplot(1, 2, 1) digunakan untuk membuat subplot pertama dari dua subplot yang ada dalam satu baris.

plt.imshow(image, cmap='gray') digunakan untuk menampilkan gambar asli dalam mode grayscale.

plt.title('Original Image') menambahkan judul "Original Image" pada subplot.

plt.axis('off') digunakan untuk menghilangkan sumbu (x dan y) pada plot.

plt.show() digunakan untuk menampilkan plot pada layar.

plt.subplot(1, 2, 2) digunakan untuk membuat subplot kedua.

plt.imshow(edges, cmap='gray') digunakan untuk menampilkan hasil dari Canny edge detection dalam mode grayscale.

plt.title('Canny Edge Detection') menambahkan judul "Canny Edge Detection" pada subplot.

plt.axis('offplt.show() digunakan untuk menampilkan plot yang telah dibuat pada layar.') 

cv2.imread() digunakan untuk membaca gambar dari file. Gambar yang dibaca akan disimpan dalam variabel image.

fotoo.JPEG adalah nama file gambar yang akan dibaca. Pastikan file ini berada di direktori yang sama dengan script atau berikan path lengkapnya.

cv2.cvtColor() digunakan untuk mengubah gambar dari format BGR (default OpenCV) ke grayscale.

cv2.threshold() digunakan untuk menerapkan thresholding pada gambar grayscale. Gambar biner disimpan dalam variabel thresh.

Parameter pertama adalah gambar yang akan diproses.

Parameter kedua adalah nilai threshold (127 dalam hal ini).

Parameter ketiga adalah nilai maksimum yang diberikan kepada piksel yang melebihi threshold (255 dalam hal ini).

cv2.findContours() digunakan untuk menemukan kontur pada gambar biner.
Parameter pertama adalah gambar biner.

cv2.RETR_TREE adalah mode retrieval yang digunakan untuk mendapatkan semua kontur dan membuat relasi hierarkis di antara mereka.

cv2.CHAIN_APPROX_SIMPLE digunakan untuk menyederhanakan kontur dengan menghapus titik-titik redundan.cv2.THRESH_BINARY adalah jenis threshold yang digunakan (biner).

image.copy() digunakan untuk membuat salinan dari gambar asli agar kontur dapat digambar di atasnya tanpa mengubah gambar asli.

cv2.drawContours() digunakan untuk menggambar kontur pada salinan gambar.

Parameter pertama adalah gambar yang akan digambar kontur.

Parameter kedua adalah daftar kontur yang ditemukan sebelumnya.

Parameter ketiga adalah indeks kontur yang akan digambar (-1 berarti semua kontur).

Parameter keempat adalah warna kontur (0, 255, 0) yang berarti hijau dalam format BGR.

cv2.cvtColor() digunakan untuk mengubah format gambar dari BGR ke RGB, karena Matplotlib menggunakan format RGB.

plt.figure(figsize=(10, 5)) digunakan untuk membuat sebuah figure baru dengan ukuran 10x5 inci.

plt.subplot(1, 2, 1) digunakan untuk membuat subplot pertama dari dua subplot yang ada dalam satu baris.

plt.imshow(image_rgb) digunakan untuk menampilkan gambar asli dalam format RGB.

plt.title('Original Image') menambahkan judul "Original Image" pada subplot.

plt.axis('off') digunakan untuk menghilangkan sumbu (x dan y) pada plot.

plt.subplot(1, 2, 2) digunakan untuk membuat subplot kedua.

plt.imshow(image_contours_rgb) digunakan untuk menampilkan gambar dengan kontur dalam format RGB.

plt.title('Contours Detection') menambahkan judul "Contours Detection" pada subplot.

plt.axis('off') digunakan untuk menghilangkan sumbu (x dan y) pada plot.Parameter kelima adalah ketebalan garis kontur (2 piksel).

