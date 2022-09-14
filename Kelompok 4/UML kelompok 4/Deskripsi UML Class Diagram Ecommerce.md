## DeliveryAPI

<h3 style="text-align: justify">
Class DevelieryApi merupakan interface. interface adalah penghubung antar objek. Interface bersifat abstrak, Class ini memiliki relasi Extension, sehingga method tersebut harus di implementasikan dalam kelas turunannya. Dalam kasus ini class tersebut di implementasikan untuk jasa pengiriman yaitu JNE, Sicepat dan JNT. class ini terdiri dari 2 method yaitu: </h3>
<ol style="text-align: justify">
  <li>+tarifPengiriman(jarak,berat): Int. Method ini digunakan untuk memasukkan tarif pengiriman dengan parameter jarak dan berat bertype integer.</li>
  <li>+requestPengiriman(asal,tujuan) : String. Method ini digunakan untuk mengirimkan pengiriman dengan parameter asal dan tujuan bertype String.</li>
</ol>
