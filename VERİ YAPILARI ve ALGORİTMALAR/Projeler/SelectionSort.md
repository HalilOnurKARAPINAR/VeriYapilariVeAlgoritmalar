# Proje 1
## Insertion Sort
### [22,27,16,2,18,6] -> Insertion Sort
***
#### 1) Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

1. [22,27,16,2,18,6] -> 22<27 ```22``` dizinde ```27``` 'den küçük olduğu için ```22,27``` şeklinde sıralanır. 
2. [22,27|16,2,18,6] -> 16<27, 16<22 ```16``` dizinde ```22, 27``` 'den küçük olduğu için ```16,22,27``` şeklinde sıralanır. 
3. [16,22,27|2,18,6] -> 2<27, 2<22, 2<16 ```2```dizinde ```16, 22, 27``` 'den küçük olduğu için ```2,16,22,27``` şeklinde sıralanır.
4. [2,16,22,27|18,6] -> 18<27, 18<22, 16<18 ```18```dizinde ```22,27``` 'den küçük ```2,16```'dan büyük olduğu için ```2,16,18,22,27``` şeklinde sıralanır.
5. [2,16,18,22,27|6] -> 6<27, 6<22, 6<18, 6<16 2<6 ```6```dizinde ```16,18,22,27``` 'den küçük ```2```'den büyük olduğu için ```2,6,16,18,22,27``` şeklinde sıralanır.
6. [2,6,16,18,22,27]
*** 
#### 2) Big-O gösterimini yazınız.
###### Dizideki eleman sayısı n olsun. Big-O yöntemine göre sıralama yapılırken işlem sayısı da ```n``` olur. Son işlem sayısı ```1``` olana kadar devam eder.
- Insertion Sort algoritması ```n``` elemanlı bir listede, ikinci eleman için en fazla 1 karşılaştırma ve 1 yer değiştirme yapar. 
- Üçüncü eleman için 2 karşılaştırma ve 2 yer değiştirme, dördüncü eleman için 3 karşılaştırma ve 3 yer değiştirme yapar. Bu şekilde son eleman için en fazla ```n-1``` karşılaştırma ve ```n-1``` yer değiştirme yapar. 
- Listedeki bütün elemanlar için yapılan karşılaştırmaların ve yer değiştirmelerin toplamı
2(1+2+3+4+...+(n-2)+(n-1))=2(n(n-1)/2)=n(n-1) yapar. 
- Hesaplamalar sonucunda elde edilen
n(n-1)
değerinin asimptotik üst sınırı O(n²) değerini verir.
#### Big-O değeri = O(n²)
* * *
#### 3) Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız.

- ```Average case: Aradığımız sayının ortada olması```
  [.,.,.,18,.,.,.] 
- ```Worst case: Aradığımız sayının sonda olması```
  [.,.,.,.,.,.,18]
- ```Best case: Aradığımız sayının dizinin en başında olması```
  [18,.,.,.,.,.,.,]
 
- [2,6,16,18,22,27] dizisine bakıldığında 18 sayısı ortada olduğu için ```Average Case``` kapsamına girer.
***
## Selection Sort
#### 4) [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.
1. [```2```,3,5,8,7,9,4,15,6]
2. [2,```3```,5,8,7,9,4,15,6]
3. [2,3,```4```,8,7,9,5,15,6]
4. [2,3,4,```5```,7,9,8,15,6]

***
[Halil Onur KARAPINAR](https://github.com/HalilOnurKARAPINAR)
[Patika.dev](https://app.patika.dev/halilonur)