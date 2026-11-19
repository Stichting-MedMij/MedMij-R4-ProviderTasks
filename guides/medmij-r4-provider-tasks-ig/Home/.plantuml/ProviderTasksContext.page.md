---
topic: ProviderTasksContext
---

<plantuml>

@startuml
scale max 900 width
skinparam shadowing false
skinparam defaultFontName Segoe UI
skinparam linetype ortho
skinparam nodesep 200
skinparam ranksep 180
skinparam ArrowColor #828282
skinparam ArrowFontColor #404040
skinparam ArrowFontSize 11
skinparam componentFontSize 15
skinparam actorBackgroundColor #FFBB33
skinparam actorBorderColor #FFBB33

actor "Patiënt" as PT

component "Browser" as BR #FFBB33
component "PGO" as PGO #FFBB33
component "<color:#FFFFFF>XIS" as XIS #0050EF
component "Modulesysteem" as MOD #B3B3B3
component "xIS eindgebruiker" as EU #B3B3B3

PT -down-> BR : **Raadpleegt gezondheidsgegevens**\n**in de browser**\n[menselijke interactie]
BR -right-> PGO : **Vraagt pagina's op bij de PGO**\n[HTTPS/HTML 5.0]
PGO -right-> XIS : **API-aanroepen**\n[HTTPS/JSON &\nOAuth 2.0]
BR -right-> MOD : **Opent de taakpagina van het**\n**modulesysteem en voert resultaten in**\n[HTTPS/HTML 5.0]
XIS -down-> MOD : **Autorisatie, launchcontext, gegevensdienst**\n[S.D. Aanbiedermodules, SMART on FHIR,\nOAuth 2.0, OIDC, GET [base]/Task]
XIS -right-> EU : **Verzamelt gegevens**\n[buiten de MedMij-standaard]
MOD -right-> EU : **Mogelijke gegevensuitwisseling**\n[buiten de MedMij-standaard]
@enduml

</plantuml>
