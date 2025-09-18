# WSINDy4Dispersal
Weak form model discovery for insect dispersal.

<img width="469" height="324" alt="CATS_WSINDY_PIC" src="https://github.com/user-attachments/assets/90722c88-fab0-419e-bd1c-1ab362f2ca26" />

---

Python code accompanying the manuscript **"Weak Form Learning for Mean-Field Partial Differential Equations: an Application to Caterpillar Movement"** submitted to *[journal name]*
- Zenodo: [https://zenodo.org/records/17156064](https://zenodo.org/records/17156064)
- ArXiV pre-print: [will update once pre-print is up]
```
@misc{?
      title={?}, 
      author={?},
      year={?},
      eprint={?},
      archivePrefix={?},
      primaryClass={?},
      url={?}}
```

**Open data:** see the [`caterpillars.csv`](https://github.com/MathBioCU/WSINDy4Dispersal/blob/main/caterpillars.csv) file.
- See [the tutorials and examples located here](https://github.com/SethMinor/PyWSINDy-for-PDEs) for instructions on how to use the codebase.
- To recreate results in the paper, see the [`wsindy_for_dispersal.ipynb`](https://github.com/MathBioCU/WSINDy4Dispersal/blob/main/wsindy_for_dispersal.ipynb) notebook.

---

###### Our code uses the following dependencies:
```python3
# Core
import torch
import scipy
import numpy as np
import matplotlib
import itertools
import symengine as sp
import pandas as pd

# Special
import torch.linalg as la
from scipy.signal import convolve
from scipy.special import factorial
import matplotlib.pyplot as plt
from tqdm import tqdm
from IPython.display import display,Math

# Weak SINDy
from wsindy import *
from helper_fcns import *
```

###### Install PyWSINDy for PDEs a Bash environment:
```python3
wget -q https://raw.githubusercontent.com/SethMinor/PyWSINDy-for-PDEs/main/wsindy.py
wget -q https://raw.githubusercontent.com/SethMinor/PyWSINDy-for-PDEs/main/helper_fcns.py
```
