## Elemente und Relationen in ADF
Auf dieser Seite https://github.com/architecture-decomposition-framework/welcome-to-adf/blob/main/adf-elements/ADF-elements.md finden Sie eine Liste aller Elemente und Relationen in ADF.
Zusätzlich gibt es eine Beschreibung für jedes Element.
Diese Datei zeigt alle Elemente in PlantUML mit einem Beispielcode.

Diese Liste dient der schnellen Übersicht über alle Elemente. Deshalb ist der Farbcode noch nicht global definiert. Wenn Sie schnell etwas erstellen wollen, können Sie den Code kopieren. Wenn man die Elemente mit Farben global definieren will, dann findet man den Ordner Color-Element, in dem alle Elemente mit Farbe global mit skinparam definiert wurden.


Alternativ kann der Code '!include color.plantuml' an den Anfang der Datei geschrieben werden, um den Zugriff auf den Farbcode zu ermöglichen. Ersetzen Sie z.B. #fff2cc durch Yellow.
### Software@Runtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Daten@Devtime und Funktionen@Devtime verwendet werden können.

| Element     | Code        | Anmerkung    |
| ----------- | ----------- | ------------ |
| ![Role](Assets/common/role.drawio.png)     | 1. ```:<<Role>>\n**Role**: as r #fff2cc``` <br>2. ```:Role: as r #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet. 3. '**' wird verwendet für Bold.|
| ![External System](Assets/sw@rt/system.drawio.png)  | ```node "**System**" <<System>> as s #fff2cc```|'**' wird verwendet für Bold.|
| ![External System](Assets/sw@rt/external_system.drawio.png)  | ```node "**External System**" <<External System>> as es #fff2cc```|'**' wird verwendet für Bold.|
| ![Layer](Assets/sw@rt/layer.drawio.png)  | ```folder "<<Layer>> \n**Layer**" as f #ffe6cc {}``` | 1. Um die Überschrift des Elements richtig zu platzieren, muss ein Element in '{}' geschrieben werden. 2. Alternativ kann man 'label "\n"'hinzufügen. Es sieht besser aus, wenn sich kein Element innerhalb des Layers befindet. |
| ![Cluster](Assets/sw@rt/cluster.drawio.png)  | ```folder "<<Cluster>> \n**Cluster**" as c #ffe6cc {} ```  | 1. Um die Überschrift des Elements richtig zu platzieren, muss ein Element in '{}' geschrieben werden.<br> 2. Alternativ kann man 'label "\n"'hinzufügen. Es sieht besser aus, wenn sich kein Element innerhalb des Clusters befindet. |
| ![Component](Assets/sw@rt/component.drawio.png)  | ```Component "**Component**" <<Component>> as c fff2cc```   | '**' wird verwendet für Bold. |
| ![Interface Connector](Assets/sw@rt/interface_connector.drawio.png)  | 1. ```-0)-```<br> 2. ```-(0-``` | Für Pfeilbeschriftung: '-0)- :use' |
| ![Interface](Assets/sw@rt/interface.drawio.png)  | ```rectangle "**Interface**" <<Interface>> as t ##ffe6cc``` | '**' wird verwendet für Bold.  |
| ![Connector](Assets/sw@rt/connector.drawio.png)  | ```Element1 <-[thickness=10]-> Element2: Connector``` | - |
| ![Data](Assets/sw@rt/data.drawio.png)  | ```rectangle "**Data**" <<Data>> as a #fff2cc{label "date \ndata1 \ndata2" }```| '**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  | ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Dataflow](Assets/sw@rt/rel_dataflow.drawio.png)  | ```Element1 ..> Element2  :<<dataflow>>```        |Für Pfeilbeschriftung: ':<\<dataflow>> dataflow'|
| ![Usage](Assets/sw@rt/rel_usage.drawio.png)  | ```Element1 ..> Element2  :<<use>>``` | Für Pfeilbeschriftung: ':<\<use>> use' |
| ![System Scope](Assets/sw@rt/system_scope.drawio.png)  |  ```rectangle "System Scope" as SystemScope #line.dashed{ node "System Name" <<System>> }```|Wenn man System Scope verwendet, kann der Pfeil die System-Komponent im System Scope erreicht werden.|
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus.|
### Software@Devtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Data@Devtime und Functions@Devtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Module](Assets/sw@dt/module.drawio.png)  |  ```rectangle "**Module**" <<Module>> as m #b9e0a5``` |'**' wird verwendet für Bold. |
| ![Interface](Assets/sw@dt/interface.drawio.png)  | ```rectangle "**Interface**" <<Interface>> as i #b9e0a5``` | '**' wird verwendet für Bold.  |
| ![Package](Assets/sw@dt/package.drawio.png)  | ```package "<<Package>> \n**Package**" #b9e0a5{ 'Elemente hinzufügen }```  |1. Wenn 'as xxx' geschrieben wird, muss unbedingt ein Element in {} eingefügt werden, da sonst die Überschrift nicht mehr korrekt positioniert ist.<br> 2. Alternativ kann man 'label "\n"'hinzufügen. Es sieht besser aus, wenn sich kein Element innerhalb des Packages befindet.|
| ![Datatype](Assets/sw@dt/datatype.drawio.png)  | ```object Datatype <<Datatype>>{ ``` <br> ```&#43; field: Type``` <br> ```__ ``` <br> ```&#43; constructor(): Type``` <br> ```__ ``` <br> ```&#43; method():Type } ``` | '&\#43;' sthet für '+'. <br> '&\#8722;' steht für '-'. <br> Mit '__' kann eine neue Linie erstellt werden.
| ![Library](Assets/sw@dt/library.drawio.png)  | ```rectangle "**Library**" <<Library>> as l #b9e0a5``` |'**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  | ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Refinement](Assets/sw@dt/rel_refinement.drawio.png)  | ```Element1 .> Element2  :<<refine>>```| Für Pfeilbeschriftung: ':<\<refine>> refine'  |
| ![Usage](Assets/en@dt/rel_usage.drawio.png)  | ```Element1 .> Element2  :<<use>>```| Für Pfeilbeschriftung: ':<\<use>> use'  |
| ![Other UML Relations](Assets/sw@dt/rel_uml_class_diagram.drawio.png)  | Asscociation : ```-``` <br> Generalization: ```-\|>```<br> Realization: ```..\|>```<br> Composition: ```*--``` <br> Aggregation: ```o--```| - |
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-``` | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus. |

### Environment@Runtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Deployment@Runtime und Activities@Runtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Computing Node](Assets/en@rt/computing_node.drawio.png)  | ```node "**Computing Node**" <<Computing Node>> as cn #ffe6cc{}```| '**' wird verwendet für Bold. |
| ![Execution Environment](Assets/en@rt/execution_environment.drawio.png)  | ```node "**Execution Environment**" <<Execution Environment>> as ee ##ffe6cc{ }``` |'**' wird verwendet für Bold.|
| ![Deployment Artifact](Assets/en@rt/deployment_artifact.drawio.png)  | ```artifact "**Deployment Artifact**" <<Deployment Artifact>> as da #b9e0a5```| '**' wird verwendet für Bold. |
| ![Operation Process](Assets/en@rt/operation_process.drawio.png)  |```action "**Operation Process**" <<Operation Process>> as op #ffe6cc``` |'**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  |  ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Thread](Assets/en@rt/thread.drawio.png)  | ```rectangle "**Thread**" <<Thread>> as t #ffe6cc``` | '**' wird verwendet für Bold.  |
| ![Role](Assets/common/role.drawio.png)     | 1. ```:<<Role>>\n**Role**: as r #fff2cc``` <br>2. ```:Role: as r #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet. 3. '**' wird verwendet für Bold.|
| ![Organizational Unit](Assets/en@rt/organizational_unit.drawio.png)  | ```node "**Organizational Unit**" <<Organizational Unit>> as a #ffe6cc{}```| '**' wird verwendet für Bold. |
| ![Operate](Assets/en@rt/rel_operate.drawio.png)  | ```Element1 .> Element2  :<<operate>>```| Für Pfeilbeschriftung: ':<\<operate>> operate'  | 
| ![Execute](Assets/en@rt/rel_execute.drawio.png)  | ```Element1 .> Element2  :<<execute>>```| Für Pfeilbeschriftung: ':<\<execute>> execute'  | 
| ![Deploy](Assets/en@rt/rel_deploy.drawio.png)  | ```Element1 .> Element2  :<<deploy>>```| Für Pfeilbeschriftung: ':<\<deploy>> deploy'  | 
| ![Own](Assets/en@rt/rel_own.drawio.png)  | ```Element1 .> Element2  :<<own>>```| Für Pfeilbeschriftung: ':<\<own>> own'  | 
| ![Manifest](Assets/en@rt/rel_manifest.drawio.png)  | ```Element1 .> Element2  :<<manifest>>```| Für Pfeilbeschriftung: ':<\<manifest>> manifest'  |
| ![Communication Path](Assets/en@rt/rel_communication_path.drawio.png)  | ```->``` | "->" kann verlängert werden(z.B. -->). Die Linie sieht auch länger aus. |
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus. |

### Environment@Devtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Deployment@Devtime und Activities@Devtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Role](Assets/common/role.drawio.png)     | 1. ```:<<Role>>\n**Role**: as r #fff2cc``` <br>2. ```:Role: as r #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet. 3. '**' wird verwendet für Bold.|
| ![Organizational Unit](Assets/en@dt/organizational_unit.drawio.png)  |```node "**Organizational Unit**" <<Organizational Unit>> as ou #ffe6cc{}```| '**' wird verwendet für Bold. |
| ![Project Increment](Assets/en@dt/project_increment.drawio.png)  | ```rectangle "**Project Increment**" <<Project Increment>> as pi #b9e0a5``` | '**' wird verwendet für Bold. |
| ![Deployment Artifact](Assets/en@dt/deployment_artifact.drawio.png)  | ```artifact "**Deployment Artifact**" <<Deployment Artifact>> as da #b9e0a5```| '**' wird verwendet für Bold. |
| ![Deployment Process](Assets/en@dt/development_process.drawio.png)  | ```action "**Deployment Process**" <<Deployment Process>> as dp #b9e0a5``` |'**' wird verwendet für Bold. |
| ![Deployment Tool](Assets/en@dt/development_tool.drawio.png)  |```node "**Deployment Tool**" <<Deployment Tool>> as dt #b9e0a5{}```| '**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  | ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Manifest](Assets/en@dt/rel_manifest.drawio.png)  | ```Element1 .> Element2  :<<manifest>>```| Für Pfeilbeschriftung: ':<\<manifest>> manifest'  |
| ![Usage](Assets/en@dt/rel_usage.drawio.png)  | ```Element1 .> Element2  :<<use>>```| Für Pfeilbeschriftung: ':<\<use>> use'  |
| ![Own](Assets/en@dt/rel_own.drawio.png)  | ```Element1 .> Element2  :<<own>>```| Für Pfeilbeschriftung: ':<\<own>> own'  | 
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus. |