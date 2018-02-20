# OS181
ZCZC Sistem Operasi 2018 Awal (1)
ZCZC Sistem Operasi Week 01
1. a01-READ-ME
   Menampilkan daftar command line
2. a02-sort-n-prepare
    - chmod : memberikan akses kepada user berhak melakukan apa saja sesuai dengan angka yang di define
    - cat : view file yang diinginkan
    - rm -rf : delete direktory yang diinginkan
    - mkdir -p : membuat direktori parent baru 
3. a03
   menampilkan fungsi dari commandline yang ada di dalam program
   - ls :> menampilkan seluruh file dan folder yang ada di dalam current directory
   - ls -a:> menampilkan seluruh file dan  folder termasuk yang hidden yang ada dalam current directory
   - ls -aF:> sama dengan ls -a bedanya, menampilkan letak directory nya dimana
   - ls -al | head -8 ; echo "(...)"; ls -al | tail -8 :> menampilkan seluruh file dan folder termasuk yang hidden beserta totalnya berbentuk daftar. 
							Setiap file dan folder juga dilengkapi keterangan privilege user.
   - ls -a .TESTFROM ; echo ":::::::::" ; ls -aF .TESTFROM:> menampilkan isi dari file dan yang hidden
   - cat .TESTFROM/program2.c :> menampilkan isi dari program2.c yang ada di folder TESTFROM. User hanya bisa melihat isi file
   - cd .TESTFROM ; cat file1.txt ; echo ":::" ; cat file2.txt ; cd ..  :> masuk ke direktori TESTFROM, view file file1.txt, print "::::", view file2.txt lalu kembali ke direktori sebelumnya
   - wc file1.txt :> menampilkan jumlah baris, jumlah kata, jumlah karakter (byte) dalam file1.txt
   - wc -l file1.txt :> menampilkan jumlah baris dalam file1.txt
   - wc -c file1.txt :> menampilkan jumlah karakter (byte) dalam file1.txt
   - date :>  menampilkan hari, tanggal dan jam sekarang
   - date +%y:> menampilkan 2 digit terakhir tahun sekarang
   - date + %Y :> menampilkan tahun sekarang
   - date +%d\ %b\ %Y\ at \ %H:%M:$S; :> menampilkan format date hari sesuai format yang diinginkan
   - top -b -n 1 | head -15 :> menampilkan proses yang berjalan, banyak user, jumlah task. head -15 menampilkan daftar 15 proses teratas yang berjalan
   - tail -7 :> daftar 7 terbawah
   - $MYVAR :> inisiasi sebuah variabel
   - echo :> print
   - printf "PATH=[%s]\nHOME=[%s]\nSHELL=[%s]\n" $PATH $HOME $SHELL : menampilkan path directory, home directory dan shell
   - printf $$ :> prosess id
   - printf $# :> argument bisa juga dengan $1, $2, $3 
   - printf $0 :> program yang sedang dijalankan
   - sleep :> delay untuk periode detik yang ditentukan
   - /bin/bash --version :> gnu bash version yang digunakan
4. a04-loop
   Program yang menampilkan looping inputan dari user. looping diteruskan ke baris selanjutnya
   $@ untuk menerima inputan yang akan di parsing ke variabel string
5. a05-tester
   program test yang check apakah isi dari current directory termasuk file atau directory
6. a06-does-it-exist
   check apakah suatu file ada di dalam current directory
7. a07-finding-EXIST
   Program menampilkan file apa saja yang ada dalam current directory
8. a08-append-a-file
   Program untuk append suatu nilai ke dalam file yang diinginkan, jika file belum ada, maka akan di create.
