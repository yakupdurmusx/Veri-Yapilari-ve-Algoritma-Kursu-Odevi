# Veri-Yapilari-ve-Algoritma-Kursu-Odevi
All comments are attached below


> Proje 1

> [22,27,16,2,18,6] -> Insertion Sort
> 
> Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
> 
> Big-O gösterimini yazınız.
> 
> Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız.
> 
> Average case: Aradığımız sayının ortada olması
> Worst case: Aradığımız sayının sonda olması
> Best case: Aradığımız sayının dizinin en başında olması


Cevap:       [22,27,16,2,18,6] n
             [16,22,27,2,18,6] n-1
             [2,16,22,27,18,6] n-2
             [2,16,18,22,27,6] n-3
             [2,6,16,18,22,27] 1

Big-O Notation => n+(n-1)+(n-2)...1 = n.(n+1)/2 = n^2+n/2 => O(n^2) (Bu notasyon worst case ve average case icin gecerlidir.)
Dizide aranan '18' sayisi Average Case kapsamina girer. 


> [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

Cevap:      [7,3,5,8,2,9,4,15,6] n
            [2,3,5,8,7,9,4,15,6] n-1
            [2,3,4,8,7,9,5,15,6] n-2
            [2,3,4,5,7,9,8,15,6] n-3
            [2,3,4,5,6,9,8,15,7] n-4

> Proje 2
> 
> [16,21,11,8,12,22] -> Merge Sort
> 
> Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
> Big-O gösterimini yazınız.

Cevap:          [16,21,11,8,12,22] n

           [16,21,11]      <>       [8,12,22] n-1
          [16] <> [21,11]     [8]<> [12,22] n-2
    [16] <> [21] <> [11]   [8]<> [12]<> [22] n-3
          [16] <> [11,21]     [8] <> [12,22] n-4
             [11,16,21]   <>      [8,12,22] n-5

                    [8,11,12,16,21,22] n-6

Big-O Notation => O(nlogn)

> Proje 3

> [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
> 
> Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

Cevap: root = 5
                                     5
                                  /      \
                                1          7
                              /  \        /   \
                             0    3      6     8 
                                  / \            \
                                 2   4             9
