---
#layout: post
#title: "jekyll-jupyte"
#date: 2017-09-23
---


```python
import numpy as np
import scipy
from sklearn.datasets import fetch_mldata

```

Once I had a bit of a notebook, I wanted to convert it to jekylly markdown. There’s an ipython command for this - having saved the notebook, run:


```python
import matplotlib.pyplot as plt
import numpy as np
a = np.linspace(0,10,100)
b = np.exp(-a)
plt.plot(a,b)
plt.show()

```


![png](jekyll_jupyter_files/jekyll_jupyter_2_0.png)



```python
1+2
```




    3




```python

```
