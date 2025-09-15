Catatan Perkuliahan Kapsel Analitika Data PEKAN-2

Proses koneksi Visual Studio Code dengan GitHub:
    Pada terminal Visual Studio Code:
        Tambah Git Bash
            git config --global username "Agnes Yohana"
            git config --global user.email "youremail@mail.com"
                #harus sama dengan email yang terdaftar di GitHub
            ssh-keygen -t ed25519 -C "youremail@mail.com" 
                #SSH key tersimpan di C:\Users \<username>\.ssh\id ed25519.pub
    Pada akun GitHub:
        setting > SSH and GPG keys > New SSH key (ada di ed25519.pub)
    Kembali ke terminal Visual Studio Code:
        ssh -T git@github.com #enter terus
        Ketik yes

Perintah:
pwd #perintah untuk memberi informasi folder apa yang saat itu sedang dibuka
ls #perintah untuk memberi informasi list file apa saja yang ada di folder tersebut
cd /c/... #perintah untuk membuka folder yang ada di folder C
rm -rf #perintah untuk hapus folder beserta semua isinya

Pembuatan Folder:
mkdir #perintah untuk membuat folder
-> jika sudah membuat repository di GitHub, tidak perlu buat folder
-> cukup ketik 
    git clone git@github.com:agnes7209/Kapsel_Analitika_Data-Tugas_1.git
    agar terbentuk folder yang berhubungan dengan repository github

Update file ke GitHub:
git status #Memberi informasi tentang status git

git add . #Menambahkan ke staging area 
    surat masuk ke amplop
git commit -m "komentar atau catatan yang kita berikan untuk orang lain saat melakukan update"
    amplop masuk ke kotak pos
git push origin main
    amplop sampai ke tujuan