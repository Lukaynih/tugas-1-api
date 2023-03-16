# WELCOME

		- Nama				: Muhammad Rafli Rasyidin
		- Kelas				: 17.6A.26
		- Nim				: 17200892
		- Mata Kuliah		: Web Programming
		- Tugas Pertemuan	: 1 (Satu)

## Sintak - Sintak Dasar Git
	
**git config**

Salah satu perintah git yang paling banyak digunakan adalah **git config**
yang bisa digunakan untuk mengatur konfigurasi tertentu sesuai keinginan pengguna, seperti email, algoritma untuk diff, username, format file, dll.
contohnya, perintah berikut bisa digunakan untuk mengatur email:

	git config --global user.email sam@google.com

**git init**
	Perintah ini digunakan untuk membuat reoisitori baru. caranya:

	git init

**git add**
Perintah git add bisa digunakan untuk menambahkan file ke index.
Contohnya, perintah berikut ii akan menambahkan file bernama tempt.txt
yang ada di direktori lokal ke index:

git addd temp.txt

**git clone**
Perintah git clone digunakan untuk checkout repositori. jia repositori berada di remove server, gunakan:

git clone alex@93.188.160.5:/path/to/repository

jika salinan repositori lokal ingin dibuat, gunakan:

git clone/path/to/repository

**git branch**
Cabang sangat penting di dunia git. Dengan menggunakan cabang, beberapa pengembang dapat bekerja secara paralel pada proyek yang sama secara bersamaan. Kita dapat menggunakan perintah git branch untuk membuat, mendaftar, dan menghapus cabang.

```
git branch <branch-name>

git push -u <remote> <branch-name>
```

**Git checkout**
Ini juga salah satu perintah Git yang paling banyak digunakan. Untuk bekerja di cabang, pertama-tama Anda harus beralih ke sana. Kami menggunakan **git checkout** sebagian besar untuk beralih dari satu cabang ke cabang lainnya. Kami juga dapat menggunakannya untuk memeriksa file dan melakukan.

```
git checkout <name-of-your-branch>
```

Ada beberapa langkah yang perlu Anda ikuti untuk berhasil berpindah antar cabang:

-   Perubahan di cabang Anda saat ini harus dilakukan atau disimpan sebelum Anda beralih
-   Cabang yang ingin Anda periksa harus ada di lokal Anda



```
git checkout -b <name-of-your-branch>
```

Perintah ini membuat cabang baru di lokal Anda (-b singkatan dari cabang) dan memeriksa cabang ke baru tepat setelah dibuat.

**Git status**
Saat kami membuat, memodifikasi, atau menghapus file, perubahan ini akan terjadi di lokal kami dan tidak akan disertakan dalam komit berikutnya (kecuali jika kami mengubah konfigurasi).

Kita perlu menggunakan perintah git add untuk memasukkan perubahan file ke dalam komit kita berikutnya.

**Untuk menambahkan satu file:**

```
git add <file>
```

**Untuk menambahkan semuanya sekaligus:**

```
git add -A
```

Ketika Anda mengunjungi tangkapan layar di atas pada bagian ke-4, Anda akan melihat bahwa ada nama file yang berwarna merah - ini berarti file tersebut adalah file yang belum dipentaskan. File yang tidak dipentaskan tidak akan disertakan dalam komit Anda.

**git commit**
Ini mungkin perintah Git yang paling banyak digunakan. Setelah kami mencapai titik tertentu dalam pengembangan, kami ingin menyimpan perubahan kami (mungkin setelah tugas atau masalah tertentu).

Git commit seperti menyetel titik pemeriksaan dalam proses pengembangan yang dapat Anda kembalikan nanti jika diperlukan.

Kami juga perlu menulis pesan singkat untuk menjelaskan apa yang telah kami kembangkan atau ubah dalam kode sumber.

```
git commit -m "commit message"
```

**Penting: Git commit hanya menyimpan perubahan Anda secara lokal.**

**Git push**
Setelah melakukan perubahan Anda, hal berikutnya yang ingin Anda lakukan adalah mengirimkan perubahan Anda ke server jarak jauh. Git push mengunggah komit Anda ke repositori jarak jauh.
```
git push <remote> <branch-name>
```

Namun, jika cabang Anda baru dibuat, Anda juga perlu mengunggah cabang tersebut dengan perintah berikut:

```
git push --set-upstream <remote> <name-of-your-branch>
```

atau

```
git push -u origin <branch_name>
```



**Git Pull**

Perintah **git pull** digunakan untuk mendapatkan pembaruan dari repo jarak jauh. Perintah ini adalah kombinasi dari **git fetch** dan **git merge** yang artinya, saat kita menggunakan git pull, perintah ini mendapatkan pembaruan dari repositori jarak jauh (git fetch) dan segera menerapkan perubahan terbaru di lokal Anda (git merge).

```
git pull <remote>
```
	 