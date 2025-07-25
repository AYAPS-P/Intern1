import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

data = {
    "Student": ["A", "B", "C", "D", "E", "F", "G"],
    "Study Hours": [1, 2, 3, 4, 5, 6, 7],
    "Sleep Hours": [8, 7, 6, 2, 3, 4, 1],
    "Score": [45, 50, 55, 70, 60, 80, 85]
}

df = pd.DataFrame(data)

print("Descriptive Statistics:\n")
print(df.describe())

print("\nCorrelation Matrix:\n")
print(df.corr(numeric_only=True))

sns.set(style="whitegrid")
plt.figure(figsize=(12, 5))

plt.subplot(1, 2, 1)
sns.scatterplot(x="Study Hours", y="Score", data=df, color="blue")
plt.title("Study Hours vs Score")

plt.subplot(1, 2, 2)
sns.scatterplot(x="Sleep Hours", y="Score", data=df, color="green")
plt.title("Sleep Hours vs Score")

plt.tight_layout()
plt.show()
