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
skinparam ranksep 140
skinparam ArrowColor #828282
skinparam ArrowFontColor #404040
skinparam ArrowFontSize 11
skinparam componentFontSize 13
skinparam actorBackgroundColor #FFBB33
skinparam actorBorderColor #FFBB33

actor "Patient" as PT

component "Browser" as BR #FFBB33
component "PHR" as PHR #FFBB33
component "<color:#FFFFFF>XIS" as XIS #0050EF
component "Provider Module" as PM #B3B3B3
component "End User xIS" as EU #B3B3B3

PT -> BR : **Views health data in Browser**\n[human interaction]
BR -right-> PHR : **Requests pages from PHR**\n[HTTPS/HTML 5.0]
PHR -> XIS : **API calls**\n[HTTPS/JSON &\nOAuth 2.0]
BR -> PM : **Opens Task page Provider Module**\n**and enters results**\n[HTTPS/HTML 5.0]
XIS -down-> PM : **Authorisation, Launch context, Data Service**\n[S.D. Provider Module, SMART on FHIR,\nOAuth 2.0, OIDC, GET [base]/Task]
XIS -right-> EU : **Collects data**\n[outside MedMij\nstandard]
PM -> EU : **Possible data exchange**\n[outside MedMij standard]
@enduml

</plantuml>
