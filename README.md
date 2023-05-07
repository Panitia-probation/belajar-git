## Flow Development

### Jika belum di-clone repositorinya

pindah ke direktori/folder yang diinginkan didalamnya repositori ini 

`cd ...`

clone repositori

`git clone https://github.com/Panitia-probation/belajar-git`

### Branch development

untuk menambah suatu fitur, jangan sampai memodifikasi di branch `master`. silahkan pindah ke suatu branch fitur, dulu:
 

untuk buat branch baru

`git branch [feature-branch]`

untuk pindah ke branch yang sudah ada 

`git checkout [feature-branch]`

lakukan modifikasi pada branch fitur

setelah melakukan modifikasi pada branch `[feature-branch]` commit pada repositori lokal

`git add -A`

`git commit -m "[pesan-perubahan]"`

pada saat ini, tidak ada test suite maka langsung aja merge ke master branch

pindah kembali ke branch master

## Push upstream feature branch ke origin (github)

`git push -u origin [feature-branch]`

untuk merge branch, silahkan buka github di browser dan bikin pull request kemudian lakukan merge

> kalo ada kesalahan, tolong bilang di group chat
