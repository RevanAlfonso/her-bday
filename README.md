# 🎂 her-bday — Template Ucapan Ulang Tahun Interaktif

Template open-source berbasis HTML untuk membuat halaman ucapan ulang tahun interaktif dan estetik. Termasuk greeting, musik, galeri foto polaroid, hingga minigame sederhana. Cocok dijadikan hadiah digital yang unik dan personal.

## ✨ Fitur

- 🎉 Halaman ucapan ulang tahun personal
- 🎵 Musik latar otomatis
- 🕹️ Minigame sederhana
- 📸 Galeri polaroid
- 💌 Desain visual sederhana & manis
- 💻 100% berbasis HTML/CSS/JS (tanpa framework)

## 🔧 Cara Menggunakan
## ✨ Bagian yang Perlu Disesuaikan - Bagian index.js dan Main.js

Berikut adalah bagian-bagian yang bisa/harus kamu ubah untuk menyesuaikan templat ini dengan orang yang ingin kamu beri kejutan ulang tahun.

### 1. 🎉 Nama Ulang Tahun
- Cari dan ganti semua `[Nama Kamu]` di seluruh file. CTRL + F
- Cari dan ganti semua `[IDOLA] ` di seluruh file. CTRL + F

### 2. 🖼️ Foto Karakter
Ganti file ./img/mainpp.jpeg dengan gambar lain sesuai karakter yang kamu inginkan.
Pastikan ukuran gambar persegi agar proporsional saat ditampilkan.
Nama file bisa disesuaikan, tapi pastikan path-nya cocok di HTML:
```
<img src="./img/mainpp.jpeg" alt="Sanzu">
```

### 3. 🔊 Musik Latar
Ganti file ./music/w2e.mp3 dengan lagu latar favorit penerima.
Pastikan format .mp3.
Update path-nya jika perlu:
```
<source src="./music/w2e.mp3" type="audio/mpeg">
```

### 4. 💬 Dialog Chat dan Pilihan
Dialog dan pilihan terstruktur di bagian chatFlow dalam JavaScript.
Contoh:
```
{
  messages: [ 
    { sender: 'sanzu', text: 'Dapet tugas dari bos hari ini.', delay: 1000 },
    ...
  ],
  choices: [
    { text: 'Eh, Betulan Ke ni?', response: 'choice1' },
    { text: 'Makasih ya sanzu', response: 'choice2' }
  ]
}
```

### 5. 📝 Ucapan Personal
Ada di halaman akhir (birthdayPage), dalam bagian:
```
<p class="text-base leading-relaxed">
  Happy birthday, Honey. Semoga hari ini jadi awal dari banyak hal baik yang datang ke hidupmu...
</p>
Sesuaikan ucapan ini agar lebih personal dan bermakna.
```

### 6. 🎁 Teks Penutup
Bagian akhir ditutup dengan teks seperti:
```
{ sender: 'sanzu', text: 'King Repan.', delay: 5200 }
```
Ubah agar sesuai dengan nama pengirim sebenarnya atau nama panggilan lucu lainnya.

## 💡 Tips Penggunaan
- Pastikan semua file (`music`, `img`) sudah dimasukkan ke folder yang sesuai.
- Bisa dijalankan langsung lokal di browser atau diunggah ke Netlify/Vercel untuk dibagikan.
- Pastikan autoplay music bisa berjalan — browser biasanya membatasi autoplay, jadi user harus interaksi dulu (sudah disiasati lewat tombol “Mulai”).