1. Dizi [22,27,16,2,18,6] -> Insertion Sort

 1. G�rev
 Sort t�r�ne g�re a�amalar�:
  Insertion sort algoritmas�nda dizinin en k���k eleman� bulunarak s�ralama yap�l�r.
  En k���k elemana bak�l�r ve 0. indekse yaz�l�r.
   - [2,27,16,22,18,6]
  0. indeksde en k���k eleman ile mevcut eleman yer de�i�tirdikten sonra sonraki indekse ge�ilir.
  Art�k dizide bak�lmas� gereken n-1 eleman vard�r.
   - [2,"27,16,22,18,6"]
  1. indekse 2. en k���k eleman� yerle�tirmek i�in tekrar en k���k veriye bak�l�r.
   - [2,6,"16,22,18,27"] bak�lmas� gereken n-2 eleman kal�r.
  n, n-1,n-2 ... 1 e kadar bu i�lem tekrarlan�r.
   - [2,6,16,"22,18,27"]
   - [2,6,16,18,"22,27"]
   - [2,6,16,18,22,27]
  B�ylece soldan sa�a k���kten b�y��e s�ralama yap�lm�� olur.

 2. G�rev
  Big-O g�sterimi
   O(n^2)

 3.G�rev
  Time Complexity
   Worst Case: Arad����m�z say�n�n her seferinde sonda olmas� durumudur. Bu durumda her bir eleman bir sonraki elemandan b�y�k olaca��ndan s�ralama s�remiz maximum olur.
    [n*(n-1)]/2   :  n^2 
  
   Best Case: Tam s�ral� dizi gelme durumu dur. Yani n kadar i�lem yap�l�r. 
     n
   Avarage Case: Worst Case ile Best Case'in ortalamas� olarak bulunabilir. 
     n^2    
 4.G�rev
  18 say�s� hangi case kapsam�na girer ?
   Dizinin ortas�nda yer ald��� i�in average case kapsam�na girer.
2. dizi [7,3,5,8,2,9,4,15,6] -> Insertion Sort

 Sort t�r�ne g�re a�amalar�:
   - [7,3,5,8,2,9,4,15,6]
  En k���k elemana bak�l�r ve 0. indekse yaz�l�r.
   - [2,3,5,8,7,9,4,15,6]
  0. indeksde en k���k eleman ile mevcut eleman yer de�i�tirdikten sonra sonraki indekse ge�ilir.
  Art�k dizide bak�lmas� gereken n-1 eleman vard�r.
   - [2,"3,5,8,7,9,4,15,6"]
  1. indekse 2. en k���k eleman� yerle�tirmek i�in tekrar en k���k veriye bak�l�r.
   - [2,3,"4,8,7,9,5,15,6"] bak�lmas� gereken n-2 eleman kal�r.
  n, n-1,n-2 ... 1 e kadar bu i�lem tekrarlan�r.
   - [2,3,4,"5,7,9,8,15,6"]
   - [2,3,4,5,"6,9,8,15,7"]
   - [2,3,4,5,6,"9,8,15,7"]
   - [2,3,4,5,6,"7,8,15,9"]
   - [2,3,4,5,6,7,"8,15,9"]
   - [2,3,4,5,6,7,8,"15,9"]
   - [2,3,4,5,6,7,8,9,"15"]
   - [2,3,4,5,6,7,8,9,15]
  