## Flow Development

### Jika belum di-clone repositorinya

pindah ke direktori/folder yang diinginkan didalamnya repositori ini 

`cd ...`

clone repositori

`git clone https://github.com/Panitia-probation/belajar-git`

`cd belajar-git/`

### Branch development

untuk update yang kecil/minor, bisa langsung update branch master

untuk menambah suatu fitur, jangan sampai memodifikasi di branch `master`. silahkan pindah ke suatu branch fitur, dulu:

jika fitur itu belum ada branch-nya di github, silahkan bikin branch baru dengan mengklik _New branch_ di link https://github.com/Panitia-probation/belajar-git/branches

update repositori lokal dengan yang ada di github 

`git fetch origin`

pindah ke feature-branch dari origin

`git checkout origin/[feature-branch]`

buat branch lokal baru jika belum ada

`git branch [feature-branch]`

pindah ke branch yang sudah ada jike belum

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
