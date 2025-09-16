# 📊 My Matplotlib Learning Journey

Welcome to my repository! 🎉  
This repo contains all the code, notes, and practice files I created while learning **Matplotlib**, a powerful Python library for data visualization.  

---

## 📚 About
- I’m documenting my progress in learning **Matplotlib step by step**.  
- Each script represents different visualization techniques and experiments.  
- The goal is to get hands-on practice with plotting and learn how to visualize data effectively.  

---

## ⚙️ Installation

To run the code in this repository, you need to have Python installed along with Matplotlib.  
You can install Matplotlib using pip:

```bash

pip install matplotlib


Clone the repository:

git clone https://github.com/your-username/matplotlib-learning.git


Navigate into the project folder:

cd matplotlib-learning


Run any Python script, for example:

python day01_line_plot.p


Example Code
import matplotlib.pyplot as plt

fig, axs = plt.subplots(1, 3, figsize=(15, 5))

# Line plot
axs[0].plot(df["Age"], df["Salary"], color="red", marker="*", linewidth=2, markersize=2)
axs[0].grid()
axs[0].set_title("Line Plot")
axs[0].set_xlabel("Age")
axs[0].set_ylabel("Salary")

# Histogram
axs[1].hist(df["Salary"], bins=5, color="skyblue")
axs[1].set_title("Histogram")
axs[1].set_xlabel("Salary")
axs[1].set_ylabel("Frequency")

# Boxplot
axs[2].boxplot(df["Salary"])
axs[2].set_title("Boxplot")
axs[2].set_xlabel("Salary")

plt.savefig("multipleplots.png")
plt.show()
