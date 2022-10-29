[16,21,11,8,12,22] --> Merge Sort 

1. yukarıdaki dizinin sort türüne göre aşamaları

###### rastgele sıralanan diziyi ilk önce ikiye bölüyoruz ikiye bölünen diziyi tekrar ikiye bölüyoruz tekli sıra haline geleseye kadar aynı işlemi yapıyoruz

|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|-----------------------------------------------  |- |- |- |- |- |- |- |- |- |- |- |- |
| diziyi ikiye bölüyoruz| 16,21,11,8,12,22 |
|sol ve sağdaki dizileri tekrar ikiye bölüyoruz|16,21,11 ----- 8,12,22|
| tek eleman kalasaya kadar tekrar ikiye bölüyoruz | 16,21 --- 11 ___________ 8,12 --- 22|
|Tek eleman kalana kadar bir kez daha bölüyoruz.		| 16 --- 21 --- 11 _________ 8 --- 12 --- 22 |

######  Bölme işlemi bitikten sonra, tek elemanlı dizilerimizi ikili ikili birleştiriyoruz. Sıralı dizi elde edinceye kadar bu işleme devam ediyoruz.


|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|-----------------------------------------------  |- |- |- |- |- |- |- |- |- |- |- |- |
| tekrar ikili şekilde birleştiriyoruz | 16,21----11_______8,12----22 |
|tekrar sıralı bir şekilde birleştiriyoruz|11,16,21 ________8,12,22|
| son olarak tekrar sıralı bir şekilde birleştiriyoruz |8,11,12,16,21,22,|

2. big o gösterimi:
Recursive bir fonksiyon olduğu için sürekli kendini çağırarak diziyi hep ikiye bölmektedir. 
=> o (nlogn)


