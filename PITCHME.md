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
sns.scatterplot(iris.species, iris.petal_length)
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
10 minutes
- Create a scatter plot for each column in the dataset
- Load a new dataset: titanic 
- Briefly describe the dataset
- Create a scatter plot for each column in the dataset

---
##### Asthetic: make your plot stands out

####### Shape
```
sns.swarmplot(iris.species, iris.petal_length)
plt.show()
sns.boxplot(iris.species, iris.petal_length)
plt.show()
sns.boxplot(iris.species, iris.petal_length)
plt.show()
```
- Color

---
##### Exercise 2

---
##### Collaboration and sharing


---
##### Exercise 3

---
##### Summary
We explored: 
* Turning data into a visual object (plot)
* Making that visual object engaging and infromative via shapes and colors
* Documenting outputs for seamless collaboration and sharing

---?image=src/thanks-06.png&size=contain



