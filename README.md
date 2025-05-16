# Attrition Uncovered: Menggali Akar Masalah Karyawan Keluar di Perusahaan Jaya Jaya Maju

## Proyek: Menyelesaikan Permasalahan Human Resources

### Business Understanding

Perusahaan fiktif "Jaya Jaya Maju" bergerak di bidang edutech dan saat ini menghadapi tantangan serius dalam hal retensi karyawan. Tingkat attrition (karyawan keluar) mencapai 16,9%, jauh di atas ambang batas ideal (<10%). Tingginya attrition ini dapat menghambat produktivitas, meningkatkan biaya rekrutmen, serta memengaruhi stabilitas dan pertumbuhan perusahaan.

### Permasalahan Bisnis

* Mengapa tingkat attrition di perusahaan ini sangat tinggi?
* Apakah attrition terkonsentrasi di departemen tertentu?
* Apakah faktor-faktor seperti lembur (overtime), work-life balance, atau gender turut berkontribusi terhadap keputusan karyawan untuk keluar?

### Cakupan Proyek

* Menganalisis data HR perusahaan untuk mencari pola dan penyebab utama attrition.
* Menyajikan temuan dalam bentuk dashboard interaktif menggunakan Google Looker Studio.
* Memberikan insight dan rekomendasi berdasarkan hasil analisis data.

### Persiapan

**Sumber data:**
Dataset HR fiktif yang berisi informasi 1.058 karyawan, termasuk data attrition, departemen, gender, overtime, dan lainnya.
> link sumber dataset => https://github.com/dicodingacademy/dicoding_dataset/tree/main/employee

**Setup environment:**

* Dengan Anaconda
```bash
conda create --name attrition-analysis python=3.9
conda activate attrition-analysis
pip install -r requirements.txt
```

* Dengan Shell / Terminal (tanpa conda)
```bash
# Buat folder proyek
mkdir attrition_uncovered
cd attrition_uncovered
# Buat dan aktifkan virtual environment
python -m venv venv
source venv/bin/activate  # Gunakan venv\Scripts\activate jika kamu memakai Windows
# Instalasi dependensi
pip install -r requirements.txt
```

### Business Dashboard

Dashboard interaktif dibangun untuk menampilkan metrik-metrik utama, seperti:

1. **Total Karyawan:** 1.058 orang
2. **Karyawan Keluar:** 179 orang
3. **Persentase Attrition:** 16,9%
4. **Attrition Berdasarkan Departemen:**

   * R\&D memiliki jumlah attrition tertinggi
   * Diikuti oleh Sales dan Human Resources
5. **Attrition Berdasarkan Gender:**

   * Laki-laki: 58,6%
   * Perempuan: 41,4%
6. **Attrition Berdasarkan Work Life Balance:**

   * Skor 3 memiliki angka attrition tertinggi
7. **Attrition Berdasarkan Overtime:**

   * Karyawan yang lembur (overtime = Yes) lebih banyak keluar dibanding yang tidak
  
> Dashboard dapat diakses melalui Looker Studio online => https://lookerstudio.google.com/reporting/5d0199fb-6605-4500-8c81-811e544efc88

### Conclusion

Analisis menunjukkan bahwa tingkat attrition tinggi di Jaya Jaya Maju terutama terkonsentrasi di departemen R\&D dan Sales. Faktor seperti lembur berlebihan dan work-life balance yang tidak optimal berperan penting dalam keputusan karyawan untuk keluar. Ini menjadi peringatan bagi manajemen untuk segera mengambil tindakan korektif.

### Rekomendasi Action Items (Optional)

**1. Audit Lingkungan Kerja di Departemen R&D dan Sales**
Data menunjukkan bahwa R&D memiliki jumlah attrition tertinggi, disusul oleh Sales. Perusahaan perlu meninjau ulang beban kerja, gaya kepemimpinan, serta kepuasan kerja di dua departemen ini, karena tingginya angka keluar dapat mengganggu produktivitas dan inovasi.

**2. Tinjau Kebijakan Lembur (Overtime)**
Attrition lebih tinggi pada karyawan yang lembur dibandingkan yang tidak. Hal ini mengindikasikan beban kerja yang berlebih. Disarankan agar perusahaan menyeimbangkan target dengan kapasitas kerja karyawan, dan menyediakan kompensasi yang adil atau fleksibilitas jam kerja.

**3. Fokus Perbaikan pada Karyawan dengan Work Life Balance Skor 3**
Skor 3 justru mencatatkan angka attrition tertinggi, bukan skor rendah seperti yang diharapkan.Ini bisa menandakan bahwa meski terlihat “cukup”, persepsi work-life balance masih belum optimal. Program peningkatan kualitas hidup seperti mental health support, fleksibilitas, atau pengurangan beban kerja bisa sangat efektif.

**4. Kembangkan Strategi Retensi Berdasarkan Gender**
Attrition lebih banyak terjadi pada pria (~58.6%) dibanding wanita (~41.4%). Walaupun distribusi relatif seimbang, pendekatan retensi bisa dipersonalisasi agar lebih efektif, misalnya program mentoring atau penyesuaian benefit berdasarkan kebutuhan dominan masing-masing kelompok.

**5. Bangun Sistem Feedback Berbasis Data untuk Pencegahan Attrition**
Tingginya attrition di beberapa kelompok menunjukkan perlunya pemantauan lebih awal.Disarankan membuat survei kepuasan berkala, indikator early-warning berbasis data HRIS, serta sistem exit interview yang lebih terstruktur agar perusahaan dapat merespons masalah sebelum karyawan memutuskan keluar.

---

