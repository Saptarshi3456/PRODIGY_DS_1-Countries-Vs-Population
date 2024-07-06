# PRODIGY_DS_1-Countries-Vs-Population

import pandas as pd
import matplotlib.pyplot as plt


data = {
    "Country": ["China", "India", "United States", "Indonesia", "Pakistan", "Brazil", "Nigeria", "Bangladesh", "Russia", "Mexico"],
    "Population": [1444216107, 1393409038, 331883986, 273523621, 225199937, 213993437, 211400708, 166303498, 145912025, 130262216]
}


df = pd.DataFrame(data)


plt.figure(figsize=(12, 8))
plt.bar(df['Country'], df['Population'], color='skyblue')
plt.xlabel('Country')
plt.ylabel('Population')
plt.title('Population Distribution of Top 10 Most Populous Countries')
plt.xticks(rotation=45)
plt.show()