[7,5,1,8,3,6,0,9,4,2] dizisinin binary search tree aşamları

ilk olarak kendimize bir root seçeriz

root=5

ilk baştan başlayarak 5 sayısına seçtiğimiz sayı 5 ten küçük mü büyük mü diye soararız küçük ise soluna büyük ise sağına yazarız

| Açıklama |      |  |
|--       |-    |-  |
|    root   |      | 5 |

### 7, 5 ten büyük olduğu için sağına ekliyoruz
| Açıklama |      |  | |
|--       |-    |-  |- |
|         |     | 5 | |
|         |     |  \  | |
|  7 ekliyoruz|     |   |   7  |

### 1, 5 ten küçük olduğu için soluna ekliyoruz

| Açıklama         |       |        |       |     |      |
|--                |-      |:---:       |-      |-    |-     |
|                  |       | 5      |       |     |      |
|                  |   /   |        |       | \   |      |
|    1 ekledik     |1      |        |       |     |7     |
|                  |       |        |       |     |      |

### 8, 7 den büyük olduğu için 7 nin sağına ekliyoruz

| Açıklama         |       |        |       |     |      |   |
|--                |-      |:---:       |-      |-    |-     |-   |
|                  |       | 5      |       |     |      |   |
|                  |   /   |        |       | \   |      |   |
|                  |1      |        |       |     |7     |   |
|                  |       |        |       |     |  \    |  |
|                  |       |        |       |     |      |  8 |

### 3, 1 den büyük olduğu için 1 in sağına ekliyoruz

| Açıklama         |       |        |       |     |      |   |
|--                |-      |:---:       |-      |-    |-     |-   |
|                  |       | 5      |       |     |      |   |
|                  |   /   |        |       | \   |      |   |
|                  |1      |        |       |     |7     |   |
|                  |   \    |        |       |     |  \    |  |
|                  |       |  3      |       |     |      |  8 |

### 6, beşten büyük olduğu için sağ tarafta yediyle kontrol ediyoruz ve 7 den küçük olduğu için 7 nin soluna ekliyoruz 

| Açıklama         |       |      |  |       |     |      |    |
|--                |-      |:---: | -|-      |-    |-     |-   |
|                  |       | 5    |  |       |     |      |    |
|                  |   /   |      |  |       | \   |      |    |
|                  |1      |      |  |       |     |7     |    |
|                  |   \   |      |  |       |   / |  \   |    |
|                  |       |  3   |  |      6|     |      |  8 |

### 0 beşten küçük 1 den de küçük olduğu için 1 in soluna ekliyouruz

| Açıklama |  |      |       |      |  |       |     |      |    |
|--        |- |-     |-      |:---: | -|-      |-    |-     |-   |
|          |  |      |       | 5    |  |       |     |      |    |
|          |  |      |   /   |      |  |       | \   |      |    |
|          |  |      |1      |      |  |       |     |7     |    |
|          |  |    / |   \   |      |  |       |   / |  \   |    |
|          | 0 |      |       |  3   |  |      6|     |      |  8 |

### 9, beşten büyük 8 den büyük olduğu için 8 in soluna ekliyoruz

| Açıklama |  |      |       |      |  |       |     |      |       |  |
|--        |- |-     |-      |:---: | -|-      |-    |-     |-      |- |
|          |  |      |       | 5    |  |       |     |      |       |  |
|          |  |      |   /   |      |  |       | \   |      |       |  |
|          |  |      |1      |      |  |       |     |7     |       |  |
|          |  |    / |   \   |      |  |       |   / |  \   |       |  |
|          | 0 |      |       |  3   |  |      6|     |      |  8   |  |
|          |   |      |       |      |  |       |     |      |    \ |  |
|          |   |      |       |      |  |       |     |      |      | 9|

 ### 4, beşten küçük olduğu için sol tarafta 3 ten büyük olduğu için 3 ün sağına yazarız

 | Açıklama |  |      |       |      |  |       |     |      |       |  |
|--        |- |-     |-      |:---: | -|-      |-    |-     |-      |- |
|          |  |      |       | 5    |  |       |     |      |       |  |
|          |  |      |   /   |      |  |       | \   |      |       |  |
|          |  |      |1      |      |  |       |     |7     |       |  |
|          |  |    / |   \   |      |  |       |   / |  \   |       |  |
|          | 0 |      |       |  3   |  |      6|     |      |  8   |  |
|          |   |      |       |   \   |  |       |     |      |    \ |  |
|          |   |      |       |      |4  |       |     |      |      | 9|

### 2 beşten küçük olduğu için sol tarafta kontrol sağlıyoruz 1 den büyük için sağa gidiyoruz ve 3 ten küçük olduğu için 3 ün soluna ekleriz

| Açıklama |  |      |       |      |  |       |     |      |       |  |
|--        |- |-     |-      |:---: | -|-      |-    |-     |-      |- |
|          |  |      |       | 5    |  |       |     |      |       |  |
|          |  |      |   /   |      |  |       | \   |      |       |  |
|          |  |      |1      |      |  |       |     |7     |       |  |
|          |  |    / |   \   |      |  |       |   / |  \   |       |  |
|          | 0 |      |       |  3   |  |      6|     |      |  8   |  |
|          |   |      |     /  |   \   |  |       |     |      |    \ |  |
|          |   |   2   |       |      |4  |       |     |      |      | 9|
