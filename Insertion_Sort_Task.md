1. Dizi [22,27,16,2,18,6] -> Insertion Sort

 1. Görev
 Sort türüne göre aþamalarý:
  Insertion sort algoritmasýnda dizinin en küçük elemaný bulunarak sýralama yapýlýr.
  En küçük elemana bakýlýr ve 0. indekse yazýlýr.
   - [2,27,16,22,18,6]
  0. indeksde en küçük eleman ile mevcut eleman yer deðiþtirdikten sonra sonraki indekse geçilir.
  Artýk dizide bakýlmasý gereken n-1 eleman vardýr.
   - [2,"27,16,22,18,6"]
  1. indekse 2. en küçük elemaný yerleþtirmek için tekrar en küçük veriye bakýlýr.
   - [2,6,"16,22,18,27"] bakýlmasý gereken n-2 eleman kalýr.
  n, n-1,n-2 ... 1 e kadar bu iþlem tekrarlanýr.
   - [2,6,16,"22,18,27"]
   - [2,6,16,18,"22,27"]
   - [2,6,16,18,22,27]
  Böylece soldan saða küçükten büyüðe sýralama yapýlmýþ olur.

 2. Görev
  Big-O gösterimi
   O(n^2)

 3.Görev
  Time Complexity
   Worst Case: Aradýýðýmýz sayýnýn her seferinde sonda olmasý durumudur. Bu durumda her bir eleman bir sonraki elemandan büyük olacaðýndan sýralama süremiz maximum olur.
    [n*(n-1)]/2   :  n^2 
  
   Best Case: Tam sýralý dizi gelme durumu dur. Yani n kadar iþlem yapýlýr. 
     n
   Avarage Case: Worst Case ile Best Case'in ortalamasý olarak bulunabilir. 
     n^2    
 4.Görev
  18 sayýsý hangi case kapsamýna girer ?
   Dizinin ortasýnda yer aldýðý için average case kapsamýna girer.
2. dizi [7,3,5,8,2,9,4,15,6] -> Insertion Sort

 Sort türüne göre aþamalarý:
   - [7,3,5,8,2,9,4,15,6]
  En küçük elemana bakýlýr ve 0. indekse yazýlýr.
   - [2,3,5,8,7,9,4,15,6]
  0. indeksde en küçük eleman ile mevcut eleman yer deðiþtirdikten sonra sonraki indekse geçilir.
  Artýk dizide bakýlmasý gereken n-1 eleman vardýr.
   - [2,"3,5,8,7,9,4,15,6"]
  1. indekse 2. en küçük elemaný yerleþtirmek için tekrar en küçük veriye bakýlýr.
   - [2,3,"4,8,7,9,5,15,6"] bakýlmasý gereken n-2 eleman kalýr.
  n, n-1,n-2 ... 1 e kadar bu iþlem tekrarlanýr.
   - [2,3,4,"5,7,9,8,15,6"]
   - [2,3,4,5,"6,9,8,15,7"]
   - [2,3,4,5,6,"9,8,15,7"]
   - [2,3,4,5,6,"7,8,15,9"]
   - [2,3,4,5,6,7,"8,15,9"]
   - [2,3,4,5,6,7,8,"15,9"]
   - [2,3,4,5,6,7,8,9,"15"]
   - [2,3,4,5,6,7,8,9,15]
  