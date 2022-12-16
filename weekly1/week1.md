terdapat 3 state dan section di git

.) modified -> working directory
.) staged -> staging area
.) committed -> repository

![git-workflow](git-workflow.jpg)

snapshot -> menghasilkan hash sebagai identitas untuk setiap commitnya
![snapshot-diagram](snapshot-diagram.png)
jika antar snapshot tidak sesuai maka susunan parentnya akan rusak

perhitungan hash

.) tidak hanya pada perubahan file tapi juga dari parent, dan child

head

.) pointer untuk menunjuk hash paling akhir
![diagram-head](diagram-head.png)

praktik

**Menambah File**
//git add .
atau
// git add file.ext

setelah di add akan pindah ke state staged -> staging area

**Commit file**
setelah melakukan add kita lakukan commit agar state pindah ke committed

//git commit -m 'pesan commit'

setelah di commit git akan memberikan sha yang unik
dan kondisi statenya berubah ke committed -> repository

**Melakukan log**

kita bisa lakukan log untuk melihat perubahan yang kita lakukan

//git log

Conventional Commit Message
agar setiap push yang kita lakukan terlihat jelas pesannya
kita bisa lakukan conventional commit message setelah file di add

-> Feat
-> Fix
-> Chore

//git commit -m 'Feat: message'

//git commit -m 'Fix: message'

//git commit -m 'Chore: message'
