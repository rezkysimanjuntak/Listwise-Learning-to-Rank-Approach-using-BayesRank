# Pairwise-Learning-to-Rank-Approach-using-LambdaRank
_Learning to Rank_ merupakan salah satu masalah machine learning yang tujuannya adalah untuk membangun suatu model perangkingan dari data pembelajaran sehingga diperoleh urutan yang memiliki relevansi dan preferensi yang optimal. **LambdaRank** pada IR (_Information Retrieval_) mampu memecahkan masalah dengan menentukan gradien dari biaya yang diberikan di tempat tujuan. **LambdaRank** memperoleh hasil yang lebih baik saat memperkuat gradien dengan perubahan NDCG yang muncul akibat dari pertukaran dokumen.

### Dataset
Million queries dataset from Microsoft LETOR 4.0 2008 :
[MQ2008](https://www.microsoft.com/en-us/research/project/letor-learning-rank-information-retrieval/#!letor-4-0)

### Parameter
Untuk membangun model perankingan digunakan library Tensorflow yang memanfaatkan _packages_ Keras untuk melakukan fungsi perangkingan dimana parameter yang digunakan adalah sebagai berikut :
```
...
input_size : X_train.shape[1
hidden_layer_sizes : (16,8,)
activation : ('relu', 'relu',)
solver : 'adam'
...
```

### Hasil Perolehan Nilai NDGC
```
NDGC for fold 1 :  0.621774
NDGC for fold 2 :  0.654353
NDGC for fold 3 :  0.639651
NDGC for fold 4 :  0.615033
NDGC for fold 5 :  0.593280
------------------------
NDGC Average    :  0.624818
```
