## Names
Rafael Epplee & Hans Ole Hatzel

## Features
Our initial choice of 3 features being the mean of each rgb value. Yielded a 84% accuracy on whole dataset used for both training and testing.

* When the rgb features and the data split in halt for training and testing set we got: 
```
Errro: 0.18333333333333332
```

* Adding standard deviation yielded to the rgb features yielded:
```
Errro: 0.06666666666666667
```

* We ran an edge detection filter (sobel) and added the brightest pixel (meaning the greatest edge) as a feature:
```
Error: 0.0
```

## Model
Our choice of features yielded this model and characteristics:

$\mu_0$  `[ 165.75069444  128.09398148  127.90520833   20.44602683  -41.93333333]`

$\mu_1$ 	` [ 179.88587963  144.90381944  147.94641204   24.30642702 -197.57777778]`

$\Sigma$:

``` [[   8116.59812886    9060.32057432    8200.28847656     994.64075342   -35886.71608796]
     [   9060.32057432   11028.62910096    9625.21327984     734.50948492   -40419.29996142]
     [   8200.28847656    9625.21327984    9420.98863812    1138.78109748   -48429.72685185]
     [    994.64075342     734.50948492    1138.78109748     507.91402611   -10200.7379977 ]
     [ -35886.71608796  -40419.29996142  -48429.72685185  -10200.7379977     387142.93333333]]
```


$\varphi: 0.5$


Error: 0.0
