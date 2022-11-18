# Istilah dalam Git

### Basic Snapshotting

  * **Working Directory**: direktori kerja, tempat dimana kita bekerja
  * **Staging Area**: area staging, tempat dimana kita menambahkan file yang akan di-commit
  * **Repository**: repositori, tempat dimana kita menyimpan file yang sudah di-commit

### The Three States

  * **Modified**: file yang sudah diubah, belum di-staging
  * **Staged**: file yang sudah di-staging, belum di-commit
  * **Committed**: file yang sudah di-commit, sudah tersimpan di-repositori

### The Life Cycle of File Status

  * **Untracked**: file yang belum di-track oleh Git
  * **Unmodified**: file yang sudah di-track oleh Git, belum diubah
  * **Modified**: file yang sudah di-track oleh Git, sudah diubah
  * **Staged**: file yang sudah di-track oleh Git, sudah diubah dan sudah di-staging

### Remote Repositories

  * **Remote**: repositori yang berada di komputer lain
  * **Origin**: nama default untuk remote repository

### Branches

  * **Branch**: cabang, tempat dimana kita bekerja
  * **Master**: cabang utama, cabang yang di-clone dari remote repository
  * **HEAD**: posisi terakhir yang kita bekerja

### Merging
  * **Merge**: menggabungkan cabang yang berbeda
  * **Fast-forward**: proses merge yang tidak menghasilkan konflik

### Stashing
  * **Stash**: menyimpan perubahan yang belum di-commit
  * **Stash List**: daftar perubahan yang belum di-commit

## Git Commands

### Basic Snapshotting

  * `git init`: membuat repository baru
  * `git add <directory/file.extension>`: menambahkan file ke staging area
  * `git commit -m "message"`: menyimpan file ke repository

### The Three States
  * `git status`: menampilkan status file
  * `git diff`: menampilkan perubahan yang belum di-staging
  * `git diff --staged`: menampilkan perubahan yang belum di-commit

### The Life Cycle of File Status
  * `git rm <file.extension>`: menghapus file dari repository
  * `git mv <file.extension> <new_file.extension>`: mengubah nama file

### Remote Repositories
  * `git clone <url>`: meng-clone repository dari remote
  * `git remote`: menampilkan remote repository

### Branches
  * `git branch`: menampilkan cabang
  * `git branch <branch_name>`: membuat cabang baru
  * `git checkout <branch_name>`: berpindah ke cabang yang dituju
  * `git merge <branch_name>`: menggabungkan cabang yang dituju ke cabang yang sedang aktif
  * `git branch -d <branch_name>`: menghapus cabang yang dituju

### Merging
  * `git log --graph`: menampilkan log dalam bentuk grafik
  * `git log --oneline`: menampilkan log dalam bentuk satu baris

### Stashing
  * `git stash`: menyimpan perubahan yang belum di-commit
  * `git stash list`: menampilkan daftar perubahan yang belum di-commit
  * `git stash apply`: mengembalikan perubahan yang belum di-commit
  * `git stash drop`: menghapus perubahan yang belum di-commit

### Undoing Things
  * `git reset HEAD <file.extension>`: menghapus file dari staging area
  * `git checkout -- <file.extension>`: mengembalikan file ke kondisi terakhir yang sudah di-commit
  * `git reset --hard <commit>`: mengembalikan file ke kondisi pada commit yang dituju
  * `git revert <commit>`: membuat commit baru yang mengembalikan kondisi file pada commit yang dituju

### Ignoring Files
  * `.gitignore`: file yang berisi daftar file yang tidak akan di-track oleh Git

### Viewing the Commit History
  * `git log`: menampilkan log
  * `git log --oneline`: menampilkan log dalam bentuk satu baris
  * `git log --graph`: menampilkan log dalam bentuk grafik
  * `git log --oneline --graph --all`: menampilkan log dalam bentuk satu baris, grafik, dan semua cabang

### Search
  * `git grep <keyword>`: mencari kata kunci di seluruh file

### Rewriting History
  * `git commit --amend`: mengubah pesan commit terakhir
  * `git rebase -i <commit>`: mengubah urutan commit

### Working with Remotes
  * `git push <remote> <branch>`: mengirim perubahan ke remote repository
  * `git pull <remote> <branch>`: mengambil perubahan dari remote repository

### Tagging
  * `git tag`: menampilkan tag
  * `git tag <tag_name>`: membuat tag baru
  * `git tag -a <tag_name> -m "message"`: membuat tag baru dengan pesan
  * `git tag -d <tag_name>`: menghapus tag
  * `git push <remote> <tag_name>`: mengirim tag ke remote repository
  * `git push <remote> --tags`: mengirim semua tag ke remote repository

### Aliases
  * `git config --global alias.<alias_name> <command>`: membuat alias

---

## References:
* [git-scm](https://git-scm.com/docs)
* [Cloud Engineering with Imre](https://yt.wkwkwk.fun/watch?v=KGSfUgaiVNI)