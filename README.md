# patika_dev_Veri_Yapilari_ve_Algoritmalar
Selection Sort Projesi --- Merge Sort Projesi --- Binary Search Tree Projesi

## Selection Sort

```
[22,27,16,2,18,6] => Selection sort

Verilen arrayin toplam elemanı n'dir. ilk olarak en küçüğünü bulmak için n kadar işlem yapıyoruz.

[2,27,16,22,18,6] => n

Ardından kalanlar arasında en küçüğünü bulmak için n-1 kadar işlem yaparız. Çünkü en küçük sayıyı bulduk ve en başa yazdık, bu nedenle bir sayımız elenmiş oldu.

[2,6,16,22,18,27] => n-1

Üçüncü eleman listedeki kalan sayılardan daha küçük olduğu için dokunmayız.

Son sayı kalana kadar bu işlem devam edecek ve son kalan için işlem n+1 olacak.

n+(n-1)+(n-2)....n+1 => n*(n+1)/2 => n²+n/2. baskın olan fonksiyo alınır ve katsayılar önemsenmez o yüzden n^2 yi alıyoruz. Yani O(n^2) dir. 
Bu sort'un big o gösterimi o(n²)dir.

[2,6,16,18,22,27] Dizi bu şekilde sıralanır. Soruda istenen 18 sayısı dizide ortadadır. Ortada olduğu için 18 average case'dir.



[7,3,5,8,2,9,4,15,6] en küçük eleman bulunur ve en baştaki ile yer değiştirir

[2,3,5,8,7,9,4,15,6] n

[2,3,5,8,7,9,4,15,6] değişim yok 2. eleman zaten olması gereken yerde

[2,3,4,8,7,9,5,15,6] n-2

[2,3,4,5,7,9,8,15,6] n-3

```

## Merge Sort

```
[16,21,11,8,12,22] -> Merge Sort

1-            [16,21,11]    [8,12,22]

2-      [16,2]  -  [11]   |   [8,12]  -  [22]

3- [16] | [2]  -  [11]    |   [8] | [12]  -  [22]

4-    [2,16]  -  [11]     |    [8,12]   -  [22]

5-            [2,11,16]   |   [8,12,22]

6-                [2,8,11,12,16,22]


Big-O gösterimi => o(nlogn)
```

## Binary Search Tree Projesi
```
###soru
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
Root 5'tir.

5'in solunda '1', sağında ise '7' bulunur.
1'in solunda '0', sağında ise '3' bulunur.
7'nin solunda '6', sağında ise '8' bulunur.
3'ün solunda '2', sağında ise '4' bulunur.
8'in sağında '9' bulunur.

bahsedilen sıralama:

[5, 1, 7, 0, 3, 6, 8, 2, 4, 9]

              5
           1  |  7
       0 | 3     6 | 8
         2 | 4        9
```
