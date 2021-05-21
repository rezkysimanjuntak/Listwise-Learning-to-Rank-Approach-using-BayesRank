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

|Fold |   NDGC@1    |   NDGC@3    |   NDGC@5   |   NDGC@10   |   Average   |
|-----|-------------|-------------|-------------|-------------|-------------|
|  1  | 0.286624    | 0.273508    | 0.413618    | 0.46639     | 0.360035    |
|  2  | 0.146497    | 0.410316    | 0.172978    | 0.424505    | 0.288574    |
|  3  | 0.216561    | 0.337628	  | 0.245291    | 0.396311    | 0.298948	  |
|  4  | 0.218684    | 0.34809     | 0.213245    | 0.412037    | 0.298014    |
|  5  | 0.163482	  | 0.170368    | 0.322891    | 0.395443    | 0.263046	  |
