# Pairwise-Learning-to-Rank-Approach-using-LambdaRank


### Dataset
Million queries dataset from TREC 2008 :
[MQ2008](https://www.microsoft.com/en-us/research/project/letor-learning-rank-information-retrieval/#!letor-4-0)

### Parameter
Untuk membangun model perankingan digunakan library XGBoost yang memanfaatkan _packages_ XGBRanker dimana parameter yang digunakan adalah sebagai berikut:
```
...
input_size : X_train.shape[1
hidden_layer_sizes : (16,8,)
activation : ('relu', 'relu',)
solver : 'adam'
...
```

### Hasil Evaluasi 
