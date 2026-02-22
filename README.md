## 📊 Part 6: Menampilkan Data dengan Tabel

Tabel digunakan untuk menyajikan data dalam baris dan kolom agar mudah dibandingkan. Di HTML, membuat tabel itu seperti menyusun bata: kita buat wadahnya dulu, lalu barisnya, baru kemudian isinya.

### 📚 Teori Singkat

Berdasarkan file `alltag.html`, sebuah tabel minimal membutuhkan empat tag utama ini:

1. **`<table>`**: Wadah utama pembungkus seluruh data tabel.
2. **`<tr>` (Table Row)**: Digunakan untuk membuat **baris**. Setiap kamu ingin membuat baris baru ke bawah, kamu butuh tag ini.
3. **`<th>` (Table Header)**: Digunakan untuk judul kolom. Teks di dalam tag ini biasanya otomatis tercetak **tebal** dan berada di tengah oleh browser.
4. **`<td>` (Table Data)**: Digunakan untuk mengisi sel/kolom dengan data biasa.
5. **Atribut `border**`: Digunakan di dalam tag `<table>` untuk memunculkan garis pembatas agar tabel tidak terlihat melayang.

---

### 🛠️ Praktek: "The Data Center"

Mari kita buat tabel jadwal atau daftar nilai sederhana di file `index.html` kamu.

**Langkah 1: Tambahkan Konten Baru**
Masukkan kode ini di bawah materi List (Part 5):

```html
<hr />

<h2>Daftar Nilai Siswa</h2>

<table border="2">
  <tr>
    <th>No</th>
    <th>Nama Siswa</th>
    <th>Mata Pelajaran</th>
    <th>Nilai</th>
  </tr>

  <tr>
    <td>1</td>
    <td>Budi Santoso</td>
    <td>HTML Dasar</td>
    <td>95</td>
  </tr>

  <tr>
    <td>2</td>
    <td>Siti Aminah</td>
    <td>CSS Layout</td>
    <td>88</td>
  </tr>
</table>
```

---

### 🔍 Analisis Struktur Baris & Kolom

Jika kamu perhatikan file `alltag.html`:

- **Baris 98-113**: Memperlihatkan penggunaan `border="2"`. Angka ini menentukan ketebalan garis tabelmu.
- **Baris 100-104**: Menunjukkan bagaimana `<th>` membedakan antara judul (Nama, Kelas, Sekolah) dengan isi datanya.

> **Tips:** Bayangkan `<tr>` sebagai baris horizontal (ke samping) dan `<td>`/`<th>` sebagai kotak-kotak di dalam baris tersebut. Semakin banyak `<td>` yang kamu tulis di dalam satu `<tr>`, semakin banyak kolom yang akan terbentuk.

---

### 💡 Tantangan untuk Kamu (Challenge)

1. Buatlah sebuah tabel berisi "Jadwal Harian" kamu.
2. Gunakan 3 kolom: **Jam**, **Aktivitas**, dan **Status** (Selesai/Belum).
3. Gunakan atribut `border="1"` agar garisnya lebih tipis.
4. Tambahkan minimal 3 baris aktivitas.

**Bagaimana? Apakah datanya sudah tersusun rapi dalam kotak-kotak? Kalau sudah berhasil, kabari ya! Kita akan lanjut ke Part 7 untuk belajar cara menghubungkan satu halaman ke halaman lain (Hyperlinks)!**

---

Mantap! Sekarang kita masuk ke bagian yang membuat internet menjadi "jaring lab-lab", yaitu **Hyperlinks**. Tanpa tag ini, website hanyalah dokumen mati yang berdiri sendiri.

---

## 🔗 Part 7: Navigasi dan Link (Hyperlinks)

Link adalah jembatan yang menghubungkan satu halaman ke halaman lain, atau bahkan ke bagian tertentu dalam halaman yang sama.

### 📚 Teori Singkat

Berdasarkan file `alltag.html`, senjata utama untuk membuat link adalah tag `<a>` (Anchor). Ada tiga jenis link yang sering digunakan:

1. **Eksternal Link**: Menuju website lain (misal: Google). Kamu butuh atribut `href` untuk alamatnya dan `target="_blank"` jika ingin link terbuka di tab baru.
2. **Internal Link**: Menuju file HTML lain di dalam folder yang sama (misal: `kontak.html`).
3. **Anchor Link (Bookmark)**: Menuju bagian tertentu di halaman yang sama menggunakan atribut `id`.
4. **Link Email/Telepon**: Menggunakan perintah `mailto:` atau `tel:`.

---

### 🛠️ Praktek: "The Web Connector"

Mari kita buat navigasi sederhana di file `index.html` kamu.

**Langkah 1: Tambahkan Konten Baru**
Masukkan kode ini di bawah tabel (Part 6):

```html
<hr />

<h2 id="bagian-link">Navigasi Halaman</h2>

<p>
  Kunjungi website resmi
  <a href="https://www.google.com" target="_blank">Google di sini</a>.
</p>

<p>
  Hubungi saya di:
  <a href="mailto:admin@belajarweb.com">admin@belajarweb.com</a>
</p>

<p>
  Kembali ke
  <a href="#bagian-link">Judul Navigasi</a> atau ke
  <a href="#Bab 6">Bagian Formulir di file alltag</a>.
</p>
```

---

### 🔍 Analisis "Si Alamat href"

Jika kamu perhatikan file `alltag.html`:

- **Baris 118-121**: Menunjukkan cara membuat link ke website luar (Wikipedia) dan link email.
- **Baris 122**: Menunjukkan link internal yang merujuk pada `id="Bab 6"`. Ini sangat berguna untuk halaman web yang sangat panjang agar pengunjung bisa "melompat" ke bagian bawah dengan satu klik.

> **Tips:** `href` adalah singkatan dari _Hypertext Reference_. Ingatlah ini sebagai "Alamat Tujuan" dari link tersebut.

---

### 💡 Tantangan untuk Kamu (Challenge)

1. Buatlah sebuah link yang menuju ke profil media sosial atau website favoritmu.
2. Pastikan link tersebut terbuka di **Tab Baru** (gunakan `target="_blank"`).
3. Buat sebuah kata di paling bawah halamanmu (misal: "Ke Atas") yang jika diklik akan memindahkan layar kembali ke `<h1>` di paling atas (Gunakan `id` pada `<h1>` tersebut sebagai targetnya).

**Apakah link-mu sudah berfungsi dan bisa "melompat"? Jika sudah lancar, kabari ya! Kita akan lanjut ke Part 8 yang paling seru: Multimedia (Gambar & Video)!**

---

Siap! Sekarang kita masuk ke bagian yang paling "hidup". Sebuah website tanpa gambar atau suara akan terasa sangat sepi. Mari kita belajar cara memasukkan **Multimedia**.

---

## 🖼️ Part 8: Multimedia (Image, Audio, Video)

Bagian ini menjelaskan bagaimana cara menampilkan aset visual dan audio agar pengunjung betah berlama-lama di website kamu.

### 📚 Teori Singkat

Berdasarkan bagian akhir file `alltag.html`, ada tiga tag utama yang harus kamu kuasai:

1. **`<img>` (Image)**: Tag ini unik karena tidak punya penutup (self-closing). Kamu butuh atribut `src` (sumber gambar) dan `alt` (teks alternatif jika gambar gagal dimuat).
2. **`<audio>`**: Digunakan untuk memutar musik atau suara. Kamu wajib menambahkan atribut `controls` agar tombol _play/pause_ muncul.
3. **`<video>`**: Mirip dengan audio, tapi untuk film/video. Kamu bisa mengatur `width` (lebar) dan `height` (tinggi) agar ukurannya pas di layar.
4. **Atribut Pendukung**:

- `loop`: Mengulang putaran secara otomatis.
- `poster`: Gambar sampul sebelum video diputar.

---

### 🛠️ Praktek: "The Media Gallery"

Mari kita coba masukkan media ke file `index.html`. Karena kamu mungkin belum punya file aslinya, kita akan gunakan link internet sebagai contoh.

**Langkah 1: Tambahkan Konten Baru**
Masukkan kode ini di bawah bagian Link (Part 7):

```html
<hr />

<h2>Galeri Multimedia</h2>

<p>Foto Pemandangan:</p>
<img
  src="https://via.placeholder.com/300x200"
  alt="Contoh Gambar Placeholder"
  width="300"
/>

<p>Putar Musik:</p>
<audio controls>
  <source src="Asset/soundwormhole.mp3" type="audio/mpeg" />
  Audio tidak didukung oleh browser kamu.
</audio>

<p>Tonton Video:</p>
<video
  width="320"
  height="240"
  controls
  poster="https://via.placeholder.com/320x240"
>
  <source src="Asset/wormhole.mp4" type="video/mp4" />
  Video tidak didukung.
</video>
```

---

### 🔍 Analisis "Path & Fallback"

Jika kamu melihat file `alltag.html`:

- **Baris terakhir-terakhir**: Filemu menggunakan `src="Asset/..."`. Ini artinya browser mencari file di dalam folder bernama **Asset**. Jika file tidak ada di sana, media tidak akan muncul.
- **Teks "Audio/Video tidak didukung"**: Ini disebut _fallback text_. Teks ini hanya akan muncul jika pengunjung menggunakan browser jadul yang tidak bisa memutar media tersebut.

> **Tips:** Selalu sertakan atribut `alt` pada gambar. Selain membantu orang tuna netra, ini juga membantu Google mengenali gambar apa yang kamu pasang (bagus untuk SEO!).

---

### 💡 Tantangan untuk Kamu (Challenge)

1. Cari satu link gambar di Google (klik kanan gambar > _copy image address_).
2. Pasang gambar tersebut di `index.html` kamu menggunakan tag `<img>`.
3. Berikan atribut `border="5"` pada gambar tersebut (atribut jadul tapi seru buat dicoba).
4. Coba tambahkan atribut `autoplay` pada tag `<audio>`, lalu simpan dan refresh. (Catatan: Banyak browser modern memblokir autoplay suara demi kenyamanan pengguna).

**Sudah muncul gambarnya? Jika sudah "ramai" websitemu, kabari ya! Kita lanjut ke Part 9 untuk mulai membuat Formulir (Input Text & Password)!**

---

Siap! Sekarang kita masuk ke bagian yang membuat website menjadi **interaktif**. Jika sebelumnya kita hanya menyajikan informasi, sekarang kita akan belajar cara menerima data dari pengunjung.

---

## 📝 Part 9: Formulir Dasar (Input & Label)

Formulir adalah pintu masuk bagi data user, mulai dari daftar akun sampai login. Di HTML, kita menggunakan tag `<form>` sebagai wadah besarnya.

### 📚 Teori Singkat

Berdasarkan bagian "Formulir Masukan" di file `alltag.html`, ada beberapa elemen dasar yang wajib kamu ketahui:

1. **`<form>`**: Kontainer utama untuk formulir. Memiliki atribut `action` (kemana data dikirim) dan `method`.
2. **`<label>`**: Nama atau keterangan untuk input. Sangat penting agar user tahu apa yang harus diisi.
3. **`<input type="text">`**: Kotak isian standar untuk teks pendek seperti Nama atau Username.
4. **`<input type="password">`**: Kotak isian yang otomatis menyembunyikan karakter (menjadi titik-titik atau bintang) demi keamanan.
5. **`<br />`**: Digunakan untuk membuat baris baru agar isian formulir tersusun rapi ke bawah (tidak berderet ke samping).

---

### 🛠️ Praktek: "Halaman Login Sederhana"

Mari kita buat formulir login dasar di file `index.html` kamu.

**Langkah 1: Tambahkan Konten Baru**
Masukkan kode ini di bawah bagian Multimedia (Part 8):

```html
<hr />

<h2>Formulir Akses Pengguna</h2>

<form action="#">
  <label>Nama Pengguna:</label><br />
  <input
    type="text"
    name="username"
    placeholder="Masukkan nama..."
  /><br /><br />

  <label>Kata Sandi:</label><br />
  <input type="password" name="pass" /><br /><br />

  <input type="submit" value="Masuk Ke Sistem" />
</form>
```

---

### 🔍 Analisis "Kerahasiaan Data"

Jika kamu perhatikan file `alltag.html`:

- **Baris 130-134**: Menunjukkan perbedaan antara `type="text"` dan `type="password"`. Meskipun keduanya adalah kotak isian, perilakunya di layar sangat berbeda demi menjaga privasi pengguna.
- **Atribut `name**`: Ini adalah identitas dari data tersebut. Saat data dikirim ke server, server akan mengenali isian tersebut berdasarkan nama yang kamu berikan (misal: `name="nama"`).

> **Tips:** Gunakan atribut `placeholder` di dalam input untuk memberikan petunjuk tipis kepada pengguna tentang apa yang harus diketik.

---

### 💡 Tantangan untuk Kamu (Challenge)

1. Buatlah formulir baru berjudul "Pendaftaran Event".
2. Tambahkan input untuk **Nama Lengkap** dan **Alamat Email**. (Tips: Untuk email, kamu bisa mencoba `type="email"`).
3. Tambahkan tag `<br />` agar tampilan antara label dan input tidak saling menabrak.
4. Coba ketik sesuatu di kolom password, apakah karakternya tersembunyi?

**Gimana? Sudah bisa membuat kotak input? Jika sudah berhasil, kabari ya! Kita akan lanjut ke Part 10 (Part Terakhir) untuk belajar Checkbox, Select Box, dan cara mengunggah file!**

---

Hore! Kita sampai di **Part 10**, bagian terakhir dari kurikulum HTML Dasar kita. Di sini kita akan melengkapi formulir dengan pilihan ganda, daftar tarik-turun, dan fitur unggah file.

---

## 🔗 Part 10: Formulir Lanjutan & Interaksi

Jika Part 9 baru soal mengetik, di Part 10 ini kita akan belajar memberikan pilihan kepada pengguna. User tidak perlu mengetik, cukup klik atau pilih saja.

### 📚 Teori Singkat

Berdasarkan sisa tag formulir di file `alltag.html`, berikut adalah elemen yang akan kita pelajari:

1. **Checkbox (`<input type="checkbox">`)**: Digunakan untuk pilihan yang bisa dipilih lebih dari satu (multi-pilihan). Contoh: Memilih hobi.
2. **Select Box (`<select>` & `<option>`)**: Membuat daftar tarik-turun (dropdown). Menghemat ruang di layar karena pilihan baru muncul saat diklik.
3. **File Upload (`<input type="file">`)**: Tombol khusus yang membuka folder komputer pengguna untuk memilih gambar atau dokumen yang akan diunggah.
4. **Textarea (`<textarea>`)**: Berbeda dengan input teks biasa, ini adalah kotak besar untuk menulis pesan panjang atau komentar.

---

### 🛠️ Praktek: "Formulir Profil Lengkap"

Mari kita gabungkan semuanya menjadi satu formulir pendaftaran yang lengkap di file `index.html` kamu.

**Langkah 1: Tambahkan Konten Baru**
Masukkan kode ini di bawah materi Part 9:

```html
<hr />

<h2>Lengkapi Profil Anda</h2>

<form action="#">
  <label>Hobi:</label><br />
  <input type="checkbox" name="hobi" value="coding" /> Coding
  <input type="checkbox" name="hobi" value="gaming" /> Gaming
  <input type="checkbox" name="hobi" value="reading" /> Membaca <br /><br />

  <label>Pekerjaan:</label><br />
  <select name="pekerjaan">
    <option value="siswa">Siswa</option>
    <option value="mahasiswa">Mahasiswa</option>
    <option value="guru">Guru/Dosen</option>
    <option value="umum">Umum</option>
  </select>
  <br /><br />

  <label>Unggah Foto Profil:</label><br />
  <input type="file" name="foto" />
  <br /><br />

  <label>Tentang Saya:</label><br />
  <textarea
    name="bio"
    rows="4"
    cols="30"
    placeholder="Ceritakan singkat tentang dirimu..."
  ></textarea>
  <br /><br />

  <input type="submit" value="Simpan Profil" />
</form>
```

---

### 🔍 Analisis Akhir `alltag.html`

Jika kamu scroll ke bagian paling bawah file `alltag.html`:

- **Baris 136-138**: Memperlihatkan bagaimana checkbox bekerja. User bisa mencentang "Memasak" dan "Menggambar" sekaligus.
- **Baris 141-146**: Menunjukkan struktur `<select>` yang membungkus banyak `<option>`.
- **Baris 149**: Adalah pintu gerbang bagi user untuk mengirimkan file ke servermu.

---

### 💡 Tantangan Terakhir (Final Challenge)

1. Tambahkan satu lagi pilihan pada **Select Box** (misal: "Developer").
2. Di dalam **Textarea**, gunakan atribut `rows="10"` untuk membuat kotaknya jadi sangat tinggi.
3. Buatlah satu paragraf di paling bawah halaman yang berisi ucapan: _"Selamat! Saya telah menyelesaikan 10 Part Belajar HTML Dasar."_ dan buat teks tersebut menjadi **Tebal** dan **Miring**.

---

**Selamat!** Kamu sudah berhasil membedah seluruh isi tag yang ada di file `alltag.html` dari nol sampai mahir secara struktur. Sekarang kamu sudah punya satu file `index.html` yang sangat panjang dan berisi semua elemen penting sebuah website.

Bagaimana perasaanmu setelah menyelesaikan Part 10 ini? Apakah ada bagian yang ingin kamu perdalam lagi, atau sudah siap lanjut ke dunia **CSS** agar tampilan webmu jadi lebih berwarna?

---

Wah, ide bagus! Sebagai penutup dari seri 10 Part ini, kita butuh satu "Ujian Akhir" yang menggabungkan semua ilmu dari Part 0 sampai Part 10. Ini akan membuktikan kalau kamu bukan cuma bisa _copy-paste_, tapi sudah bisa membangun struktur web sendiri.

Berikut adalah tambahan **Tugas Project** untuk **Part 10**:

---

## 🏆 Project Akhir: "The Digital Bio-Page"

**Goal:** Buatlah sebuah halaman "Profil Pribadi" atau "CV Online" sederhana dalam satu file HTML yang menggunakan minimal 80% tag yang sudah kita pelajari dari file `alltag.html`.

### 📋 Kriteria Tugas

Di dalam file `index.html` kamu, pastikan terdapat elemen-elemen berikut:

1. **Struktur Dasar (Part 0):** Dokumen harus punya `<!DOCTYPE html>`, `<html>`, `<head>`, dan `<body>`.
2. **Identitas (Part 1 & 3):** \* Gunakan `<h1>` untuk namamu.

- Gunakan `<abbr>` untuk gelar atau singkatan hobi.
- Masukkan kutipan favoritmu menggunakan `<blockquote>`.

3. **Teks & Cerita (Part 2 & 4):**

- Tuliskan bio singkat tentang dirimu.
- Gunakan **tebal**, _miring_, dan ~~coret~~ (misal: "Hobi lama: ~~Main Kelereng~~, Hobi baru: Coding").

4. **Data Terstruktur (Part 5 & 6):**

- Buat daftar (List) berisi "Skill atau Keahlian" kamu.
- Buat tabel (Table) berisi "Riwayat Pendidikan" atau "Jadwal Belajar HTML".

5. **Navigasi & Media (Part 7 & 8):**

- Masukkan foto profilmu (atau gambar dari internet) menggunakan `<img>`.
- Tambahkan link menuju media sosial atau emailmu.

6. **Interaksi (Part 9 & 10):**

- Buat "Formulir Kontak" di bagian bawah agar orang bisa mengirim pesan, memilih jenis layanan lewat _Dropdown_, dan mencentang _Checkbox_ setuju syarat & ketentuan.

---

### 🛠️ Contoh Gambaran Struktur Kode

```html
<h1 id="top">Profil Digital Saya</h1>

<center>
  <img src="https://via.placeholder.com/150" alt="Foto Saya" border="2" />
  <p>
    Halo, saya seorang <b><abbr title="Web Developer">WebDev</abbr></b> masa
    depan!
  </p>
</center>

<hr />

<h3>Riwayat Pendidikan</h3>
<table border="1" width="100%">
  <tr>
    <th>Tahun</th>
    <th>Instansi</th>
  </tr>
  <tr>
    <td>2024-2026</td>
    <td>Self-Taught di Jalur HTML</td>
  </tr>
</table>

<hr />

<h3>Hubungi Saya</h3>
<form>
  <input type="text" placeholder="Nama Anda" /><br />
  <textarea placeholder="Pesan Anda"></textarea><br />
  <input type="checkbox" /> Saya bukan robot <br />
  <input type="submit" value="Kirim Pesan" />
</form>

<a href="#top">Kembali ke Atas</a>
```

---

### 🔍 Cara Mengumpulkan

1. Simpan file tersebut.
2. Buka di browser dan pastikan tidak ada gambar yang pecah atau link yang mati.
3. Coba isi formulirnya dan klik tombol submit (meskipun belum terkirim ke server, pastikan halamannya ter-_refresh_).

**Gimana? Siap mengerjakan Project Akhir ini? Kalau sudah selesai, kamu boleh kirimkan kodenya di sini untuk saya review secara detail!**
