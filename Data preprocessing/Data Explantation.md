# 4. Data explantation:

De methode data-analyse is tijdens het onderzoek meerder malen toegepast. Als eerst in dit onderzoek is de methode data-analyse toegepast op het verkregen data set. De dataset bestaat uit een Excel bestand met daarin verschillende gegevens van klanten zoals: procesdag, cust_id, aantal pakketten en het aantal pakketten voor de volgende dag. Met behulp van de methode is het gelukt om de informatie in de dataset te begrijpen en toe te passen. 

Bij de procesdag werd de gewenste dagen gefilterd dit werd gedaan met de volgende code:
```python
date_filter = data['procesdag'].dt.dayofweek <= 4
```
Hier zijn de weekenden eruit gefilterd, omdat deze klant niks verstuurde in het weekend.

Bij cust id werd de gewenst klant gefilterd dit werd gedaan met de volgende code:
```python
cust_filter = data['cust_id'] == 'klant_289'
```

Aantal pakketten spreekt voor zich, hier wordt aangegeven hoeveel pakketten er zijn in de dataset. En tot slot bij aantal pakketten volgende dag staat er informatie voor de volgende dag. Zie [afbeelding](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/afbeeldingen/uitleg%20289.PNG) om het overzichtelijker te maken.

