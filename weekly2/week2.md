**Review Weekly1**
![review-weekly1](./review-w1.png)

**Deleting File**
Saat mendelete file maka working directory akan membaca perubahan tersebut
agar perubahan pada github kita terupadate kita perlu lakukan add agar
delete file berpindah ke staged area
jadi langkahnya:
1.) Hapus File
2.) git status
3.) git add (file-yang-dihapus)
4.) git commit -m 'pesannya'
5.) git push origin master
6.) lalu lakukan git log untuk mengecek perubahan yang terjadi
atau
6.) git log --oneline untuk mengecek perubahan secara ringkas

**Membatalkan penambahan file di working directory**
Jika ingin menambahkan file ke working directory dan membatalkan perubahannya
![git-clean](git-clean.png)

**Membatalkan penambahan file di staged area**
jika ingin membatalkan perubahan pada saat di staged area maka dapat lakukan
/git restore --staged #ini akan membatalkan seluruh perubahan pada staged area
atau
/git restore --staged (nama-file)
maka perubahan dari staged area akan kembali ke working directory

Jika kita ingin membatalkan spesifik file di staged area bisa lakukan
![git-restore](./git-restore.png)

**menghapus file dengan git reset**
terdapat 3 mode pada git reset
--soft hanya memindahkan HEAD pointer
--mixed memindahkan HEAD pointer dan mengubah staging area sama seperti pada repo
--hard memindahkan HEAD pointer dan mengubah staging area, working directory sama seperti pada repo

![git-reset-mode](./git-reset.png)
![git-reset-mode2](./git-reset2.png)

#Warning pada penggunaan git reset
![git-reset3](./git-reset3.png)

**Git Revert**
mengembalikan ke kondisi sebelumnya dan membuat commit baru dengan hasil kondisi yang dikembalikan
git revert
