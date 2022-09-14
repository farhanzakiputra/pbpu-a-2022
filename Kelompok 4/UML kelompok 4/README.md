## Pengembangan Beroritentasi Penggunaan Ulang

**Kelompok 4**

1. 215150409111010 M.FAHMI ARESHA
2. 215150409111016 FAIZ AL QURNI
3. 205150401111024 Nur Izzah Maula Ramadhani
4. 205150401111029 Syahra Rizkia Andina

## Penjelasan UML Diagram

### Store

**Class Store memiliki atribut**
| Name | Type Data |
| ----------- | ----------- |
| namaToko | String |
| namaProduk | String |
| tipeProduk | String |
| beratProduk | Float |
| harga | Double |
| pembeli | String |
| ekspedisi | String[] |
| asal | String |
| tujuan | String |

**Methode yang terdapat pada class Store**
| Name | Type | Description |
| ----------- | ----------- | ----------- |
| shippingRate | void | Melakukan pengecekan tarif pengiriman produk yang ingin dibeli pembeli berdasarkan attribute tipe produk, alamat asal dan tujuan serta berat dari produk yang ingin dibeli menggunakan akses methode melalui interface|
| requestSend | void | Melakukan request pengiriman produk berdasarkan attribute yang terdapat pada class **Store**, serta menggunakan interface request pengiriman untuk melakukan permohonan pengiriman melalui ekspedisi yang dipilih |

### DeliveryAPI

<h3 style="text-align: justify">
Class DevelieryApi merupakan interface. interface adalah penghubung antar objek. Interface bersifat abstrak, Class ini memiliki relasi Extension, sehingga method tersebut harus di implementasikan dalam kelas turunannya. Dalam kasus ini class tersebut di implementasikan untuk jasa pengiriman yaitu JNE, Sicepat dan JNT. class ini terdiri dari 2 method yaitu: </h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>

### SiCepat

<h3 style="text-align: justify">
Class SiCepat merupakan sebuah class yang memiliki beberapa atribut. Atribut- atribut tersebut adalah idPengiriman, alamatPenerima, tanggalPengiriman, namaPengirim , namaPenerima, jenisProduk, berat, statusPengiriman. Class ini pula mengimplemantasi method dari interface DeliveryAPI yaitu :</h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>

### JNE

<h3 style="text-align: justify">
Class JNE merupakan sebuah class yang memiliki beberapa atribut. Atribut- atribut tersebut adalah idPengiriman, alamatPenerima, tanggalPengiriman, namaPengirim, namaPenerima, jenisProduk, berat, statusPengiriman. Class ini pula mengimplemantasi method dari interface DeliveryAPI yaitu :</h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>

### JNT

<h3 style="text-align: justify">
Class JNT merupakan sebuah class yang memiliki beberapa atribut. Atribut- atribut tersebut adalah idPengiriman, alamatPenerima, tanggalPengiriman, namaPengirim , namaPenerima, jenisProduk, berat, statusPengiriman. Class ini pula mengimplemantasi method dari interface DeliveryAPI yaitu :</h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>

## Relationship Class

### Class Store dengan Interface DeliveryAPI 
<ol style="text-align: justify">
Class Store dengan Interface DeliveryAPI memiliki hubungan asosiasi yang artinya adalah setiap objek memiliki siklus hidupnya sendiri dan tidak memiliki ownership. Hubungan asosiasi ini menunjukkan jalur komunikasi sehingga satu objek dapat mengirim pesan ke yang lain. Asosiasi class Store dapat berinteraksi dengan class jasa pengiriman (jne, jnt, siCepat) menggunakan method-methodnya, tetapi hanya dengan jasa pengiriman yang telah mengimplementasikan interface DeliveryAPI.
</ol>

### Class Interface DeliveryAPI dengan class Sicepat, JNT, dan JNE
<ol style="text-align: justify">
Ketiga class jasa pengiriman, yaitu Sicepat, JNT, JNE dengan class Interface DeliveryAPI memiliki hubungan inheritance (pewarisan). Di sini, class DeliveryAPI berperan menjadi superclass dan class Sicepat, JNT, serta JNE berperan sebagai subclass. Subclass di sini harus memiliki method yang ada pada DeliveryAPI untuk mengimplementasikan interfacenya.
</ol>
