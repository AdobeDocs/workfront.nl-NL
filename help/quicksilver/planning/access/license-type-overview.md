---
title: Overzicht van licentietype bij gebruik van Adobe Workfront-planning
description: De toegang tot Adobe Workfront Planning is afhankelijk van het type licentie en van de machtigingen tot objecten. Niet alle gebruikers in de organisatie hebben de zelfde toegang en de toestemmingen om de Planning van Adobe Workfront te gebruiken. In dit artikel worden de toegangsniveaus beschreven die gebruikers kunnen hebben voor Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---


# Overzicht van licentietype bij gebruik van Adobe Workfront Planning

{{planning-important-intro}}

Het Adobe Workfront-licentietype werkt in combinatie met uw Adobe Workfront-planningsbevoegdheden en geeft de volgende toegang:

* Werkruimten weergeven, bijdragen of beheren
* Weergaven weergeven of beheren.

Voor informatie over toestemmingen aan voorwerpen in de Planning van Workfront, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Voor informatie over toegang tot de Planning van Workfront, zie [ de toegangsoverzicht van de Planning van de Adobe ](/help/quicksilver/planning/access/access-overview.md).

## De relatie tussen Workfront-licentietypen en Workfront-planningsmachtigingen

In de onderstaande tabel wordt de relatie beschreven tussen het licentietype van een gebruiker in Adobe Workfront en het machtigingsniveau dat u aan deze gebruiker kunt toekennen aan Adobe Workfront-planningsobjecten op basis van die licentie.

Het verlenen van gebruikerstoestemmingen aan een werkruimte verleent hen ook toestemmingen om types, verslagen, en gebieden te registreren.

U moet gebruikers afzonderlijke toestemmingen aan meningen, naast degenen verlenen zij voor werkruimten hebben, om tot meningen toegang te hebben en te leiden.

| Adobe Workfront-licentietype* | Hoogste machtigingen toegestaan in Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standaard | <p>Gebruikers kunnen werkruimten en weergaven beheren. Ze kunnen werkruimten, recordtypen, records, velden en weergaven maken, bewerken of verwijderen.</p> <br> <p>Systeembeheerders hebben beheermachtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p> |
| Licht of medewerker | <p>De gebruikers kunnen de werkruimten bekijken die met hen, evenals de verslagtypes, verslagen, en gebieden van die werkruimten worden gedeeld.</p> <br> <p>Gebruikers kunnen de weergaven bekijken die met hen worden gedeeld, maar ze kunnen hun eigen weergaven niet maken. </p><br> <p>Gebruikers kunnen geen werkruimten, recordtypen, records of velden maken, bewerken of verwijderen.</p> |

*Workfront Planning is niet beschikbaar voor verouderde Workfront-licenties.
Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Licentietypen en werkruimtemachtigingen

Alleen gebruikers met een standaardlicentie kunnen over Contribute- of beheermachtigingen voor werkruimten beschikken. Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor werkruimten die met hen worden gedeeld.

Systeembeheerders kunnen alle werkruimten in het systeem weergeven, zelfs de werkruimten die ze niet hebben gemaakt.

>[!INFO]
>
>**VOORBEELD:**
>
>Medewerkers of gebruikers met een lichtlicentie kunnen geen bijdrage leveren aan werkruimten en hun objecten of deze beheren.
>
>Er is een aanwijzing in het deelvak dat gebruikers geen machtigingen kunnen worden verleend om bij te dragen aan een werkruimte of een werkruimte te beheren wanneer zij een licentie op een lager niveau hebben, omdat deze machtigingsniveaus grijs worden weergegeven.
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Licentietypen en weergavemachtigingen

Alleen gebruikers met een standaardlicentie kunnen beheermachtigingen voor weergaven hebben. Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor weergaven die met hen worden gedeeld.

>[!INFO]
>
>**VOORBEELD:**
>
>Medewerkers of gebruikers met een lichtlicentie kunnen geen weergaven beheren. Ze kunnen tijdelijke filters, sorteren of groeperingen toepassen op weergaven waartoe ze toegang hebben.
>
>Er is een aanwijzing in het deelvak dat gebruikers geen machtigingen kunnen worden verleend om een weergave te beheren wanneer zij een licentie op een lager niveau hebben, omdat deze machtigingsniveaus grijs worden weergegeven.
>
>![](assets/permissions-grayed-out-for-light-user.png)
