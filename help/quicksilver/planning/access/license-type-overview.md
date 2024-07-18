---
title: Overzicht van licentietype bij gebruik van Adobe Workfront Planning
description: De toegang tot Adobe Workfront Planning is afhankelijk van het type licentie en van de machtigingen tot objecten.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Overzicht van licentietype bij gebruik van Adobe Workfront Planning

{{planning-important-intro}}

Het Adobe Workfront-licentietype werkt in combinatie met uw Adobe Workfront-planningsbevoegdheden en geeft de volgende toegang:

* Werkruimten weergeven, bijdragen of beheren
* Weergaven weergeven of beheren.

Voor informatie over toestemmingen aan voorwerpen in de Planning van Workfront, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## De relatie tussen Workfront-licentietypen en Workfront-planningsmachtigingen

In de onderstaande tabel wordt de relatie beschreven tussen het licentietype van een gebruiker in Adobe Workfront en het machtigingsniveau dat u aan deze gebruiker kunt toekennen aan Adobe Workfront-planningsobjecten op basis van die licentie.

Het verlenen van gebruikerstoestemmingen aan een werkruimte verleent hen ook toestemmingen om types, verslagen, en gebieden te registreren.


| Adobe Workfront-licentietype* | Hoogste machtigingen toegestaan in Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nieuw: Standaard <br> of <br> Huidig: Plan | Gebruikers kunnen werkruimten beheren. Ze kunnen werkruimten, recordtypen, records en velden maken, bewerken of verwijderen. <br> Systeembeheerders hebben beheermachtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt. |
| Nieuw: Licht, Medewerker <br> of <br> Huidig: Werk, Aanvrager, Reviewer | De gebruikers kunnen de werkruimten bekijken die met hen, evenals de verslagtypes, verslagen, en gebieden van die werkruimten worden gedeeld. <br> Gebruikers kunnen geen werkruimten, recordtypen, records of velden maken, bewerken of verwijderen. |

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

### Licentietypen en werkruimtemachtigingen

Alleen gebruikers met een Standard- (of Plan-) licentie kunnen over Contribute- of Manage-machtigingen voor werkruimten beschikken. Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor werkruimten die met hen worden gedeeld.

Systeembeheerders kunnen alle werkruimten in het systeem weergeven, zelfs de werkruimten die ze niet hebben gemaakt.

>[!INFO]
>
>**VOORBEELD:**
>
>Aanvragers (of medewerkers volgens het nieuwe licentiemodel) kunnen geen bijdrage leveren aan werkruimten en hun objecten of deze beheren.
>
>Er is een aanwijzing in het deelvak dat gebruikers geen machtigingen kunnen worden verleend om bij te dragen aan een werkruimte of een werkruimte te beheren wanneer zij een licentie op een lager niveau hebben, omdat deze machtigingsniveaus grijs worden weergegeven.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)

### Licentietypen en weergavemachtigingen

Alleen gebruikers met een Standard- (of Plan-) licentie kunnen beheermachtigingen voor weergaven hebben. Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor weergaven die met hen worden gedeeld.

>[!INFO]
>
>**VOORBEELD:**
>
>Medewerkers (of aanvragers en revisoren) kunnen geen weergaven beheren. Ze kunnen tijdelijke filters, sorteren of groeperingen toepassen op weergaven waartoe ze toegang hebben.
>
>Er is een aanwijzing in het deelvak dat gebruikers geen machtigingen kunnen worden verleend om een weergave te beheren wanneer zij een licentie op een lager niveau hebben, omdat deze machtigingsniveaus grijs worden weergegeven.
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->