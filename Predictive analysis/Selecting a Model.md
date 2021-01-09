Selecteren van een model

Nadat we de dataset met 300 klanten hadden gekregen was de groep onderverdeeld in 2 groepjes. Eén groep ging aan de slag met multiverate lineaire regression en de andere groep ging aan de slag met tijdseriemodellen. Met twee andere groepsleden ging ik aan de slag met tijdseriemodellen. Allereerst is er een lijst van elf tijdseriemodellen geselecteerd: 

1.	Autoregression (AR)
2.	Moving Average (MA)
3.	Autoregressive Moving Average (ARMA)
4.	Autoregressive Integrated Moving Average (ARIMA)
5.	Seasonal Autoregressive Integrated Moving-Average (SARIMA)
6.	Seasonal Autoregressive Integrated Moving-Average with Exogenous Regressors (SARIMAX)
7.	Vector Autoregression (VAR)
8.	Vector Autoregression Moving-Average (VARMA)
9.	Vector Autoregression Moving-Average with Exogenous Regressors (VARMAX)
10.	Simple Exponential Smoothing (SES)
11.	Holt Winter’s Exponential Smoothing (HWES)

Nadat is er een selectie gemaakt met de meest bruikbare modellen voor de opdracht. Hieruit kwam naar voren dat er tijdens dit project gebruik zou gemaakt worden van de volgende tijdseriemodellen:

•	AutoRegression (AR) 
De Moving Average methode modelleert de volgende stap in de reeks als een lineaire functie van een gemiddeld proces in eerdere tijdstappen en eerdere foutmarges. De lineaire functie hangt dus af van voorafgaande waardes uit het verleden.
•	Autoregressive Moving Average (ARMA)
ARMA is een mix van AR& MA 
Voor- en/of Nadelen: het is niet stationair wat neerkomt dat het niet geschikt is voor modellen met trends en seizoen componenten
•	Autoregressive Integrated Moving Average (ARIMA)
ARIMA is een mix van AR & MA, maar r komt integratie(I) bij om het model stationair te maken
•	Seasonal Autoregressive Integrated Moving-Average (SARIMA)
SARIMA is een mix van AR & MA, maar r komt integratie(I) bij om het model stationair te maken. En een S bij om seizoen componenten geschikt te maken voor het model

