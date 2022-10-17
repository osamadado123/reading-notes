# Pandas in 10

## importing pandas
```
import numpy as np`

import pandas as pd
```

## to create an object in pandas 

### Creating a Series by passing a list of values, letting pandas create a default integer index:

```
s = pd.Series([1, 3, 5, np.nan, 6, 8])`

s
```
## Creating a DataFrame by passing a NumPy array, with a datetime index using date_range() and labeled columns:

```
dates = pd.date_range("20130101", periods=6)

dates
```

## merging using concat and join 
- concat <br>
pandas provides various facilities for easily combining together Series and DataFrame objects with various kinds of set logic for the indexes and relational algebra functionality in the case of join / merge-type operations.

```
df = pd.DataFrame(np.random.randn(10, 4))

df

pieces = [df[:3], df[3:7], df[7:]]

pd.concat(pieces)
```
- Join <br>
merge() enables SQL style join types along specific columns. See the Database style joining section.
```
left = pd.DataFrame({"key": ["foo", "foo"], "lval": [1, 2]})

right = pd.DataFrame({"key": ["foo", "foo"], "rval": [4, 5]})

left

right

pd.merge(left, right, on="key")
```

## ploting 

We use the standard convention for referencing the matplotlib API

```
import matplotlib.pyplot as plt

plt.close("all")
```

The plt.close method is used to close a figure window:

```
ts = pd.Series(np.random.randn(1000), index=pd.date_range("1/1/2000", periods=1000))

ts = ts.cumsum()

ts.plot();
```

![plot img](https://pandas.pydata.org/pandas-docs/stable/_images/series_plot_basic.png)

On a DataFrame, the plot() method is a convenience to plot all of the columns with labels:

```
df = pd.DataFrame(
    np.random.randn(1000, 4), index=ts.index, columns=["A", "B", "C", "D"]
)


df = df.cumsum()

plt.figure();

df.plot();

plt.legend(loc='best');
```

![plot img2](https://pandas.pydata.org/pandas-docs/stable/_images/frame_plot_basic.png)