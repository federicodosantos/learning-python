# Python

Python merupakan bahasa pemrograman yang sedang populer saat ini. Python dikenal sebagai bahasa pemrograman yang memiliki
syntax yang sangat sederhana dibanding bahasa pemrograman lain.

## How it Works - Intepreter
Bagaimana sebuah program python itu dapat berjalan? Jadi python menggunakan **intepreter** untuk menerjemahkan source code nya agar dapat berjalan di terminal.
**Intepreter** ini akan membaca kode baris per baris dan menerjemahkannya. 

## How it Works - ByteCode
Sebelumnya kita tahu bahwa program python itu dapat dijalankan menggunakan intepreter dengan cara menerjemahkan baris per baris yang ada pada source code.
Bagaimana jika jumlah baris kode dalam satu file itu sangat panjang? Maka penggunaan intepreter disini kurang disarankan
karena membutuhkan waktu yang lebih lama untuk menerjemahkan baris-baris kode tersebut.

Jadi Solusi yang dapat digunakan yaitu dengan mengkompilasi/compiling source code kita. Source code yang kita compile ini nanti akan berbentuk
ByteCode. ByteCode merupakan sekumpulan low level instruction yang merupakan hasil kompilasi dari source code python.
Nantinya file python yang berbentuk bytecode ini akan dijalankan oleh Python Virtual Mesin.
Dengan mengkompilasi source python kita, dapat mempercepat proses eksekusi dibandingkan menjalankan kode python langsung.

## Single and Double Underscore
Underscore dalam python berguna untuk melakukan naming convention entah itu untuk public atau private sebuah kelas, variable dan lainnya.

### Single Underscore(_)
Single underscore biasanya digunakan untuk memberitahu bahwa atribut atau fungsi tersebut private atau hanya dapat digunakan untuk penggunaan internal saja.
Selain itu penggunaan single underscore saja (_) bisa digunakan apabila kita tidak menggunakan nilai return yang dikembalikan oleh sebuah fungsi.

## Double Leading Underscore(__Name)
Double leading underscore biasanya digunakan agar variable sebuah kelas ini tidak dapat dioverride oleh kelas turunannya. Maksudnya jika 
kita memiliki sebuah variabel yang ada kelas parent, kelas child tidak bisa melakukan modifikasi dan bahkan tidak bisa mengaksesnya.
Convention ini dikenal dengan **Name Mangling**.

## Double Leading and Trailing Underscore(__Name__)
Convention ini digunakan untuk membuat **magic method** atau **dunder methods**. Kalau untuk penggunaan dari convention ini biasanya
digunakan untuk mendefinisikan perilaku sebuah kelas, misal construstor, toString method dan sebagainya.