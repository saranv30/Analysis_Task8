# 1. Run SQL script to generate ranked customer data
# (in your SQL client)
source 'task8_window.sql';

# 2. Load ranked customers in Python
import pandas as pd
ranked = pd.read_csv('ranked_customers.csv')

# 3. Load MoM growth metrics
mom = pd.read_csv('mom_growth.csv')

# 4. Analyze trends and check insights
with open('insights_task8.txt', 'r') as f:
    print(f.read())
