## Elemente und Relationen in ADF
### Software@Runtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Daten@Devtime und Funktionen@Devtime verwendet werden können.

| Element     | Code        | Anmerkung    |
| ----------- | ----------- | ------------ |
| ![Role](Assets/common/role.drawio.png)     | 1. ```: <<Role>>\nRole:``` <br>2. ```:Role: #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet.|
| ![External System](Assets/sw@rt/system.drawio.png)  | ```node "System Name" << System >> as w #fff2cc```| - |
| ![External System](Assets/sw@rt/external_system.drawio.png)  | ```node "External System Name" << External system >> as w #fff2cc```| - |
| ![Layer](Assets/sw@rt/layer.drawio.png)  | Text        | txt |
| ![Cluster](Assets/sw@rt/cluster.drawio.png)  | Text        | txt |
| ![Component](Assets/sw@rt/component.drawio.png)  | Text        | txt |
| ![Interface Connector](Assets/sw@rt/interface_connector.drawio.png)  | ```-0)-``` | - |
| ![Interface](Assets/sw@rt/interface.drawio.png)  | Text        | txt |
| ![Connector](Assets/sw@rt/connector.drawio.png)  | ```Element1 <-[thickness=10]-> Element2: Connector``` | - |
| ![Data](Assets/sw@rt/data.drawio.png)  | ```rectangle "Data" <<Data>> as a #fff2cc{label "date \nmeal \nprice \ncoldBowlProbability" }```| - |
| ![Technology](Assets/common/technology.drawio.png)  | Text        | txt |
| ![Dataflow](Assets/sw@rt/rel_dataflow.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<dataflow>>```        |Nach '<\<dataflow>>' kann die Beschreibung noch hinzugefügt werden.|
| ![Usage](Assets/sw@rt/rel_usage.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<use>>``` | Nach '<\<use>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![System Scope](Assets/sw@rt/system_scope.drawio.png)  |  ```rectangle "System Scope" as SystemScope #line.dashed{ node "Node Name" << System >> }```|Wenn man System Scope verwendet, kann der Pfeil die System-Komponent im System Scope nicht erreicht werden.|
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --), sieht die Linie auch länger aus. |
### Software@Devtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Data@Devtime und Functions@Devtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Module](Assets/sw@dt/module.drawio.png)  | Text        |
| ![Interface](Assets/sw@dt/interface.drawio.png)  | Text        |
| ![Package](Assets/sw@dt/package.drawio.png)  | Text        |
| ![Datatype](Assets/sw@dt/datatype.drawio.png)  | Text        |
| ![Library](Assets/sw@dt/library.drawio.png)  | Text        |
| ![Technology](Assets/common/technology.drawio.png)  | Text        |
| ![Refinement](Assets/sw@dt/rel_refinement.drawio.png)  | Text        |
| ![Usage](Assets/en@dt/rel_usage.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<use>>```| Nach '<\<use>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Other UML Relations](Assets/sw@dt/rel_uml_class_diagram.drawio.png)  | Text        | txt|
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --), sieht die Linie auch länger aus. |

### Environment@Runtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Deployment@Runtime und Activities@Runtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Computing Node](Assets/en@rt/computing_node.drawio.png)  | Text        |
| ![Execution Environment](Assets/en@rt/execution_environment.drawio.png)  | Text        |
| ![Deployment Artifact](Assets/en@rt/deployment_artifact.drawio.png)  | Text        |
| ![Operation Process](Assets/en@rt/operation_process.drawio.png)  | Text        |
| ![Technology](Assets/common/technology.drawio.png)  | Text        |
| ![Thread](Assets/en@rt/thread.drawio.png)  | Text        |
| ![Role](Assets/common/role.drawio.png)     | 1. ```: <<Role>>\nRole:``` <br>2. ```:Role: #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet.|
| ![Organizational Unit](Assets/en@rt/organizational_unit.drawio.png)  | Text        |
| ![Operate](Assets/en@rt/rel_operate.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<operate>>```| Nach '<\<operate>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Execute](Assets/en@rt/rel_execute.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<execute>>```| Nach '<\<execute>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Deploy](Assets/en@rt/rel_deploy.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<deploy>>```| Nach '<\<deploy>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Own](Assets/en@rt/rel_own.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<own>>```| Nach '<\<own>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Manifest](Assets/en@rt/rel_manifest.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<manifest>>```| Nach '<\<manifest>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Communication Path](Assets/en@rt/rel_communication_path.drawio.png)  | ```->``` | "->" kann verlängert werden(z.B. -->), sieht die Linie auch länger aus. |
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --), sieht die Linie auch länger aus. |

### Environment@Devtime
#### Die folgende Tabelle zeigt die Elemente, die in Ansichten vom Typ Deployment@Devtime und Activities@Devtime verwendet werden können.

| Element     | Code        | Anmerkung   |
| ----------- | ----------- | ----------- |
| ![Role](Assets/common/role.drawio.png)     | 1. ```: <<Role>>\nRole:``` <br>2. ```:Role: #fff2cc``` | 1. '\n' dient dazu, dass es so wie im Bild aussieht. Ansonsten kann man auch '<\<Role>>\n' weglassen.<br> 2. 'Role' wird ohne '<\<Role>>' abgebildet.|
| ![Organizational Unit](Assets/en@dt/organizational_unit.drawio.png)  | Text        |
| ![Project Increment](Assets/en@dt/project_increment.drawio.png)  | Text        |
| ![Deployment Artifact](Assets/en@dt/deployment_artifact.drawio.png)  | Text        |
| ![Deployment Process](Assets/en@dt/development_process.drawio.png)  | Text        |
| ![Deployment Tool](Assets/en@dt/development_tool.drawio.png)  | Text        |
| ![Technology](Assets/common/technology.drawio.png)  | Text        |
| ![Manifest](Assets/en@dt/rel_manifest.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<manifest>>```| Nach '<\<manifest>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Usage](Assets/en@dt/rel_usage.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<use>>```| Nach '<\<use>>' kann die Beschreibung noch hinzugefügt werden.  |
| ![Own](Assets/en@dt/rel_own.drawio.png)  | ```Element1 --> Element2  #black;line.dashed;:<<own>>```| Nach '<\<own>>' kann die Beschreibung noch hinzugefügt werden.  | 
| ![Note](Assets/common/note.drawio.png)  | ```note "This note is a note." as n #ffffff```| - |
| ![Note Relation](Assets/common/rel_note.drawio.png)  | ```-```      | "-" kann verlängert werden(z.B. --), sieht die Linie auch länger aus. |