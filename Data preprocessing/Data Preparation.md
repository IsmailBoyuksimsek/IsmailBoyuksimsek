# 3. Datavoorbereiding

## De student heeft de data op een gepaste manier voorbereid, waar nodig data getransformeerd, uitschieters verwijderd, ontbrekende waarden ingevuld, etc.

In de vorige hoofdstuk is er uitgelegd dat de data gefilterd moest worden. Het alleen filteren van de data is niet genoeg voorbereiding, want uit deze [grafiek](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/python%20codes/Untitled7.ipynb) is te zien dat in het weekend geen pakketten worden verstuurd. De voorspelling zou niet meer kloppen als er in het weekenden niks zou worden verstuurd, want als er ineens niet meer word verstuurd zou de model voor de volgende dag de voorspelling niet goed voorspellen. Door deze oorzaak is de weekend voor deze klant met de volgende code eruit gefilterd.
```Python
cust_filter = data['cust_id'] == 'klant_289'
date_filter = data['procesdag'].dt.dayofweek <= 4
data = data.where(date_filter & cust_filter).dropna()
#data = data.where(cust_filter).dropna()

data['procesdag']=pd.to_datetime(data['procesdag'])
data = data.set_index(data.procesdag, drop=True)
data = data['2016-01-01':'2020-01-01']
```
