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
sns.countplot(iris.species)
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
- Create a plot for each column in the dataset
- Load a new dataset: titanic 
- Briefly describe the dataset
- Create a plot for each column in the dataset

---
##### Asthetic: make your plot stands out

* Shape
* Style and color

---

* Shape

```
# plot a swarmplot
sns.swarmplot(iris.species, iris.petal_length)
plt.show()

#plot a boxplot
sns.boxplot(iris.species, iris.petal_length)
plt.show()
```

---
* Color and style

```
#clear the background
sns.set(style='ticks') 
sns.swarmplot(iris.species, iris.petal_length)
plt.show()

#clear the background and uses other palette
sns.set(style='ticks', palette='husl') 
sns.swarmplot(iris.species, iris.petal_length)
plt.show()

#save the plot
plt.savefig('plot_name.png')

```

---
##### Exercise 2 (10 minutes)
- Interactive programming is a lot of fun but documenting your codes can save a lot of time!
- Create a file yourname_plots.py with a text editor (Vi, TextEdit, Nano, Notepad)
- Recreate swarm, boxen, and box plots. Save them.
- add plt.close() after each plt.save()
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
#bring your code (recreate yourname_plots.py) to the notebook
#run the code with shift + enter (or by clicking the *run* button)

#add on top of your notebook if plot doesnt show
%matplotlib inline

#download the notebook
#send it to the person sitting next to you
```

---
##### Exercise 3 (10 minutes)
This time no code examples. Use your previous experience to solve this exercise.
- Your mission: Using the titanic dataset, figure out if money increase the chance of survival
- Dataset [titanic.csv](https://github.com/fibonaccirabbits/visual_python/tree/master/src)

```
#Hint:
Run this code to list all kinds of plots in seaborn

print([item for item in dir(sns) if 'plot' in item])
```

---
##### Summary
We explored: 
* Turning data into a visual object (plot)
* Making that visual object engaging and infromative via shapes and colors
* Documenting codes and outputs for seamless collaboration and sharing

---?image=src/bg-05.png&size=contain
Share your thoughts: [**feedback**](https://docs.google.com/forms/d/e/1FAIpQLSf3Q05NBO8jELU_6uLeobsRcvbNUBpwPRU3OPivHoukbDZmlQ/viewform)

---?image=src/thanks-06.png&size=contain



