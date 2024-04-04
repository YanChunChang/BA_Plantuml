## Die Erklärung zur Positionierung im PlantUML
Unter dieser Adresse finden Sie allgemeine Informationen zur Positionierung: https://crashedmind.github.io/PlantUMLHitchhikersGuide/layout/layout.html

PlantUML bietet von Natur aus bereits automatische Positionierung. 
Allerdings ist diese nicht immer optimal dargestellt.
Daher sind insbesondere die folgenden Eigenschaften wichtig:

1. Generell im PlantUML gilt: </br>
--> geht von oben nach unten</br>
-> geht von links nach rechts</br>
Je länger der "-", desto länger der Pfeil</br>


2. Wenn man extra Positionangabe gibt sowie:</br>
-u-> up</br>
-d-> down</br>
-r-> right</br>
-l-> left</br>
Die Elemente können durch den Befehl 'Manuell' positionieren.

3. left to right direction:</br>
Standardmäßig ist die Richtung des Diagramms von oben nach unten.(top to bottom direction)</br>
Das Ändern der Richtung des Diagramms kann manchmal helfen, die Elemente des Diagramms besser zu positionieren.(Siehe Beispiel 1 und 2 in der Tabelle)</br>

In diesem Ordner finden Sie drei Beispiele mit drei unterschiedlichen Schreibweisen, die jedoch alle zum gleichen Ergebnis führen. (Siehe Beispiel 3, 4, und 5 im Ordner)

Bei der Positionierung ist es wichtig, die **Reihenfolge der Elemente** zu beachten, da dies das Layout beeinflusst. Auch die **Richtung der Verbindung** (a --> b und b <-- a) kann einen Unterschied machen.

### Anmerkung:
Beim Zeichnen von Diagrammen mit PlantUML ist es manchmal leider schwierig zu entscheiden, welche Reihenfolge oder Verbindungsrichtung 'richtig' ist.  Es gibt keinen eindeutig richtigen Weg, das Diagramm zu erstellen. Dies ist ähnlich wie bei der Programmierung. Es gibt mehrere Wege, um ein Ziel zu erreichen.


| Nr.         | Beispiel    |
| ----------- | ----------- | 
|1|![Mapping runtime to devtime](https://www.plantuml.com/plantuml/svg/dLH1Jy8m6BttLtp2mOG3OHiRQ80GIV14D7emndYetRVHh6kNqac8yj_jnjm8S9X-X-RrzRNVUstI-SPGRV9Km8fc6PSnw5mQdY8O1I5-5f1SXHXnYV2AGgWjTACeSXchwNkDAA7xSOC3wjVi8vT9AHtWk2QVCBJScE7HzWTDPOo558CZ-cNDJSaMHSYrmCWKfZIFrmP2hf4PhYJP95ncLDCKu8k0BQRIJ4cKffeNjLJIF9kTG91AfrJK2tUK9R5MkGmNIYXTHIoNz-LOjB7-xCv_d5RUJ7NOtcPmRXtoDfrELxl5hybtc4pgoMm6T0FC8KtNJg-tsgrKc0lizJfMVC07PUeGvi3akz-t4Ce6iaq3jtM3C-NItZHkbKukY3t2tCgD2mts2cVoFBfpoPftgd8lgOQdAk-IocyTSqYOLxaTMkV38-mtk4YHjaeHj4enQktF_yip18G5bMaV6XnOF3hYHmrFvYX3-mdy0000 "Mapping runtime to devtime")|
|2|![Mapping runtime to devtime](https://www.plantuml.com/plantuml/svg/dLHTJy8m57tlhxZ2WmaFX7s21WYH19-8HX-CCJxKxcuqszgbT1AY_7UxmUO2UvZUXwRdtDFUSxfaYwscIkTf0ckQPLn4e7AXUOgW9GJuMMp9LO0X5mYlc2Ho1_qm36t6QlfU8GheVzpWY7er-yX5N4f7EAd99mmCDs7OEFwWg8YmaABVe5ysN9TiKIJ1K1UM58ys6WAka6ak1Td6N6HKqHJWYu0f9jDC2XJwX8jQIQ6VzJv145AbDAaRTvJ5aPAv29OoaUeKi6mVohKOOzoPa_-uhNoNqsK7GgwjMukypMQpzNvPcNo7wRG6ypdGBJ2B_4xj3GRh_Le6UOA3GS-8Z_kZChK8is3wFGo6PW_50D5bWDrvm8LoPLuQTrB5BMA7CBjoOqC3E632YylmLfivvrnbjwdSSvNJfl8w1tK9Sogxhl7kDe7N04MGj5CGlrEGSMUBtb--XK-ONxdse05y0yRDphZH8GiKWVaN_000 "Mapping runtime to devtime")|
