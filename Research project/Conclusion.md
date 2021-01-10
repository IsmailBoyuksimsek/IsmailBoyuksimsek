# 3. Conclusies

Hoe kan PostNL machine learning modellen toe passen, om te voorspellen hoeveel pakketten er voor de volgende dag verwerkt moeten worden? Om deze vraag te kunnen beantwoorden is er in het begin van deze project een lijst opgesteld met [timeseriemoddelen](https://machinelearningmastery.com/time-series-forecasting-methods-in-python-cheat-sheet/).  De meest relevante modellen voor deze project zou de volgende modellen zijn:
•	AutoRegression (AR) 
•	Autoregressive Moving Average (ARMA)
•	Autoregressive Integrated Moving Average (ARIMA)
•	Seasonal Autoregressive Integrated Moving-Average (SARIMA)


Allereerst ben ik begonnen met een [Auto Regressive model](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/afbeeldingen/AR%20Model.PNG). Dit is een simpel model, deze model sluite niet helemaal aan op mijn klant. hierna heb ik de model aangepast naar een [ARMA](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/afbeeldingen/ARMA%20model.PNG). Bij deze model was de resultaat heel slecht, dus heb ik het model aangepast naar [ARIMA](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/afbeeldingen/ARIMA%20model.PNG) zodat het model stationair werd. Deze model was al wat beter dan de voorgaande moddelen, maar de pieken waren nog niet goed te voorspellen. Tot slot is de model verwerkt naar [SARIMA model](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/afbeeldingen/SARIMA%20model.PNG). SARIMA is mijn eindresultaat, deze model is de best passende timeseriemodel. 

SARIMA is uitgevoerd en geoptimaliseerd bij verschillende klanten. Deze model is de meest geschikte tijd serie model voor PostNL, dit is zowel van mijn perspectief als die van Tim Ottens. Hiermee gaat PostNL deze modellen verder uitwerken bij verschillende klanten,  evalueren en uitvoeren in de praktijk. Het doel van PostNL is hiermee de kosten te verlagen door betere planning, minder mankrachten en meer efficiëntie.

