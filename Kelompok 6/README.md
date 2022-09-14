# Pengembangan Beroritentasi Penggunaan Ulang Kelompok 6
![diagram plantUML](https://github.com/andrisan-ub/pbpu-a-2022/blob/6-uml-kelompok-6/Kelompok%206/PlantUML%20Kel-6.png)
## 1. Interface IJasaPengiriman
Merupakan sebuah interface yang terdiri dari metode hitungOngkir yang berfungsi untuk menghitung ongkos kirim berdasarkan jarak pengiriman dan berat barang yang akan dikirim. Kemudian, terdapat metode terimaRequestPengiriman untuk menerima request pengiriman dari E-Commerce atau sumber lainnya dengan parameter berupa DetailPemesanan dan akan mereturn Resi.
## 2. Kelas Ecommerce
Merupakan kelas yang merepresentasikan E-commerce seperti Shopee, Tokopedia, dan lain sebagainya. Kelas ini memiliki metode kirimRequestPengiriman dengan parameter DetailPemesanan untuk mengirim request pengiriman ke JasaPengiriman.
## Penjelasan Relasi Antar Class
### Class JNE, JNT, dan SiCepat dengan Class JasaPengiriman
Hubungan dari class JNE, JNT, dan SiCepat dengan class JasaPengriman adalah mengimplementasikan inheritance yang dimana JasaPengiriman berperan sebagai parent class dan class JNE, JNT, dan SiCepat berperan sebagai sub class.
