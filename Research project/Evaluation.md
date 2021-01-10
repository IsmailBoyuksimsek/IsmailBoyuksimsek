# 2. Evaluation

Na een traject van een half jaar heb ik de opgestelde hoofd -en deelvragen kunnen beantwoorden met mijn projectgroepje. De hoofdvraag was

•	Hoe kan PostNL machine learning modellen toe passen, om te voorspellen hoeveel pakketten er voor de volgende dag verwerkt moeten worden

Na de experimenten is gebleken dat twee soorten modellen als beste het aantal pakketten kunnen voorspellen:
-	Multivariate Linear Regression
-	SARIMA

### Multivariabele lineaire regressie

Uit de experimenten blijkt, dat het model over het algemeen goede voorspellingen levert voor de meeste dagen binnen de test set. Ondanks het model goed presteert op de meeste consistente tijdsintervallen, zijn de voorspellingen niet zo goed op bepaalde inconsistente dagen die afwijken van het algemene patroon van de data. Dit is vooral bij de maanden: December en Mei goed te zien, die voornamelijk onverwachtse pieken en dalen bevatten. Verder is aan de resultaten ook te zien dat er negatieve [voorspellingen](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/afbeeldingen/MVLR%20model.PNG) tussen zitten. Dit komt omdat de features geschaald zijn met een StandardScaler, daarop voorspellingen zijn gebaseerd en die voorspellingen terug zijn geschaald naar de daadwerkelijke waardes. Aangezien het aantal pakketten niet negatief kan zijn, kan er besloten worden om deze negatieve voorspellingen af te leiden naar nul.

### SARIMA

SARIMA modellen zijn uitgevoerd en geoptimaliseerd bij specifieke klanten zie [Conclusion](https://github.com/IsmailBoyuksimsek/IsmailBoyuksimsek/blob/main/Research%20project/Conclusion.md). PostNL heeft deze modellen uitgeroepen als beste modellen voor het voorspellen van het aantal pakketjes van de voor de volgende dag.

Hiermee gaat PostNL in de toekomst deze modellen verder uitwerken bij verschillende klanten,  evalueren en uitvoeren in de praktijk. Het doel van PostNL is hiermee de kosten te verlagen door betere planning, minder mankrachten en meer efficiëntie. Wanneer dit is gedaan is er een model dat het aantal pakketten voor de volgende of zelfs nog meer in de toekomst de pakketten voorspelt. 

