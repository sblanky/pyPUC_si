# pyPUC_si

Raw data from the paper. 

* `psd.zip` contains original pore size distributions
* `aif.zip` contains experimental CO<sub>2</sub> uptake isotherms
* `dataset1` and `dataset2` contain processed data, compressed into a [pickle](https://docs.python.org/3/library/pickle.html), using [lzma compression](https://docs.python.org/3/library/lzma.html). To decompress/unpickle some `file.xz` try;

```py
import pickle
import lzma

with lzma.open('file.xz', 'rb') as f:
  data = pickle.load(f)
data.to_csv('file.csv')
```
