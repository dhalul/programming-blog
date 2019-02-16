---
layout: post
title:  "Apa itu Source Code Management, Version Control atau Revision Control?"
author: dhal
categories: [ editor ]
image: assets/images/github/gituhub-pages.jpg
featured: true
hidden: true
---

>A component of software configuration management, version control, also known as revision control or source control,[1] is the management of changes to documents, computer programs, large web sites, and other collections of information. Changes are usually identified by a number or letter code, termed the "revision number", "revision level", or simply "revision". For example, an initial set of files is "revision 1". When the first change is made, the resulting set is "revision 2", and so on. Each revision is associated with a timestamp and the person making the change. Revisions can be compared, restored, and with some types of files, merged.

>Sumber : Wikipedia

>Nahh, sebelum mulai saya ingin menjelaskan bahwa artikel ini adalah artikel yang saya buat berdasarkan penjelasan yang saya pelajari di
>https://arcadsoftware.com/news-events/blog/what-is-source-code-management/

Menurut Ray Bernadi, Senior Consultant dari ARCAD Software yang dia hidup dimasa System/34 dan System/38 masih berjalan.
Pada masa-masa itu, kontrol source code masih sangat simpel. Jika kita ingin membuat perubahan terhadap source code yang sebelumya kita kerjakan, kita harus membuat salinannya, agar source code asli masih bisa kembalikan ke keadaan semula jika terjadi hal-hal yang tidak diinginkan.

Tentu saja, dengan cara seperti itu menimbulkan sedikit masalah. Code Regression merupakan salah satu masalah tersebut. Code Regression adalah masalah yang timbul ketika terjadi perubahan source code sebuah program, dimana kita harus memastikan bahwa program lama masih bisa bekerja dengan perubahan source code yang kita lakukan. Nah, kita coba buat contoh satu masalah. Ketika Satu Programmer  ingin membuat perubahan terhadap source code asli, dan dia melakukan backup source code asli. Kemudian semalaman ia melakukan perubahan, atau peningkatan terhadap source code sebelumnya. Esoknya, ia bertemu dengan sesama Programmer kedua dari Perusahaan yang sama dengan dia. Nah Programmer kedua ini rupanya melakukan perubahan terhadap source code juga. Yang menjadi masalah adalah tentu saja apa yang dia ubah menimpa apa yang dibuat oleh Programmer pertama, begitu juga sebaliknya. Programmer kedua tentu saja mulai melakukan perubahan dibaris yang sama dengan yang dimulai oleh Programmer pertama.

Memang tentu saja hal itu dapat dihindari dengan pembagian tugas atau sejenisnya, tetapi untuk menggabungkan setiap perubahan dari beberapa programmer bukan menjadi hal yang mudah. Jadi, dapat kita simpulkan bahwa membuat salinan belumlah cukup.