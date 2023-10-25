### Horizontal bar Lot 

```
plt.figure(figsize=(50, 250))  # Optional: You can specify the figure size for better visibility
sns.barplot(x='moodle_cum_act', y='coursecode', data=week_9_results_good_merge, palette="Blues_d")  # Use barplot for horizontal bars

plt.ylabel('Course Code')  # y-axis represents course codes
plt.xlabel('Average Moodle Activity')  # x-axis represents the Moodle activity
plt.title('Average Moodle Activity by Course Code')
plt.tight_layout()  # Adjust the layout to avoid clipping
plt.show()
```

### Showing 3 variables in a scatter Plot:

```
sns.relplot(data=week_9_results_good_merge,height=10,x = "at_risk_f1-score" , y="moodle_cum_act" , hue="macro avg_support")

plt.grid()  #just add this
```


## HeatMap of Correlation: 

```
  
# Importing necessary libraries
import seaborn as sns
import pandas as pd
import matplotlib.pyplot as plt

# Create a sample dataset: This would be your actual data in practice
data = {'Feature1': [1, 2, 3, 4, 5],
        'Feature2': [5, 4, 3, 2, 1],
        'Feature3': [2, 2, 2, 2, 2],
        'Class': [0, 1, 0, 1, 0]}

df = pd.DataFrame(data)

# Compute the correlation matrix
corr = df.corr()

# Generate the heatmap
plt.figure(figsize=(10, 8))
sns.heatmap(corr, annot=True, cmap='coolwarm', cbar=True, square=True, fmt='.2f', annot_kws={'size': 15})
plt.show()

```
