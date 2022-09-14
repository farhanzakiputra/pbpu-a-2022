# Pengembangan Beroritentasi Penggunaan Ulang
<h4> Kelompok 1 : </h4>
<ul>
	<li>205150401111020 MUHAMMAD DAVALA SAFA</li>
    <li>205150401111025 MOHAMMAD KEVIN ABDILLAH</li>
    <li>205150400111051 DANIEL DEARY</li>
    <li>205150407111020 ILHAM NUANSA SHAYLENDRA PUTRA PAMUNGKAS</li>
</ul>

## Penjelasan UML Diagrams

### E-Commerce
**Class Ecommerce** memiliki **enam atribut** bersifat public diantaranya atribut bertipe data String yaitu asalPengiriman, tujuanPengiriman, namaPengirim, namaPenerima dan atribut bertipe data double yaitu jarakPengiriman, beratBarang. Class ini juga **memiliki method** bersifat public yaitu setRequestPengiriman(String asalPengiriman, String tujuanPengiriman, String namaPengirim, String namaPenerima) yang digunakan untuk menerima dan memberi nilai request pengiriman dari pengirim, dan method getTarif() yang digunakan untuk mengembalikan nilai tarif yang telah dihitung.

### DeliveryAPI
**Interface deliveryAPI** memiliki **dua atribut bersifat** public dengan tipe data double yaitu hargaPerKm dan hargaPerKg. Interface deliveryAPI memiliki **dua method** yaitu setTarif(Double jarakPengiriman, Double beratBarang) yang digunakan untuk memberikan nilai tarif yang telah dihitung, dan method getRequestPengiriman() digunakan untuk mengembalikan nilai request pengiriman.

### Sicepat
**Class Sicepat** memiliki **tiga atribut** bersifat public dengan tipe data double yaitu tarif, hargaPerKm, hargaPerKm. Class ini memiliki **dua method** yaitu setTarif(Double jarakPengiriman, Double beratBarang), dan method getRequestPengiriman().

### JNT
**Class JNT** memiliki **tiga atribut** bersifat public dengan tipe data double yaitu tarif, hargaPerKm, hargaPerKm. Class ini memiliki **dua method** yaitu setTarif(Double jarakPengiriman, Double beratBarang), dan method getRequestPengiriman().

### JNE
**Class JNE** memiliki **tiga atribut** bersifat public dengan tipe data double yaitu tarif, hargaPerKm, hargaPerKm. Class ini memiliki **dua method** yaitu setTarif(Double jarakPengiriman, Double beratBarang), dan method getRequestPengiriman().

## Relationship Class 

### Class E-Commerce dengan Interface DeliveryAPI 
Hubungan antara class E-Commerce dengan Interface DeliveryAPI adalah asosiasi yang dimana pada dasarnya hubungan asosiasi antara dua objek atau lebih menunjukkan jalur komunikasi (juga disebut tautan) di antara mereka sehingga satu objek dapat mengirim pesan ke yang lain. Asosiasi class E-commerce dapat berinteraksi dengan class jasa pengiriman (jne, jnt, siCepat) menggunakan method-methodnya, tetapi hanya dengan jasa pengiriman yang telah mengimplementasikan interface DeliveryAPI.

### Class Interface DeliveryAPI dengan class Sicepat, JNT, dan JNE
Hubungan antara ketiga class jasa pengiriman yaitu Sicepat, JNT, JNE dan class Interface Delivery API merupakan Inheritance, yang dimana class deliveryAPI berperan menjadi superclass sedangkan class Sicepat, JNT, dan JNE berperan sebagai subclass yang dimana setiap classnya harus memiliki method yang ada pada deliveryAPI untuk mengimplementasikan interfacenya.
