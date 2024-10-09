# Laporan Jobsheet 6
## Layout dan Navigasi
### Nama : Diva Aji Kurniawan <br> Kelas : TI 3G <br> No. Absen : 11 <br> NIM : 2241720183

## Praktikum 1: Membangun Layout di Flutter
### Langkah 1: Buat Project Baru
Link repo github: https://github.com/DivaAji/layout_flutter

Buatlah sebuah project flutter baru dengan nama layout_flutter.
<img src="images/1.1.png">

### Langkah 2: Buka file lib/main.dart
Buka file main.dart lalu ganti dengan kode berikut. Isi nama dan NIM Anda di text title.
<img src="images/1.2.png">

### Langkah 3: Identifikasi layout diagram
### Langkah 4: Implementasi title row
Membuat kolom bagian kiri pada judul. Tambahkan kode berikut di bagian atas metode build() di dalam kelas MyApp:
```
Widget titleSection = Container(
  padding: const EdgeInsets.all(...),
  child: Row(
    children: [
      Expanded(
        /* soal 1*/
        child: Column(
          crossAxisAlignment: ...,
          children: [
            /* soal 2*/
            Container(
              padding: const EdgeInsets.only(bottom: ...),
              child: const Text(
                'Wisata Gunung di Batu',
                style: TextStyle(
                  fontWeight: FontWeight.bold,
                ),
              ),
            ),
            Text(
              'Batu, Malang, Indonesia',
              style: TextStyle(...),
            ),
          ],
        ),
      ),
      /* soal 3*/
      Icon(
       ...,
        color: ...,
      ),
      const Text(...),
    ],
  ),
);
```

**soal 1**  
Letakkan widget Column di dalam widget Expanded agar menyesuaikan ruang yang tersisa di dalam widget Row. Tambahkan properti crossAxisAlignment ke CrossAxisAlignment.start sehingga posisi kolom berada di awal baris.
<img src="images/1.4.1.png">

**soal 2** 
Letakkan baris pertama teks di dalam Container sehingga memungkinkan Anda untuk menambahkan padding = 8. Teks ‘Batu, Malang, Indonesia' di dalam Column, set warna menjadi abu-abu.
<img src="images/1.4.2.png">

**soal 3** 
Dua item terakhir di baris judul adalah ikon bintang, set dengan warna merah, dan teks "41". Seluruh baris ada di dalam Container dan beri padding di sepanjang setiap tepinya sebesar 32 piksel. Kemudian ganti isi body text ‘Hello World' dengan variabel titleSection
<img src="images/1.4.3.1.png">
<img src="images/1.4.3.2.png">
<img src="images/1.4.3.3.png">

### Output Praktikum 1
<img src="images/output1.png">

## Praktikum 2: Implementasi button row
### Langkah 1: Buat method Column _buildButtonColumn
<img src="images/2.1.png">

### Langkah 2: Buat widget buttonSection
Buat Fungsi untuk menambahkan ikon langsung ke kolom. Teks berada di dalam Container dengan margin hanya di bagian atas, yang memisahkan teks dari ikon.
<img src="images/2.2.png">

### Langkah 3: Tambah button section ke body
Tambahkan variabel buttonSection ke dalam body seperti berikut:
<img src="images/2.3.png">

### Output Praktikum 2
<img src="images/output2.png">

## Praktikum 3: Implementasi text section
### Langkah 1: Buat widget textSection
Tentukan bagian teks sebagai variabel. Masukkan teks ke dalam Container dan tambahkan padding di sepanjang setiap tepinya. Tambahkan kode berikut tepat di bawah deklarasi buttonSection:
<img src="images/3.1.png">

### Langkah 2: Tambahkan variabel text section ke body
Tambahkan widget variabel textSection ke dalam body seperti berikut:
<img src="images/3.2.png">

### Output Praktikum 3
<img src="images/output3.png">

## Praktikum 4: Implementasi image section
### Langkah 1: Siapkan aset gambar
Buatlah folder images di root project layout_flutter. Masukkan file gambar tersebut ke folder images, lalu set nama file tersebut ke file pubspec.yaml seperti berikut:
<img src="images/4.1.png">

### Langkah 2: Tambahkan gambar ke body
Tambahkan aset gambar ke dalam body:
<img src="images/4.2.png">
BoxFit.cover memberi tahu kerangka kerja bahwa gambar harus sekecil mungkin tetapi menutupi seluruh kotak rendernya.

### Langkah 3: Terakhir, ubah menjadi ListView
Pada langkah terakhir ini, atur semua elemen dalam ListView, bukan Column, karena ListView mendukung scroll yang dinamis saat aplikasi dijalankan pada perangkat yang resolusinya lebih kecil.
<img src="images/4.3.png">

### Output praktikum 4
<img src="images/output4.png">

## Tugas Praktikum 1
1. Selesaikan Praktikum 1 sampai 4, lalu dokumentasikan dan push ke repository Anda berupa screenshot setiap hasil pekerjaan beserta penjelasannya di file README.md!
>Link repo : https://github.com/DivaAji/layout_flutter
2. Silakan implementasikan di project baru "basic_layout_flutter" dengan mengakses sumber ini: https://docs.flutter.dev/codelabs/layout-basics
>Link repo : https://github.com/DivaAji/basic_layout_flutter
3. Kumpulkan link commit repository GitHub Anda kepada dosen yang telah disepakati!
