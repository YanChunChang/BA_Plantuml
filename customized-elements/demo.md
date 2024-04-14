## Demo für Define und Procedure
### Methode 1 !Define
Code für diese Diagram, finden Sie in "customized-elements/system-context.plantuml und withDefine.plantuml".

![!define](https://www.plantuml.com/plantuml/svg/lLRVRzem47xtN-6bao0ee9N72L1HH_SqhIhTCtAJIshLiIFRZD2k__lE8Ga9FwQjrU87v9pllk-pp_ZkobYcxJeLz4C4CPT0Y7dYCcEQfLH3Q9bC1D0NGd7SA6cNTelVKkcK2V9AI6yX80LfWPG0TBar5j8-h9ZWp0GKLe8zWF0RSDvWK5e70uzE9hkGsOmoGyiuUX77yJWCQzX5Ra5B9bPlmAzYwTyGxNnMor1bKB4SWEzSQE7Y61fez48Wo2XYvX6Y6lDQfPcIU4p_9BkEQWkk5PFU7GXckPBcaMUcPaFhweTnuerQwn3c5IFcEW4xRmbmauWx4OWpzJoVjiAQgsq4-XabhWtCPYLIY_yBiomMQjE5YAZaEgtahfXseKCNJATLVCz0Czk93BMZEgrZaKEuxaO7xAZEt0_8XDfsSZiAfZDPsSXEChAHf_c_CSbZCBOB4Md9jLVIalB_9PmwWAyWyR8A_bmyOwZXHglKaTohchEWAIMUM0weD_mry_o3F_sxGKUZ8zJYGJRyFQY3uV00T9ua6f9tILL7eDTAIao3qcy-qa_-q6sVz285HbgwKVg9zAesGIYPq8Mqt6wFIfgRO7tKK03cbyNlsCVWHgcRJajlL-Wg_rQTUy40Do3lDr0EosK-_cE9po_hQjcZhqu_o6Y_1TpUHpXeBEuttAB59wr6W5NV_OU0pbFshAHF3dkICA2tR7lBX4_s5JyAw1BqJnv2qme1DWNIQYM4uofomGAAuDvamcKerX6-d5v0HwFPRdcVKdGA0mzBhrS6eY4w7-YMuVnoqIau0BIXgHXNU4hO5Fu6 "!define")

### Problemstellung für Define-Art
1. Im PlantUML Language Reference Guide, Kapitel 25.23 Migration notes, wird beschrieben, dass !Define nicht mehr verwendet werden sollte. Auch wenn es funktioniert.
2. Es funktionierte nicht, wenn mehrere Elemente verschachtelt wurden. Auch in Archimate-Repo wurde die Verschachtelung von Elementen nicht verwendet.

** ArchiMate ist eine Modellierungssprache für Enterprise-Architekturen. ArchiMate-Repo ist ein Repository, das ArchiMate-Diagramme in PlantUML umsetzen kann. 
### Methode 2 !Procedure
Code für dieses Diagramm, finden Sie in "customized-elements/withProcedure.plantuml".

![test Procedure](https://www.plantuml.com/plantuml/svg/VPJRZfim48Rl_HGJYWH4KINsiahGjjdkNQLARAzN4p34Mh0ZsxHTHNcptlN5Qfj38D2WWEAPttFuV7XK6gLkwWeqLHg-Iv7Hl96KaDMf_mz-hShGLwAH6Ts0dnibuwYPu141w1pmiKecFlYqtUQeiQZ4hoGXAyhpqt9u-bjJoR5wLUzAqphqiMAe8gBU63-Xn1hE9W-0f9b6NbQq6zldMN2TwdTZuqBMM0sEBvYzbL8qFD-BIaZuK1J5GvOv_uMOtueL4DxcXjKEF2zogfLlR2zOAjZDQZJjL8hEPC7NJWQfamMkRLOGSgrzlMxxMwzXkxtH9mcWWiEPaCizOEcOarcHJDGdmIdNEyyR3-DTsyijo6MKTs3Un-c0cjTyMgX30LESrcn0MPo3miuPeRnAWdql2PocnJZB42-cY2SvukKaLXHSHQCqOpwJvHgl4lRaVCppeTYmZnxTzSQH8tQpnfD5dixhZiH_AnkaIN9U3DrlcXTpGZVmkT77bCgVp9xe7uhARX2HsMbyPf8UK5cNlGSE6um82PuC0MPkZEBl7mdx2fM29uQbsMCaW74RZ3Fzcbb1w7EiJPZ0K746S0Qp0uCngLhmRrGVHHwsqeiDE6rccc5vcXQfbeoNtV28whWNENN3MRXnbLuXHEn52zQ7rcefjA8Dz6RoQ4AQQ_GV "test Procedure")

### Problemstellung für Procedure-Art
1. Alternativ zu !Define kann !Procedure verwendet werden. Wie in der Abbildung gezeigt, ist eine Verschachtelung möglich. Es ist machbar, aber sehr zeitaufwendig.
2. Es gibt noch ein weiteres Problem. Wenn man sich diesen Code ```!procedure $System($alias, $component="", $component1="")``` (withProcedure.plantuml) anschaut, braucht man für diese "Funktion" $system noch 3 weitere "Parameter". Das bedeutet, dass man in diesem Block nur 2 Komponenten hinzufügen kann. Wenn man mehr Komponenten braucht, muss man den Code erweitern, was natürlich nicht so flexibel und dynamisch ist.
3. Wenn man es trotzdem flexibel und dynamisch machen will, muss man es wie C4-Repo machen. In diesem Repo sind aber sehr viele Codes und die Codes sind nicht überschaubar, oft sind sie miteinander verschachtelt.

** $alias ist der Name für das System.
### Anmerkung
Ich habe mir auch das Repo "plantuml-stdlib" angesehen. Darin sind alle Standard-Bibliotheken von Plantuml enthalten. Leider hat das nicht weiter geholfen. Viele haben noch !Define verwendet und die meisten brauchen keine Verschachtelung in ihren Diagrammen.