---
author: "Ilham N"
title: "Hacktoberfest 2025 💻"
date: "2025-10-20"
description: "dokumentasi hacktoberfest 2025 [DOKSLI]"
tags: ["event", "programmer", "git"]
draft: false
---

![header](https://hacktoberfest.com/_next/static/media/opengraph.6e804091.png)

> _Di antara ribuan commit yang ku-push setiap hari, dirimu tetap satu-satunya branch yang tak pernah ingin ku-merge dengan siapa pun._

Duh.

Yah, ini sharing-sharing aja sih. Pastikan udah daftar [disini](https://hacktoberfest.com/profile/) ya

---

### Tentang Repository

Siapin dulu reponya banh, kita mengenal ada 2 jenis:

1. Remote Repository
   ![remote repo](/posts/7/image.png)
2. Local Repository
   ![local repo](/posts/7/image-1.png)

fungsinya? _remote_ buat pusat datanya, _local_ buat (proses) melakukan perubahan. Idealnya perubahan dari dalam dulu (lokal) sebelum ditampilkan keluar (remote), kan?

### Basic Command

1. Perubahan di lokal

   ![save-local](/posts/7/image-2.png)

   (misal saya) menambahkan perubahan pada baris 141, jangan lupa di save.

2. Simpan, tambahkan

   ![add](/posts/7/image-3.png)

   > “Memasukkan barang X ke kotak pengiriman.”

   ```sh
    git add file-terdampak
   ```

   untuk cek status, gunakan

   ```sh
    git status
   ```

   Ini adalah staging: barang sudah dipilih dan siap dikemas, tapi belum difinalisasi.

3. Commit

   ![commit](/posts/7/image-4.png)

   > “Kotak disegel dengan daftar isi: ‘perbaikan tombol login’.”

   ```sh
    git commit -m "catatan perubahan"
   ```

   jangan lupa untuk cek status

   ```sh
    git status
   ```

   Commit = rekaman lokal dari keadaan paket pada saat itu.

4. Upload ke remote

   ![push](/posts/7/image-5.png)

   > “Kurir di-panggil — paket dikirim ke gudang pusat.”

   ```sh
    git push
   ```

   Push = kirim perubahan dari lokal ke gedung pusat.

5. Check

   ![check-update](/posts/7/image-6.png)

   > “Pastikan deskripsi paket sesuai commit sebelumnya.”

### Geme Start

> Disini letak asiknya.

1. Remote Repository

   ![check-update](/posts/7/image-6.png)

   masih di halaman remote repository, masuk ke tab Pull Requests.

2. Pull Requests

   ![new-pull-req](/posts/7/image-7.png)

   tekan new pull request

   ![create-pull-req](/posts/7/image-8.png)

   pastikan comparing changes branch sesuai dengan repo yg dituju. misal case yg saya kerjakan saat ini adalah :

   ![comparing-changes](/posts/7/image-9.png)

   > dari remote repo IlhamLamp/hello-world.
   > ke repo akmalsyrf/hello-world.

   ![labels-assign-req](/posts/7/image-10.png)

   isi deskripsi sesuai kebutuhan,
   sesuaikan label dengan **hacktoberfest-accepted**

   sudah sesuai? tekan button _create pull request_

3. Merge Requests

   ![merge-req](/posts/7/image-11.png)

   pastikan setiap title, label, desc, dll sudah sesuai. kemudian tekan button _merge pull request_.

   > opsional : biarkan commit message default
   > ![com-message](/posts/7/image-12.png)

   terakhir, tekan button _confirm merge_.

   halaman berubah menjadi berikut,

   ![merged](/posts/7/image-13.png)

   proses merging sudah selesai.

   ![status](/posts/7/image-14.png)

   remote repository sudah merekam perubahan.

### Selanjutnya apa?

cek lagi [disini](https://hacktoberfest.com/profile/), proses merge yg berhasil sebelumnya membutuhkan kurang lebih 15 menit sampai ter-rekam di halaman.

![pr/m-status](/posts/7/image-15.png)

Untuk mengulangi langkah, pastikan repository pribadi kita sudah di sync dengan tujuan, misal (saya):

    > https://github.com/IlhamLamp/hello-world

![alt text](/posts/7/image-16.png)

tekan _update branch_.

terakhir, di local repository (vs code), lakukan berikut :

![git pull](/posts/7/image-17.png)

```sh
    git pull
```

Hal ini untuk melakukan sync juga yg ada di local repo.
