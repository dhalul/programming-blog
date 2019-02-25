---
layout: post
title:  "C/C++ (Compiler)"
author: dhal
categories: [ c, c++, compiler ]
image: assets/images/cpp/compiler.jpg
featured: true
hidden: false
table: true
---

>C (/siː/, as in the letter c) is a general-purpose, imperative computer programming language, supporting structured programming, lexical variable scope and recursion, while a static type system prevents many unintended operations. By design, C provides constructs that map efficiently to typical machine instructions, and therefore it has found lasting use in applications that had formerly been coded in assembly language, including operating systems, as well as various application software for computers ranging from supercomputers to embedded systems.

>C++ (/ˌsiːˌplʌsˈplʌs/ "see plus plus") is a general-purpose programming language. It has imperative, object-oriented and generic programming features, while also providing facilities for low-level memory manipulation.

>Sumber : Wikipedia

<hr/>

## C / C++ Compiler

C / C++ punya banyak variasi tergantung dari compiler yang kita gunakan. Compiler yang paling umum digunakan adalah GCC/C. Selain itu masih banyak compiler lain yang bisa teman teman coba (link ada pada postingan sebelumnya) seperti Microsoft Visual C++, Borland C, QuickC dan lain lain. Setiap compiler memiliki perbedaan sendiri baik dari segi library yang bisa kita gunakan serta penulisan syntax yang sedikit berbeda, seperti Visual C++, kita bisa menggunakan library, Windows API, Direct X, .NET yang tidak memungkinkan jika kita menggunakan library tersebut dan melakukan compile dengan compiler lain, karena library tersebut merupakan library spesifik yang disediakan oleh Microsoft. Visual C++ yang sekarang menjadi Visual Studio termasuk dalam kategori proprietary software atau software yang memiliki kepemilikan (owner) dan biasanya untuk menggunakan ini kita harus mengeluarkan biaya tertentu untuk dibayarkan kepawa owner.

Jadi dalam hal pemilihan compiler tergantung dari keperluan kita terhadap software yang akan kita buat.

Untuk penggunaan umum (seperti pembelajaran), melakukan input output data, operasi aritmetika, fungsi dan lain lain kita bisa memanfaatkan Compiler C/C++ yang tersebar secara gratis dan benar benar gratis yaitu GCC (GNU Compiler Collection) yang disediakam oleh GNU. GCC sendiri merupakan kumpulan dari beberapa Compiler untuk berbagai bahasa seperti : gcc untuk bahasa c, g++ untuk c++, gfortran untuk fortran, gccgo untuk bahasa Go dan lain lain.

Di operating system berbasis Linux sendiri biasanya sudah tersedia GCC dari bawaan sedangkan operating system lain kita diharuskan untuk menggunakan aplikasi pihak ketiga.

    + Untuk Windows :
    Windows tidak memiliki compiler bawaan untuk bahasa C/C++. Adapun beberapa compiler yang bisa digunakan adalah MinGW, WSL dan Cygwin.

        - MinGW (Minimalist GNU for Windows) merupakan software hasil portingan dari GNU GCC, GNU BinUtils dan beberapa native library lain yang bisa kita pakai untuk dapat menggunakan beberapa API dari OS Windows.
        MinGW sendiri memiliki 2 versi yaitu :
            * MinGW, yang merupakan port GCC secara langsung ke Windows. Tidak semua Windows API di support oleh compiler ini (tetapi untuk kebanyakan penggunan, itu sudah lumayan cukup) dan compiler ini hanya mendukung program 32-bit (Program hasil compile tetap bisa berjalan di Windows berbasis 64-bit, tetapi ada kemungkinan beberapa tidak bisa, dan kita tidak bisa melakukan compile program menjadi 64-bit)
            * MinGW-w64, adalah Pengembangan dari MinGW yang support 32-bit dan 64-bit, dan mendukung lebih banyak Windows API (Tidak semua, tetapi hampir semua dapat bekerja dengan lebih baik dari MinGW).<br/>

            Dari beberapa penjelasan yang saya baca dari Forum, MinGW sudah tidak dikembangkan lagi. MinGW-w64 merupakan hasil fork dari MinGW (Pengembangan dari Source Code asli MinGW) dan masih tetap di maintain sampai sekarang.

        - Sedangkan Cygwin sendiri adalah software yang digunakan untuk dapat menggunakan aplikasi berbasis UNIX, serta membuat windows agar terlihat seperti benar benar terdapat pada lingkungan UNIX. Jadi pada Cygwin software yang dilakukan portingan bukan hanya GCC tetapi juga beberapa aplikasi lain.

        - Windows Subsystem for Linux merupakan fitur yang telah disediakan oleh Microsoft pada Operating System nya yaitu Windows. Kita bisa menghidupkan opsi ini dengan mencari "Turn Windows features on or off" kemudian pada kolom dialog cari "Windows Subsystem for Linux" dibagian bawah, setelah itu ceklis kemudian klik OK.

        <center><img src="https://programming.my.id/assets/images/cpp/wsl/feature-wsl.png" width="70%"/></center>

        Jika anda ingin sekalian merasakan pengalaman menggunakan lingkungan UNIX (seperti menggunakan linux) maka silahkan menginstall Cygwin/Windows Subsystem for Linux atau silahkan menginstall linux sekalian. Tapi jika anda hanya ingin menggunakan Compiler GCC maka ada baiknya anda menginstall MinGW/MinGW-w64 saja.

    - Link Download untuk MinGW
    - Link Download untuk Cygwin

    Tahapan install MinGW : 

    Untuk Mac

    Mac :