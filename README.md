# Pokemon-API-Groovy-JMeter-FinalProject-EdwardWidjanarko

# Uji POKEMON API dengan Apache JMeter

  Proyek ini menunjukkan cara menggunakan Apache JMeter untuk menguji API Pokemon (pokeapi.co/api/v2/pokemon-species?offset=0&limit=20). 
  Skenario pengujian melibatkan pengiriman permintaan HTTP ke API Pokemon dan melakukan validasi terhadap respons yang diterima.
  
# Persyaratan ==>
  Sebelum menjalankan uji, pastikan Anda telah menginstal perangkat lunak berikut:
    - Apache JMeter
    - Java

# Gambaran Rencana Uji
# Rencana uji JMeter (Pokemon-API-Test.jmx) memiliki struktur sebagai berikut:

    Thread Group:  simulasi pengguna.

    While Controller: Terus menjalankan elemen anak selama suatu kondisi bernilai benar. Dalam hal ini, terus berlanjut hingga Pikachu ditemukan.
    HTTP Request: Mengirim permintaan GET ke API Pokemon untuk mendapatkan informasi tentang spesies Pokemon.
    JSR223 PostProcessor: Mengurai respons JSON untuk memeriksa apakah Pikachu ditemukan. Jika ditemukan, mengatur variabel untuk menghentikan pengulangan; jika tidak,     
    menambahkan nilai offset.

    HTTP Request ke Endpoint Lainnya: Permintaan HTTP tambahan ke endpoint berbeda dalam API Pokemon untuk pengujian lebih lanjut.
    JSR223 PostProcessor untuk Endpoint Tambahan: Serupa dengan post processor pertama, melakukan tindakan berdasarkan respons.
    
    HTTP Request ke Endpoint Lainnya: Permintaan HTTP tambahan ke endpoint berbeda dalam API Pokemon untuk pengujian lebih lanjut.
    JSR223 PostProcessor untuk Endpoint Tambahan: Serupa dengan post processor pertama, melakukan tindakan berdasarkan respons.

    View Results Tree, Table, dan Summary Report: Pendengar berbeda untuk melihat dan menganalisis hasil.

# Cara Menjalankan

   1. Buka Apache JMeter.
   2. Buka program uji (Pokemon-API-Groovy-JMeter-FinalProject-EdwardWidjanarko.jmx).
   3. Klik "Run" untuk memulai test.
   4. Lihat hasilnya.

# Catatan
  Final Project = mungkin masih diperlukan latihan dan penerapan kembali. Mohon doa restu. Amien

# Penulis
