## DeliveryAPI

<h3 style="text-align: justify">
Class DevelieryApi merupakan interface. interface adalah penghubung antar objek. Interface bersifat abstrak, Class ini memiliki relasi Extension, sehingga method tersebut harus di implementasikan dalam kelas turunannya. Dalam kasus ini class tersebut di implementasikan untuk jasa pengiriman yaitu JNE, Sicepat dan JNT. class ini terdiri dari 2 method yaitu: </h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>

## SiCepat

<h3 style="text-align: justify">
Class SiCepat merupakan sebuah class yang memiliki beberapa atribut. Atribut- atribut tersebut adalah idPengiriman, alamatPenerima, tanggalPengiriman, namaPengirim , namaPenerima, jenisProduk, berat, statusPengiriman. Class ini pula mengimplemantasi method dari interface DeliveryAPI yaitu :</h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>

## JNE

<h3 style="text-align: justify">
Class JNE merupakan sebuah class yang memiliki beberapa atribut. Atribut- atribut tersebut adalah idPengiriman, alamatPenerima, tanggalPengiriman, namaPengirim, namaPenerima, jenisProduk, berat, statusPengiriman. Class ini pula mengimplemantasi method dari interface DeliveryAPI yaitu :</h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>

## JNT

<h3 style="text-align: justify">
Class JNT merupakan sebuah class yang memiliki beberapa atribut. Atribut- atribut tersebut adalah idPengiriman, alamatPenerima, tanggalPengiriman, namaPengirim , namaPenerima, jenisProduk, berat, statusPengiriman. Class ini pula mengimplemantasi method dari interface DeliveryAPI yaitu :</h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>
