Deskripsi project :
- 
Membuat kerangka Web Automation dengan menggunakan Selenium, Cucumber, dan WebDriverManager yang megadopsi konsep Page Object Model (POM). Dengan framework ini, pengujian untuk login, menambah/hapus item dari keranjang belanja, serta menangani pesan kesalahan dapat dilakukan dengan mudah dan efisien.

Cara run project :
-
Tes Positif
- Buka project menggunakan Intellij Idea
- Buka terminal
- Ketik ./gradlew webTest
- Enter
  
Tes Negatif
- Buka project menggunakan Intellij Idea
- Buka terminal
- Ketik ./gradlew webTestNegative
- Enter

Konfigurasi project :
-
1. Struktur Direktori Proyek :

    src/test/java/ :
  - pages/ : Berisi kelas WebPage, berfungsi untuk melakukan aksi pada elemen-elemen halaman web.
  - stepDef/ : Berisi kelas WebStep, berfungsi sebagai step definitions untuk Cucumber.
  - helper/ : Berisi kelas Utility yang mengelola konfigurasi WebDriver.

    src/test/resources/ :
  - features/ : Berisi file fitur Cucumber dalam format .feature, yang mendefinisikan skenario pengujian.
2. Dependensi :
Konfigurasi dependensi untuk Selenium, Cucumber, dan WebDriverManager
![image](https://github.com/user-attachments/assets/689ded4b-edf0-448a-b865-1b404cf58953)

3. Pengaturan Driver Selenium (WebDriverManager):
WebDriverManager digunakan untuk mengelola driver browser secara otomatis dengan konfigurasi sebagai berikut :
![Screenshot 2024-11-28 090034](https://github.com/user-attachments/assets/a16bab78-3766-45fe-878f-816a483a8d95)



Screenshot hasil pengujian tes positif dan negatif :
-
Tes positif : Menguji fungsionalitas login dengan normal user, menambahkan , dan menghapus item dari keranjang
![Screenshot 2024-11-28 091459](https://github.com/user-attachments/assets/8088c5dd-5eee-437f-a28f-a7b3aca01bf7)
![Screenshot 2024-11-28 091517](https://github.com/user-attachments/assets/8ace34b0-560a-4ad9-8ed6-5494c4a5cde0)
![Screenshot 2024-11-28 091534](https://github.com/user-attachments/assets/a8950d4f-be80-473c-a0c2-affa4adf61f6)
![Screenshot 2024-11-28 091543](https://github.com/user-attachments/assets/4019d61a-f359-45aa-a602-e95997d6fd32)

Tes negatif : Menguji fungsionalitas login dengan locked user
![Screenshot 2024-11-28 091650](https://github.com/user-attachments/assets/2cce756f-eace-4200-b2e3-00d411d1f3ca)
![Screenshot 2024-11-28 091701](https://github.com/user-attachments/assets/0c5bd568-59e0-4d78-82db-bfdf9942698b)

GitHub Actions Workflow
![Screenshot 2024-11-29 084052](https://github.com/user-attachments/assets/5acec1e7-672c-40eb-a990-ab8d6188c8f0)









