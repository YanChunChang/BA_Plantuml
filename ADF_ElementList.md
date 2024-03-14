## Elemente und Relationen in ADF
### Software@Runtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Daten@Devtime und Funktionen@Devtime verwendet werden können.

| Element     | Code        | Anmerkung    |
| ----------- | ----------- | ------------ |
| ![Role](Assets/common/role.drawio.png)     | 1. ```:<<Role>>\nRole: #fff2cc``` <br>2. ```:Role: #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet.|
| ![External System](Assets/sw@rt/system.drawio.png)  | ```node "System Name" << System >> as w #fff2cc```| - |
| ![External System](Assets/sw@rt/external_system.drawio.png)  | ```node "External System Name" << External system >> as w #fff2cc```| - |
| ![Layer](Assets/sw@rt/layer.drawio.png)  | ```folder "<<Layer>> \nLayer" as l #ffe6cc {}``` | In '{}' können Komponente hinzugefügt werden. |
| ![Cluster](Assets/sw@rt/cluster.drawio.png)  | ```folder "<<Cluster>> \nCluster" as c #ffe6cc {} ```        | In '{}' können Komponente hinzugefügt werden. |
| ![Component](Assets/sw@rt/component.drawio.png)  | ```[===Component] <<Component>> as c1```   | '===' wird verwendet für Bold. |
| ![Interface Connector](Assets/sw@rt/interface_connector.drawio.png)  | 1. ```-0)-```<br> 2. ```-(0-``` | - |
| ![Interface](Assets/sw@rt/interface.drawio.png)  | ```rectangle "**Interface**" <<Interface>> as t ##ffe6cc``` | '**' wird verwendet für Bold.  |
| ![Connector](Assets/sw@rt/connector.drawio.png)  | ```Element1 <-[thickness=10]-> Element2: Connector``` | - |
| ![Data](Assets/sw@rt/data.drawio.png)  | ```rectangle "**Data**" <<Data>> as a #fff2cc{label "date \ndata1 \ndata2" }```| '**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  | ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Dataflow](Assets/sw@rt/rel_dataflow.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<dataflow>>```        |Nach '<\<dataflow>>' kann die Beschreibung noch hinzugefügt werden.|
| ![Usage](Assets/sw@rt/rel_usage.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<use>>``` | Nach '<\<use>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![System Scope](Assets/sw@rt/system_scope.drawio.png)  |  ```rectangle "System Scope" as SystemScope #line.dashed{ node "Node Name" << System >> }```|Wenn man System Scope verwendet, kann der Pfeil die System-Komponent im System Scope erreicht werden.|
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus.|
### Software@Devtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Data@Devtime und Functions@Devtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Module](Assets/sw@dt/module.drawio.png)  |  ```rectangle "**Module**" <<Module>> as m #b9e0a5``` |'**' wird verwendet für Bold. |
| ![Interface](Assets/sw@dt/interface.drawio.png)  | ```rectangle "**Interface**" <<Interface>> as t #b9e0a5``` | '**' wird verwendet für Bold.  |
| ![Package](Assets/sw@dt/package.drawio.png)  | ```package "<<Package>> \nPackage" as p #b9e0a5{ label "\n" as la1 }```  | - |
| ![Datatype](Assets/sw@dt/datatype.drawio.png)  | ```object Controller { ``` <br> ```&#43; Controller()``` <br> ```__ ``` <br> ```&#43; getData(parameters: DataRequest) : data``` <br> ```&#43; getInstance() : Object } ``` | '&\#43;' sthet für '+'. <br> '&\#8722;' steht für '-'. <br> Mit '__' kann eine neue Linie erstellt werden.
| ![Library](Assets/sw@dt/library.drawio.png)  | ```rectangle "**Library**" <<Library>> as m #b9e0a5``` |'**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  | ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Refinement](Assets/sw@dt/rel_refinement.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<refine>>```| Nach '<\<refine>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Usage](Assets/en@dt/rel_usage.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<use>>```| Nach '<\<use>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Other UML Relations](Assets/sw@dt/rel_uml_class_diagram.drawio.png)  | Asscociation : ```-``` <br> Generalization: ```-\|>```<br> Realization: ```..\|>```<br> Composition: ```*--``` <br> Aggregation: ```o--```| - |
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-``` | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus. |

### Environment@Runtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Deployment@Runtime und Activities@Runtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Computing Node](Assets/en@rt/computing_node.drawio.png)  | ```node "**Mobile Device**" <<Computing Node>> as a #ffe6cc{}```| '**' wird verwendet für Bold. |
| ![Execution Environment](Assets/en@rt/execution_environment.drawio.png)  | ```node "**App-Sandbox**" <<Execution Environment>> as e ##ffe6cc{ }``` |'**' wird verwendet für Bold.|
| ![Deployment Artifact](Assets/en@rt/deployment_artifact.drawio.png)  | ```artifact "**Mobile App**" <<Deployment Artifact>> as a #b9e0a5```| '**' wird verwendet für Bold. |
| ![Operation Process](Assets/en@rt/operation_process.drawio.png)  |```action "**Operation Process**" <<Operation Process>> as op #ffe6cc``` |'**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  |  ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Thread](Assets/en@rt/thread.drawio.png)  | ```rectangle "**Thread**" <<Thread>> as t #ffe6cc``` | '**' wird verwendet für Bold.  |
| ![Role](Assets/common/role.drawio.png)     | 1. ```:<<Role>>\nRole:``` <br>2. ```:Role: #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet.|
| ![Organizational Unit](Assets/en@rt/organizational_unit.drawio.png)  | ```node "**Web Abteilung**" <<Organizational Unit>> as a #ffe6cc{}```| '**' wird verwendet für Bold. |
| ![Operate](Assets/en@rt/rel_operate.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<operate>>```| Nach '<\<operate>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Execute](Assets/en@rt/rel_execute.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<execute>>```| Nach '<\<execute>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Deploy](Assets/en@rt/rel_deploy.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<deploy>>```| Nach '<\<deploy>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Own](Assets/en@rt/rel_own.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<own>>```| Nach '<\<own>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Manifest](Assets/en@rt/rel_manifest.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<manifest>>```| Nach '<\<manifest>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Communication Path](Assets/en@rt/rel_communication_path.drawio.png)  | ```->``` | "->" kann verlängert werden(z.B. -->). Die Linie sieht auch länger aus. |
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus. |

### Environment@Devtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Deployment@Devtime und Activities@Devtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Role](Assets/common/role.drawio.png)     | 1. ```:<<Role>>\nRole:``` <br>2. ```:Role: #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet.|
| ![Organizational Unit](Assets/en@dt/organizational_unit.drawio.png)  |```node "**Web Abteilung**" <<Organizational Unit>> as o #ffe6cc{}```| '**' wird verwendet für Bold. |
| ![Project Increment](Assets/en@dt/project_increment.drawio.png)  | ```rectangle "**Project Increment**" <<Project Increment>> as p #b9e0a5``` | '**' wird verwendet für Bold. |
| ![Deployment Artifact](Assets/en@dt/deployment_artifact.drawio.png)  | ```artifact "**Mobile App**" <<Deployment Artifact>> as a #b9e0a5```| '**' wird verwendet für Bold. |
| ![Deployment Process](Assets/en@dt/development_process.drawio.png)  | ```action "**Operation Process**" <<Operation Process>> as op #b9e0a5``` |'**' wird verwendet für Bold. |
| ![Deployment Tool](Assets/en@dt/development_tool.drawio.png)  |```node "**GitLab**" <<Deployment Tool>> as a #b9e0a5{}```| '**' wird verwendet für Bold. |
| ![Technology](Assets/common/technology.drawio.png)  | ```rectangle "**Technology**" <<Technology>> as t #f8cecc``` | '**' wird verwendet für Bold. |
| ![Manifest](Assets/en@dt/rel_manifest.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<manifest>>```| Nach '<\<manifest>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Usage](Assets/en@dt/rel_usage.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<use>>```| Nach '<\<use>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Own](Assets/en@dt/rel_own.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<own>>```| Nach '<\<own>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --). Die Linie sieht auch länger aus. |