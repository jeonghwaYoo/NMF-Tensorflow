# NMF-Tensorflow
Non-negative Matrix Factorization (NMF) Tensorflow Implementation

# Examples
```
>>> from nmf import NMF
>>> import numpy as np
>>> V = np.array([[1, 1], [2, 1], [3, 1.2], [4, 1], [5, 0.8], [6, 1]])
>>> model = NMF(r_components=2,max_iter=200,learning_rate=0.01,display_step=10,optimizer='mu')
>>> W, H = model.fit_transform(V)
>>> print(V)
>>> print(model.inverse_transform(W, H))
```
