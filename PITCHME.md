# Data is Beauty

Hands on session

---
#### Lingos
Geek speaks for today:
- **Data structure:**  a format that enables efficient access and modification.
- **Object:** a combination of variables, functions, and data structures.
- **Package manager:** a tool that manages packages (programs).

---

#### Python and libraries

Downoad and install [Anaconda](https://www.anaconda.com/download/)


On your terminal do: 
```
pip install pandas # real nice data structures
pip install matplotlib # plot object
pip install seaborn # plot object
```

---

#### Toy data

```
# boot up python interpreter (interactive programming)
python

# import libraries (modules)
import pandas as pd 
import matplotlib.pyplot as plt 
import seaborn as sns 

# load Iris dataset
iris = sns.load_dataset('iris')

# plot distribution of petal lenght
sns.countplot(iris['petal_length'], data=iris)
plt.show()

```

- Congrats! You have just created your first plot with Python.

