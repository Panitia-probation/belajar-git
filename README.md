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

`git checkout master`

### Jika sudah siap di-merge

`git merge [feature-branch]`

jika ada konflik,

```
Auto-merging main.py
CONFLICT (content): Merge conflict in main.py
Automatic merge failed; fix conflicts and then commit the result.
```

silahkan modifikasi repositori, dalam kasus ini file `main.py` sehingga merge conflict 
solved, kemudian commit lagi (hanya setelah fix conflict) 

`git add -A`

`git commit -m "fixed conflict"`

push upstream repositori lokal ke github

`git push -u origin`

## Jika belum siap di-merge

`git push -u origin [feature-branch]`

> kalo ada kesalahan, tolong bilang di group chat
