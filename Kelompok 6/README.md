# Pengembangan Beroritentasi Penggunaan Ulang Kelompok 6
- SHELLEN WIDYA AZZAHRA 205150400111008
- PUTRY AMAYLIA SUSILOWATI 205150400111048
- SULISTIA NENGSIH 205150400111067
- MEGANANDA DWI FITRIYANI 205150401111028
- MOHAMMAD RAFI AZZAKY 205150407111031
![diagram plantUML](https://github.com/andrisan-ub/pbpu-a-2022/blob/6-uml-kelompok-6/Kelompok%206/PlantUML%20Kel-6.png)
## 1. Interface IJasaPengiriman
Merupakan sebuah interface yang terdiri dari metode hitungOngkir yang berfungsi untuk menghitung ongkos kirim berdasarkan jarak pengiriman dan berat barang yang akan dikirim. Kemudian, terdapat metode terimaRequestPengiriman untuk menerima request pengiriman dari E-Commerce atau sumber lainnya dengan parameter berupa DetailPemesanan dan akan mereturn Resi.
## 2. Kelas Ecommerce
Merupakan kelas yang merepresentasikan E-commerce seperti Shopee, Tokopedia, dan lain sebagainya. Kelas ini memiliki metode kirimRequestPengiriman dengan parameter DetailPemesanan untuk mengirim request pengiriman ke JasaPengiriman.
## 3. Jasa Pengiriman
Jasa Pengiriman merupakan class yang memiliki atribut public idJasaPengiriman yang memiliki tipe data integer, nama dengan tipe data String. Dan terdapat implementasi method dari interface JasaPengiriman yaitu:
1.  **hitungOngkir(double jarak, double berat)**
2.  **terimaRequestPemesanan(DetailPemesanan dp): Resi**
## Penjelasan Relasi Antar Class
### Class JNE, JNT, dan SiCepat dengan Class JasaPengiriman
Hubungan dari class JNE, JNT, dan SiCepat dengan class JasaPengriman adalah mengimplementasikan inheritance yang dimana class JasaPengiriman berperan sebagai parent class dan class JNE, JNT, dan SiCepat berperan sebagai sub class.
