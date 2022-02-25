# oikotie-helsinki-restapi
Apartment for sale and sold on the Oikotie.fi website. The data is not updated daily and only includes apartments located in Helsinki.

link : https://oikotie-helsinki-restapi.herokuapp.com/ 

Tutorial:

```python
import requests
import pandas as pd

data = requests.get('https://oikotie-helsinki-restapi.herokuapp.com/').json()['Data']
df = pd.DataFrame.from_dict(data)
print(df.head(10))

```


