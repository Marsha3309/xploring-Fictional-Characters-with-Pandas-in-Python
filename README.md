# xploring-Fictional-Characters-with-Pandas-in-Python

# 📚 Fictional Character Dataset Exploration with Pandas

This notebook is part of my learning project at **Dibimbing.id**.  
The objective is to explore and analyze a structured dataset of fictional characters using **Python and pandas**.

The dataset contains character traits, roles, backgrounds, and more — giving us the chance to practice basic data wrangling and exploration techniques.

---
# Import library
import pandas as pd

# Load the dataset
df = pd.read_csv('/content/fictional_characters.csv')

# Display the first 5 rows
df.head()

---
# Check number of rows and columns
print(f"Shape of dataset: {df.shape}")

# Show all column names
print("\nColumns:")
print(df.columns.tolist())

# Check for missing values
print("\nMissing values per column:")
print(df.isnull().sum())

## 📁 Dataset Overview

This dataset contains **1,500+ fictional characters**, each with attributes such as:

- `Character Name`
- `Media Type`, `Media Source`
- `Genre`, `Role`, `Alignment`
- `Personality Traits`, `Skills/Abilities`, `Backstory`
- `Relationships`, `Appearance Description`, `Interests/Hobbies`
- And more...

This kind of data can be useful for:
- NLP projects
- Character generator models
- Categorical analysis
- Creative writing prompts

---
# Most common genres
df['Genre'].value_counts().head()
# Unique roles in the dataset
df['Role'].unique()
# Preview characters with 'Hero' alignment
df[df['Alignment'] == 'Hero'].head()

## 🔍 Key Insights

1. Pandas makes it easy to explore structured text data.
2. Fields like *Genre*, *Role*, and *Alignment* can help us group characters for deeper analysis.
3. This type of dataset is great for practicing real-world data cleaning and exploratory data analysis (EDA).

## 💡 What I Learned

✅ How to load and read a CSV file with pandas  
✅ How to view structure and column info  
✅ Filtering and selecting specific data  
✅ Thinking ahead about data cleaning and visualization

---

## 📬 Contact

Feel free to connect or reach out if you'd like to collaborate or discuss Python/data projects!

🔗 (https://www.linkedin.com/in/marsha-rania-chairunissa-b2b599219/)
📧  rania3309@gmail.com

> Created by **Marsha Rania Chairunissa**  
> #Python #Pandas #GoogleColab #DibimbingID #FictionalDataset


