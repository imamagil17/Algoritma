#Imam Agil Aiman
#F55123066
# Algoritma

#Analisis Quiz 2


Analisis Best Case pada Naive dengan menggunakan Bubble Sort
Base Case dapat terjadi karena ketika data sudah sepenuhnya terurut, yang dimana ketika dalam kondisi ini, algoritma tidak perlu melakukan pertukaran elemen, sehingga hanya memeriksa pasangan elemen tanpa memodifikasi array-nya, langkahnya dimulai dari bubble sort melakukan iterasi melalui array yang dimana pada setiap iterasi, membandingkan elemen bersebelahan dan tidak ada pertukaran dilakukan jika elemen-elemen sudah dalam urutan yang benar, proses berlanjut hingga seluruh array diperiksa. Komplesitas yang ada dalam Best Case, waktunya jika tanpa di optimasi, algoritma tetap akan melakukan "n x (n-1) / 2" perbandingan, menghasilkan O(n2), bahkan dalam kondisi base case, dengan optimisasi (flag), hanya diperlukan satu iterasi penuh, menghasilkan kompleksitas waktu O(n). Ruangnya jika kompleksitas ruang tetap O(1) karena sorting dilakukan in-place tanpa alokasi tambahan.


Analisis Base Case pada Conquer dengan menggunakan Merge Sort
Base casenya terjadi karena data yang sudah terturut secara keseluruhan, meskipun array sudah terurut, algoritma tetap harus membagi array menjadi subarray dan menggabungkan kembali, dengan begitu merge sort akan selalu memiliki kompleksitas waktu O(n log n), bahkan dalam base case-nya. Dengan melakukan pembagian, array dibagi menjadi dua bagian secara rekursif hingga tiap bagiannya hanya memiliki satu elemen dan proses pembagian terjadi dalam log n langkah, di mana n adalah jumlah elemen dalam array, penggabungan dengan dua bagian yang terurut digabungkan menjadi satu array terurut dan dalam setiap level penggabungan, kita mengunjungi setiap elemen sekali (kompleksitas O(n)). Total waktu eksekusi, karena ada log n level pembagian, dan setiap level membutuhkan waktu O(n) untuk penggabungan, kompleksitas totalnya adalah O(n log n). Untuk merge sort dimana kondisi best case-nya ketika data diinput sudah terurut maka kompleksitas waktunya, tetap O(n log n), karena semua langkah pembagian dan penggabungan tetap harus dilakukan.
