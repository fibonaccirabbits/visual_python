---?image=src/bg-05.png&size=contain
# Data is Beauty

Hands on session

---
####  Geek speak for today
- **Data structure:**  a format that enables efficient access and modification.
- **Object:** a combination of variables, functions, and data structures.
- **Package manager:** a tool that manages packages (programs).

---

#### Python and libraries

Downoad and install a package manager: [Anaconda](https://www.anaconda.com/download/)


On your terminal do: 
```
pip install pandas # real nice data structures
pip install matplotlib # plotting object
pip install seaborn # plotting object
```

---

#### Visualization: a first plot

```
# boot up python interpreter (interactive programming)
python

# import libraries (modules)
import pandas as pd 
import matplotlib.pyplot as plt 
import seaborn as sns 

# load the Iris dataset
iris = sns.load_dataset('iris')

# plot the distribution of petal length
sns.countplot(iris['petal_length'], data=iris)
plt.show()

```

- Congrats! You have just created your first plot with Python.

---
##### Exercise 1

```
# get to know your data
iris.info()

# show available columns
iris.columns

```
- Plot the distribution for each column in the dataset
- (10 minutes)

---
##### Asthetic: make your plot stands out

- Shape
- Color

---
##### Exercise 2

---
##### Collaboration and sharing


---
##### Exercise 3


---?
##### Thank you and see you on the next one!

---
