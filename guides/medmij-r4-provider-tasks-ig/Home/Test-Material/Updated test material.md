# Updated test material

Changes to the test material for Alpha.1

# Scenario 1

## Task data

### Information tasks

Two information tasks. The patient is not required to launch the module on a specific date; the entire execution period (22-12-2025 t/m 28-12-2025) is available.

| Identifier | ActivityDefinition | Description | Status | LastModified |
| --- | --- | --- | --- | --- |
| TASK-Informatie-diabetes-12345 | Wat is diabetes type 2? | Lees wat diabetes type 2 is en wat je zelf kunt doen | received | 23-12-2025 07:00 |
| TASK-Informatie-Gezonderleven-6789 | Gezonder gaan leven | Lees tips voor een gezonder leven: voeding, bewegen en volhouden | requested | 24-12-2025 07:00 |
| TASK-Informatie-Gezonderleven-6789 | Gezonder gaan leven | Lees tips voor een gezonder leven: voeding, bewegen en volhouden [1] | requested | 24-12-2025 07:00 |

### Measurement tasks (Bloedglucosemeting)

Fourteen blood-glucose measurement tasks, 2 per day during 7 consecutive days (22-12-2025 t/m 29-12-2025). All 16 tasks share the following properties:

| | |
| --- | --- |
| ActivityDefinition | Bloedglucose meting volgens NHG protocol |
| BasedOn (digital group plan) | Digitale zorgmodule Diabetes |
| Focus (execution order) | Uitvoeringsopdracht Bloedglucosemeting |
| AuthoredOn / LastModified | 22-12-2025 08:00 |

The execution date, status and description per task are:

| Identifier | ExecutionPeriod | Status | Description |
| --- | --- | --- | --- |
| TASK-Glucose-1 | 22-12-2025 (1st measurement) | completed | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [completed] |
| TASK-Glucose-2 | 22-12-2025 (2nd measurement) | completed | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel.[completed] |
| TASK-Glucose-3 | 23-12-2025 (1st measurement) | completed | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [completed] |
| TASK-Glucose-4 | 23-12-2025 (2nd measurement) | cancelled | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [cancelled] |
| TASK-Glucose-5 | 24-12-2025 (1st measurement) | failed | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [failed] |
| TASK-Glucose-6 | 24-12-2025 (2nd measurement) | rejected | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [rejected] |
| TASK-Glucose-7 | 25-12-2025 (1st measurement) | requested | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [requested] |
| TASK-Glucose-8 | 25-12-2025 (2nd measurement) | received | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [received] |
| TASK-Glucose-9 | 26-12-2025 (1st measurement) | ready | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [ready] |
| TASK-Glucose-10 | 26-12-2025 (2nd measurement) | in-progress| Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [in-progress] | 
| TASK-Glucose-11 | 27-12-2025 (1st measurement) | in-progress | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [in-progress] |
| TASK-Glucose-12 | 27-12-2025 (2nd measurement) | in-progress | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [in-progress] |
| TASK-Glucose-13 | 28-12-2025 (1st measurement) | accepted | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [accepted] |
| TASK-Glucose-14 | 28-12-2025 (2nd measurement) | on-hold | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [on-hold] |
| TASK-Glucose-15 | 29-12-2025 (1st measurement) | draft | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [draft] |
| TASK-Glucose-16 | 29-12-2025 (2nd measurement) | entered-in-error | Deze meting helpt om inzicht te krijgen in de bloedsuikerspiegel. [entered-in-error] |

# Scenario 4

## Patient data Lucy Di Bartini

| | |
| --- | --- |
| Name.GivenName (official) | Lucy (qualifier 'BR' – call name) |
| Name.GivenName (usual / call name) | Lucy |
| Name.FamilyName.Prefix | Di |
| Name.FamilyName.LastName | Bartini |
| Gender | Female (code 'F' from code system 'http://terminology.hl7.org/CodeSystem/v3-AdministrativeGender') |
| BirthDate | 01-07-1999 |
| Deceased | No |
| Nationality | Nederlandse (code '0001' from code system 'urn:oid:2.16.840.1.113883.2.4.4.16.32') |
| Address.AddressType | Primary home (code 'HP' from code system 'http://terminology.hl7.org/CodeSystem/v3-AddressUse') |
| Address.Street | Parkweg |
| Address.HouseNumber | 1130 |
| Address.PostalCode | 2271 AK |
| Address.City | Voorburg |
| Address.Country | Nederland (code 'NL' from code system 'urn:iso:std:iso:3166') |
| ContactInformation.TelephoneNumber | +31655501234 (mobile contact, code 'MC' from code system 'http://terminology.hl7.org/CodeSystem/v3-AddressUse') |
| ContactInformation.EmailAddress | Lucy.dibartini@voorbeeldmail.nl (home) |
| PatientIdentificationNumber (BSN) | masked (in identifier system 'http://fhir.nl/fhir/NamingSystem/bsn') |