## Demo für Define und Procedure
### Methode 1 !Define
Code für diese Diagram, finden Sie in "customized-elements/system-context.plantuml und withDefine.plantuml".

![test](https://www.plantuml.com/plantuml/png/lPPTRvim58Rl_IlEwAIKY4HgBgS6DThINKsh-d4TkN0WgCP6jgEGTVtlEoQ40cscRT7mHKJiSzxtiGq-lZAMQxl91LWqbZ7pbCc2Qvw3niXocGg4PmRKhfMqTtP7_wNIEHViXR7HKc2EqYBx46EIIOIxdR6Od-EAYuoR070b-2CAloNdZSTrxtZimUNbFYKCWHkey-0iIP9P53MoozAYbboi_a7_a0j_OhIFMTr5gi23Iqzy7m9LY7DegS6P895fpCqQuqRpiyeB9McP_WgxoUe2DyHiT8k2sqn9iyuAqxXHx-h1E7YZDZh2nS6HDZf5k-W0k8SuSn2aC_Sy7pffxT6k0dmYn8t1CFHgAQz3y8LRdWYr7G8ZhhsEiTnMZqEGwChf6CVt0ZMtWu2elTKnacM9qMOO4jnR7NrFi11gDyXRKZaTtPkj76HVjl8OmJSkiuJEu24myjghpTA1-VyGxo_2LvJquehiHtMm4SMrLhcpkLUDQsLKGxup780t-HbwVky8E5bqEdsZMXtH9Zj5TJoPz4GNQQenFGbLLQ9i52iqqi9MwISsWjf4A9d2KjhCxjxK8_T0nKrZ9LTULBypdv9RTMe-FsoT-xph-4wHUgO4rx0yRwdqQrqv-srzBY-QKZU25yUFCdwT0atl8_Pk1VVRp58FJRr_N-01tF3T3HS-gtiU0sZ2EqK_yjbhmOu3gjxIQYL4fNiehgGNqKAlKGZb1J2TXZxhVCGKG0uUBRs8sm4kcJ99rtCNBXgQJ6Z8jIkQ7rt4VW40 "test")

### Problemstellung für Define-Art
1. Im PlantUML Language Reference Guide, Kapitel 25.23 Migration notes, wird beschrieben, dass !Define nicht mehr verwendet werden sollte. Auch wenn es funktioniert.
2. Es funktionierte nicht, wenn mehrere Elemente verschachtelt wurden. Auch in Archimate-Repo wurde die Verschachtelung von Elementen nicht verwendet.

### Methode 2 !Procedure
Code für diese Diagram, finden Sie in "customized-elements/withProcedure.plantuml".

![test Procedure](https://www.plantuml.com/plantuml/png/ZLPjRzis4FwkNt7MD4YANQpDno4skhekDc3D2iIVsXa6BL4s4OhqI6f9DlIVzTl-M8-aPBqvpW845e_7vvvxU4VohJP4cQhaOAWsy4d9ZEQLea4mgSHVbJGqXsDZX7Uo4ZbHJqb4E2Dw1X4dEyhnrpmTwJmCxHVPQ__5cRZ7hpIOHBjwuHedOGuHoVC6wvFKfc2FYLkO1Z48cLFj4K7HIhi1pGu2SbemmGoJ0cG1FL2CuIX4HguuBQamlwXzucoplkSCmje3HskBYrp3niEoPGKaZZnCvc3v0qmYv97VqeVVcQ2OGBpP_2dcS_Zo9OQfpnH_OuYThnDbRVcZvpalEzefIkxNzD4a9n4xCLBhkDd4mOHoJSynSF77yLx2HK2HioBmQJgHJrcEiDh1r0QyqUmV-hDZlrujVxtTVlZZThsz--tpoiulV9QcTj_S_6JT5t4JSISV8MmXGtILTuOgAdNIwZ_OBS_ts2dBSJLkLo9FqW3z06EC5fofuwKKXg0QQdkXeiTrZFgush1JVTK8vqrfkqdCVverGTmcrTlOTuu7FaudmFhmAhfwH-9_C-9mGPidRb6UPUturlWryw62hHv59JBNJ1VQiKxvHsqKfwAs0bRUwpfrHKsb1CIz14ODxwUnDX4UXnRkYDlku93rr8lxS62SehxURT46SSdRPTKELpRBNjjQiQwDr_2KwOsdNaBScMrZdyOjl1xZU_3fcnFyPVQOl4lW6SqMRJR_WwVk4UsBMqi-EFzmkjdGNfT4fSQ3KCjAPVOenBFLC46icwLJJy2hLulUt8MsY_1ieKeGlhrxqeQMRH5gD_PDaydoA0MUidNdw7icZaIH4lvrAW2UxPaXOeyxtbZitmViY3jRvdWFg9BmpjGxajtlbKrwARbKy4DH5DTPLdjy3Vo_Rr5FfT-aQ6iKzzE3lcpdOvzPH_OJy2clFhOrhrsHdXm6wAr7l6nSUllQwd5rvIMzkeARcrMjDdXEYqMZbktQZrBH-ZPB6lvfP_uKAMdYfqwc2xixH7LCqkVvTMcz1DoXynBioVKPv61KXWVAkPp1mu6OQqhCpBreqi3LVzXOxLrlxRXnGH2_9neOFdkA_xufM7AYDRndP8zLYk-GBdVxxDXcrY6912cfVQS0E0Cu0zPmt5MzbE8ZDGTfBwROLMSCWmpw4SulipUaOc9V3mz47vRuF7B34LoNPLX8-IPCprYllTMfufnGaTeSl4L8V0j-1m00 "test Procedure")

### Problemstellung für Procedure-Art
1. Alternativ zu !Define kann !Procedure verwendet werden. Wie in der Abbildung gezeigt, ist eine Verschachtelung möglich. Es ist machbar, aber sehr zeitaufwendig.s
2. Es gibt noch ein weiteres Problem. Wenn man sich diesen Code ```!procedure $external_System($alias, $system="", $component="")``` (withProcedure.plantuml) anschaut, braucht man für diese "Funktion" $external_System noch 3 weitere "Parameter". Das bedeutet, dass man in diesem Block nur ein System + eine Component hinzufügen kann. Wenn man mehr Komponenten braucht, muss man den Code erweitern, was natürlich nicht so flexibel und dynamisch ist.
3. Wenn man es trotzdem flexibel und dynamisch machen will, muss man es wie C4-Repo machen. In diesem Repo sind aber sehr viele Codes und die Codes sind nicht überschaubar, oft sind sie miteinander verschachtelt.

### Anmerkung
Ich habe mir auch das Repo "plantuml-stdlib" angesehen. Darin sind alle Standard-Bibliotheken von Plantuml enthalten. Leider hat das nicht geholfen. Define und die meisten brauchen keine Verschachtelung in ihren Diagrammen.