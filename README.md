# ProjectKelompok_8

# --- TAHAP 1: CLONE REPOSITORY HASIL FORK ---
git clone https://github.com/USERNAME_ANDA/NAMA_REPO.git
cd ProjectKelompok_8

# --- TAHAP 2: PEMBUATAN BRANCH BARU ---
git checkout -b feature/tugas-aol

# --- TAHAP 3: EDIT FILE & COMMIT ---
# (Asumsi membuat file baru untuk tugas)
echo "Kontribusi dari USERNAME_ANDA" >> kontribusi.txt
git add .
git commit -m "feat: tambahkan file kontribusi anggota kelompok"

# --- TAHAP 4: MERGE DENGAN NO FAST-FORWARD ---
# Pindah ke branch utama untuk melakukan penggabungan
git checkout main

# Eksekusi merge manual dengan flag --no-ff
git merge --no-ff feature/tugas-aol -m "merge: gabungkan feature/tugas-aol ke main (non-fast-forward)"

# --- TAHAP 5: PUSH KE REPOSITORY FORK ---
git push origin main

# --- TAHAP 6: VERIFIKASI HISTORY (OPTIONAL) ---
git log --graph --oneline --all

  
   
