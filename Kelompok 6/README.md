# Pengembangan Beroritentasi Penggunaan Ulang Kelompok 6
![diagram plantUML](//www.plantuml.com/plantuml/png/lLF1JiCm3BtdAwoTDi4cSQquJ88Ts06cRJ_WjQQOnMv9d1FmxmHKKOhAaTxY9-Szlpnd7Gs39V6ErIWyOabmjyM8EzAQ0migl3guU69BMZzeVUOmhvfqyWJF6F1y2Lrree2soAr6dzVsz98esew48Yhg_9OCsN_NKBMB0lOKsRqxLtgC4JPb8qAXf2_9hCJIqVJJZF7q32EJSpK42s2rZ2iA5d2mm5fFPN1xl_dlruIVQiVfiZlm3RLeazZhzsHsjLhDOBdi3iEadHlMSFsMEtC6V-37KRmpDhvWBAqd8RNu-zUuDMcLn7y0)
## 1. Interface IJasaPengiriman
Merupakan sebuah interface yang terdiri dari metode hitungOngkir yang berfungsi untuk menghitung ongkos kirim berdasarkan jarak pengiriman dan berat barang yang akan dikirim. Kemudian, terdapat metode terimaRequestPengiriman untuk menerima request pengiriman dari E-Commerce atau sumber lainnya dengan parameter berupa DetailPemesanan dan akan mereturn Resi.
## 2. Kelas Ecommerce
Merupakan kelas yang merepresentasikan E-commerce seperti Shopee, Tokopedia, dan lain sebagainya. Kelas ini memiliki metode kirimRequestPengiriman dengan parameter DetailPemesanan untuk mengirim request pengiriman ke JasaPengiriman.
