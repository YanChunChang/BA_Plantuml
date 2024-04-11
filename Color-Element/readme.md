## Elemente mit Farben
In der entsprechenden Datei werden alle Elemente farbig dargestellt. Man kann den Code von skinparam und die entsprechenden Elemente erzeugen. Und vergessen Sie nicht !include color.plantuml zu schreiben, um die vordefinierte Farbe zu verwenden. 

In einigen Ausnahmefällen kann die Farbe nicht global mit skinparam definiert werden. In solchen Fällen schreibt man die Farbe einfach hinter das Element oder verwendet style am Anfang des Diagramms. Der Unterschied zwischen style und skinparam besteht darin, dass innerhalb von style die Bezeichnungen wie <\<System>> oder <\<Interface>> nicht wie bei skinparam funktionieren. Außerdem gibt es einige Elemente wie action oder artifact, für die skinparam nicht verwendet werden kann.

Sonderfälle sind Cluster und Folder. Man muss ein Element in '{}' schreiben, sonst wird die Überschrift des Elements nicht richtig platziert.

Datatype in Software@Devtime kann jedoch nicht mit anderen Elementen abgebildet werden, daher eine separate Datei.