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
Download and install a package manager: [Anaconda](https://www.anaconda.com/download/)



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
##### Exercise 1 (10 minutes)

```
# get to know your data
iris.info()

# show available columns
iris.columns

```
- Create a scatter plot for each column in the dataset
- Load a new dataset: titanic 
- Briefly describe the dataset
- Create a scatter plot for each column in the dataset

---
##### Asthetic: make your plot stands out

* Shape
* Style and color

---

* Shape

```
sns.swarmplot(iris.species, iris.petal_length)
plt.show()
sns.boxenplot(iris.species, iris.petal_length)
plt.show()
sns.boxplot(iris.species, iris.petal_length)
plt.show()
```

---
* Color and style

```
#clears the background
sns.set(style='ticks') 
plt.swarmplot(iris.species, iris.petal_length)

#clears the background and uses other palette
sns.set(style='ticks', palette='husl') 
plt.swarmplot(iris.species, iris.petal_length)

#save the plot
plt.savefig('plot_name.png')

```

---
##### Exercise 2 (10 minutes)
- Interactive programming is a lot of fun but documenting your codes can save a lot of time!
- Create a file yourname_plots.py with a text editor (Vi, TextEdit, Nano, Notepad)
- Recreate swarm, boxen, and box plots. Save them.

```
# run you code
python yourname_plots.py
```
---
##### Collaboration and sharing

---
So far the code and its output are at different places. Jupyter notebook integrates them so you don't have to!

```
#start a jupyter notebook
jupyter notebook

#bring your code to the notebook
#run the code with shift + enter
```

---
##### Exercise 3 (10 minutes)
This time no code examples. Use your previous experience to solve this exercise.
- Your mission: Using the titanic dataset, figure out if money increase the chance of survival

```
#Hint: run this code to list all kinds of plots in seaborn
print([item for item in dir(sns) if 'plot' in item])
```

---
##### Summary
We explored: 
* Turning data into a visual object (plot)
* Making that visual object engaging and infromative via shapes and colors
* Documenting outputs for seamless collaboration and sharing

---?image=src/thanks-06.png&size=contain



