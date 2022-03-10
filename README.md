# oikotie-helsinki-restapi
* Apartments that are for sale and apartments that have already been sold on the Oikotie.fi website. The data is not updated daily and only includes apartments located in Helsinki.

* total of 5853 apartments


link : https://oikotie-helsinki-restapi.herokuapp.com/ 

* Tutorial:

```python
import requests
import pandas as pd

data = requests.get('https://oikotie-helsinki-restapi.herokuapp.com/').json()
df = pd.DataFrame.from_dict(data)
print(df.head(10))

```

* result:
 (Status inactive means the apartment has been removed from the site (sold))

![result](https://github.com/aapopalkama/oikotie-helsinki-restapi/blob/c4570f38761d5e42c5e5de603babd733a2df3c3f/result.jpg) 


