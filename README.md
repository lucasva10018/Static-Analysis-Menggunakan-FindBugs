# Static-Analysis-Menggunakan-FindBugs


Pembahasan   :

Judul :
Static Analysis Menggunakan FindBugs.

Langkah-langkahnya :

Masuk ke CMD, dan berikan perintah sbb :

Microsoft Windows XP [Version 5.1.2600]
(C) Copyright 1985-2001 Microsoft Corp.

C:\Documents and Settings\Student>  ant -version
Apache Ant(TM) version 1.8.2 compiled on December 20 2010
= Perintah untuk memeriksa instalan apache ant,  kalau sudah benar instalnya maka shell akan mengenali ant yang telah terinstal tersebut,hasilnya akan menampilkan tanggal,bulan, dan tahun instalanya seperti ini  : Apache Ant(TM) version 1.8.2 compiled on December 20 2010

C:\Documents and Settings\Student>  cd "My documents"
= Perintah untuk menggunakan atau masuk pada memori yang berada di “My documen”

C:\Documents and Settings\Student\My Documents>  cd Pertemuan4
=  Perintah untuk menggunakan atau masuk ke dalam data dengan memanggil data Pertemuan4

C:\Documents and Settings\Student\My Documents\Pertemuan4>
C:\Documents and Settings\Student\My Documents\Pertemuan4>  ant clean
= Perintah ant clean diatas berfungsi untuk membersihkan pada build sebelum dilakukan compile.

Buildfile: C:\Documents and Settings\Student\My Documents\Pertemuan4\build.xml

clean:
     [echo] Cleaning and creating new directory
   [delete] Deleting directory C:\Documents and Settings\Student\My Documents\Pe
rtemuan4\classes
    [mkdir] Created dir: C:\Documents and Settings\Student\My Documents\Pertemua
n4\classes

BUILD SUCCESSFUL
Total time: 0 seconds

C:\Documents and Settings\Student\My Documents\Pertemuan4>  ant compile
= Perintah ant compile  diatas berfungsi untuk compile build tadi yang telah debersihkan dengan melakukan ant clean sebelum ant compile tadi.

Buildfile: C:\Documents and Settings\Student\My Documents\Pertemuan4\build.xml

clean:
     [echo] Cleaning and creating new directory
   [delete] Deleting directory C:\Documents and Settings\Student\My Documents\Pe
rtemuan4\classes
    [mkdir] Created dir: C:\Documents and Settings\Student\My Documents\Pertemua
n4\classes

compile:
     [echo] compiling all vehicles and tests classes
    [javac] C:\Documents and Settings\Student\My Documents\Pertemuan4\build.xml:
16: warning: 'includeantruntime' was not set, defaulting to build.sysclasspath=l
ast; set to false for repeatable builds
    [javac] Warning: vehicles\BicycleMain.java modified in the future.
    [javac] Compiling 2 source files to C:\Documents and Settings\Student\My Doc
uments\Pertemuan4\classes

BUILD SUCCESSFUL
Total time: 1 second

C:\Documents and Settings\Student\My Documents\Pertemuan4>  ant findbugs
= Perintah ant finddebugs  diatas berfungsi untuk menmpilkan kesalahan atau error pada project  atau skript juga bisa berfungsi sebagai analisis static,Compiler hanya akan memeriksa error yang bersifat sintaksis .

Buildfile: C:\Documents and Settings\Student\My Documents\Pertemuan4\build.xml

clean:
     [echo] Cleaning and creating new directory
   [delete] Deleting directory C:\Documents and Settings\Student\My Documents\Pe
rtemuan4\classes
    [mkdir] Created dir: C:\Documents and Settings\Student\My Documents\Pertemua
n4\classes

compile:
     [echo] compiling all vehicles and tests classes
    [javac] C:\Documents and Settings\Student\My Documents\Pertemuan4\build.xml:
16: warning: 'includeantruntime' was not set, defaulting to build.sysclasspath=l
ast; set to false for repeatable builds
    [javac] Warning: vehicles\BicycleMain.java modified in the future.
    [javac] Compiling 2 source files to C:\Documents and Settings\Student\My Doc
uments\Pertemuan4\classes

findbugs:
 [findbugs] Executing findbugs from ant task
 [findbugs] Running FindBugs...
 [findbugs] Calculating exit code...
 [findbugs] Exit code set to: 0
 [findbugs] Output saved to findbugs-results.txt

BUILD SUCCESSFUL
Total time: 7 seconds

Selesai.
