# Penjelasan UML Diagram Kelompok 5

#### Shipment
Shipment merupakan komponen utama untuk menciptakan composition Order sehingga dengan tidak adanya Shipment maka tidak ada order

#### Order
Order bertujuan untuk mendapatkan informasi customer melalui Shipment

#### APIdelivery
APIdelivery merupakan class interface yanng memiliki 3 atribut dan 2 method public, yaitu: reqPengiriman dan tarifPengiriman
1. reqPengiriman merupakan method yang digunakan untuk menerima request pengiriman yang dilakukan pada class Shipment
2. tarifPengiriman merupakan method yang digunakan untuk melakukan perhitungan tarif pengiriman sesuai dengan jarak pengirim dan penerima

#### JNE
JNE merupakan pengimplementasian dari kelas interface APIdelivery yang memiliki atribut dan method yang sama dengan kelas APIdelivery

#### JNT
JNT merupakan pengimplementasian dari kelas interface APIdelivery yang memiliki atribut dan method yang sama dengan kelas APIdelivery

#### SiCepat
SiCepat merupakan pengimplementasian dari kelas interface APIdelivery yang memiliki atribut dan method yang sama dengan kelas APIdelivery
