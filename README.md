![ ](https://user-images.githubusercontent.com/44925804/50568927-607a6e00-0d28-11e9-8023-ed5f33346748.jpg)
# Mega Sena Statistics: 

### Overview

Creating statistics on 'Mega-Sena' lottery results.

### Methods
 - Data cleaning , EDA and Statistic was made using Pandas and Numpy librarys in Python.
 - Plots using matplotlib.pyplot library.
 - Words were tokenized using CountVectorize from sklearn library 
### Results
 - Numbers 10, 5, 53, 4, 23 where the most frequent.
 - Numbers 9, 22, 55, 21, 26 where the less frequent.
 - Even and Odd numbers almost had the same frequency (50.4 and 49.6 respectively).
 - Numbers from 1-10 are present in 17.02% of draws (highest).
 - Numbers from 21-30 are present in 16.34% of draws(lowest).
 - Number combination 29,38,50 was present in 8 draws.(highest)
 
### Softwares Used
- Jupyter notebook
- Python 3.6
- Powerpoint

### Notebooks:

1. mega_sena.ipynb

### Datasets

[Mega-Sena results](https://campograndesantos.wordpress.com/64-concurso-da-mega-senatodos-os-resultados/)


#### Data Dictionary

|Label|Type|Description|
|---|---|---|
|draw|int64|Number of the draw|
|data|object|Date of the draw (dd/MM/YYYY)|
|num1|int64|1st winning number in the draw|
|num2|int64|2st winning number in the draw|
|num3|int64|3st winning number in the draw|
|num4|int64|4st winning number in the draw|
|num5|int64|5st winning number in the draw|
|num6|int64|6st winning number in the draw|
|is_even|int64|Dummy: 1 for even, 0 for odd|
