### [22,27,16,2,18,6] -> insertion sort 
## 1.Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
1.adım [22,27,16,2,18,6] = 27 sayısını 22 ile karşılaştır ve 22 den büyük ise olduğu yerde kalsın 

2.adım [22,27,16,2,18,6] = 16 sayısını 27 ile karşılaştır 16, 27 den küçük ise yer değistir -> [22,16,27,2,18,6] = 16 yı tekrar kendinden önceki sayı ile karşılaştır küçük ise yer değiştir -> [16,22,27,2,18,6] 

3.adım [16,22,27,2,18,6] = 2 sayısını kendinden bir önceki sayı ile karşılaştır, eğer kendinden büyük ise yer değiştir ve bunu kendinden önceki sayıdan küçük olana kadar yap -> [16,22,2,27,18,6] -> [16,2,22,27,18,6] -> [2,16,22,27,18,6]

4.adım [2,16,22,27,18,6] = 18 sayısını kendinden bir önceki sayı ile karşılaştır, kendinden küçük ise yer değiştir ve bunu kendinden önceki sayıdan küçük olana kadar yap -> [2,16,22,18,27,6] -> [2,16,18,22,27,6]

5.adım [2,16,18,22,27,6] = 6 sayısını kendinden bir önceki sayı ile karşılaştır, kendinden küçük ise yer değiştir ve bunu kendinden önceki sayıdan küçük olana kadar yap ->[2,16,18,22,6,27] -> [2,16,18,6,22,27] -> [2,16,6,18,22,27] -> [2,6,16,18,22,27]

## 2.Big-O gösterimini yazınız.

O(n^2)
s
## 3.Time Complexity

1. Worst Case
- Aradığımız sayının sonda olması

2. Average Case
- Aradığımız sayının ortada olması

3. Best Case 
- Aradığımız sayının ilk başta olması


## 4.Dizi sıralandıktan sonra 18 sayısı hangi case yapısına girer?
[2,6,16,18,22,27] --> 18 sayısı ortada olduğu için average case yapısı olur


### [7,3,5,8,2,9,4,15,6] insertion sort sıralamasına göre ilk dört adımı?

1. adım [3,7,5,8,2,9,4,15,6]
2. adım [3,5,7,8,2,9,4,15,6]
3. adım [3,5,7,8,2,9,4,15,6]
4. adım [2,3,5,7,8,9,4,15,6] 