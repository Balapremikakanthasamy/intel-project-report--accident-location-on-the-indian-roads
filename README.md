import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv('accident location.csv.csv')  
locations = df[['LOCATION OF THE ACCIDENT']]  
fatalities = df[['NO OF FATALITIES']]  
plt.scatter(locations['LOCATION OF THE ACCIDENT'],fatalities['NO OF FATALITIES'], c='green', alpha=0.5) 
plt.xticks(rotation='vertical')
plt.xlabel('locations')
plt.ylabel('fatalities')
plt.title('Accident Locations')
plt.show()
