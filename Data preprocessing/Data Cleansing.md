#2. Gegevens opschonen
##De student heeft de data op een goede en voldoende manier opgeschoond.

de dataset waar er gegevens van 300 klanten inzaten hadden we opgeschoond. Klant 289 was een latere klant bij PostNL, dus deze klant moest vanaf 2016-01-01 beginnen met voorspellen. Om dit daadwerkelijk te kunnen realiseren moest de er gefilterd worden. Dit is gedaan door de volgende codes:
```python
cust_filter = data['cust_id'] == 'klant_289'
date_filter = data['procesdag'].dt.dayofweek <= 4
data = data.where(date_filter & cust_filter).dropna()
#data = data.where(cust_filter).dropna()

data['procesdag']=pd.to_datetime(data['procesdag'])
data = data.set_index(data.procesdag, drop=True)
data = data['2016-01-01':'2020-01-01']
```

zie [afbeelding](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/afbeeldingen/filteren%20289.PNG) voor de resultaat.
