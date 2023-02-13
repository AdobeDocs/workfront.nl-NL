---
product-area: projects
navigation-topic: convert-issues
title: Een uitgave converteren naar een taak in Adobe Workfront
description: Als er meer moet worden gedaan om een probleem op te lossen nadat het probleem is verzonden, kunt u het probleem omzetten in een taak.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Een uitgave converteren naar een taak in Adobe Workfront

Als er meer moet worden gedaan om een probleem op te lossen nadat het probleem is verzonden, kunt u het probleem omzetten in een taak.

Voor algemene informatie over het converteren van problemen raadpleegt u [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen, taken en projecten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor de uitgave</p> <p>Contribute-machtigingen voor het project</p> <p>U krijgt beheermachtigingen voor de taak nadat de uitgave is omgezet</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Een uitgave converteren naar een taak

1. Ga naar een project en klik op [!UICONTROL **Problemen** ] in het linkerdeelvenster.
1. Klik op de uitgave die u wilt converteren om naar de openingspagina van de uitgave te gaan.
1. Klik op de knop [!UICONTROL **Meer**] menu over de kwestie, dan [!UICONTROL **Omzetten in taak**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Als het probleem is gekoppeld aan een goedkeuringsproces of al is gekoppeld aan een oplossend object, geeft Workfront boven aan het dialoogvenster een waarschuwing weer [!UICONTROL Convert to Project] om aan te geven dat de goedkeuring is verwijderd of dat het oplossende object tijdens de conversie is overschreven. Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Werk de taaknaam bij in het dialoogvenster [!UICONTROL Task Name] sectie. Standaard krijgt de taak dezelfde naam als de oorspronkelijke uitgave.

   ![](assets/convert-to-task-box-nwe.png)

1. Klikken [!UICONTROL **Doelproject**], dan begin de naam van het project te typen waar u de nieuwe taak in wilt plaatsen [!UICONTROL **Doelproject**] en selecteert u deze wanneer deze in de lijst wordt weergegeven. Het project van de kwestie wordt geselecteerd door gebrek.

1. Klikken [!UICONTROL **Overzicht**] Typ vervolgens een [!UICONTROL **Beschrijving**] voor de taak.

   >[!TIP]
   >
   >   Een systeem- of groepsbeheerder kan de volgorde van de secties in het linkerdeelvenster van het conversievak wijzigen door de lay-outsjabloon te wijzigen.

1. (Optioneel en voorwaardelijk) Klik op [!UICONTROL **Opties**] selecteert u een van de onderstaande opties.

   De Workfront-beheerder of groepsbeheerder moet deze voorkeuren inschakelen voordat deze zichtbaar zijn tijdens de conversie van uitgaven:

   * [!UICONTROL **Behoud het oorspronkelijke probleem en koppel zijn resolutie aan deze taak**]

      Als deze optie niet is geselecteerd, wordt de oorspronkelijke uitgave verwijderd.

      >[!NOTE]
      >
      >Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:
      >   
      >   * [Toegang verlenen tot kwesties](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
      >   * [Een uitgave delen](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


   * [!UICONTROL **(Gebruikersnaam) toegang tot deze taak geven**]

      Als deze optie niet is geselecteerd, heeft de primaire contactpersoon van de uitgave geen toegang tot de nieuwe taak.

   * [!UICONTROL **Behoud de geplande einddatum van de uitgifte**]

      Als deze optie niet is geselecteerd, wordt [!UICONTROL Planned Completion Date] van de nieuwe taak wordt berekend op basis van [!UICONTROL Planned Start Date] van de taak. De [!UICONTROL Planned Start Date] van de nieuwe taak wordt ingesteld volgens de systeemvoorkeuren voor nieuwe taken .

      >[!NOTE]
      >
      >
      >Welke opties hier worden weergegeven, is afhankelijk van de configuratie die de Workfront-beheerder heeft opgegeven voor iedereen in het systeem. Zie voor meer informatie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
      >
      >Of, als de top-level groepen in uw organisatie hen afzonderlijk vormden, hangen de opties die hier tonen af van welke groep met het project wordt geassocieerd u in stap 6 selecteerde. Zie voor meer informatie [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Optioneel) Klik op [!UICONTROL **Aangepaste Forms**] en voeg een aangepast formulier toe voor de nieuwe taak.

   >[!TIP]
   >
   >Als een aangepast formulier voor meerdere objecten dat aan de uitgave is gekoppeld, is geconfigureerd voor gebruik met zowel uitgaven als taken, wordt het formulier standaard bijgevoegd. Alle informatie die in het uitgifteformulier is opgeslagen, blijft voor de taak behouden wanneer u de conversie uitvoert.
   >
   >Als voor het doelproject standaardformulieren zijn gedefinieerd in het veld Standaard aangepaste Forms voor taak bij het bewerken van het project, worden deze taakformulieren ook toegevoegd aan de nieuwe taak. Aangepaste velden die veel voorkomen tussen de oorspronkelijke uitgave en de velden op de standaardtaakformulieren, worden vooraf ingevuld met informatie uit de uitgiftevelden.

1. Klikken [!UICONTROL **Omzetten in taak**].

   De kwestie is nu een taak op het aangewezen project, als u besloot om de originele kwestie te schrappen.

   of

   Het probleem is nu gekoppeld aan de nieuwe taak voor het project dat u hebt gekozen en wordt voltooid zodra de taak is voltooid, als u de oorspronkelijke uitgave wilt behouden.

   Sommige probleemvelden worden overgebracht naar de taak. Zie voor meer informatie de [Originele informatie over projecten en taken weergeven](#view-original-issue-information-on-projects-and-tasks) in dit artikel.

1. (Optioneel) Ga desgewenst verder met het bewerken van de taak.

## Originele informatie over projecten en taken weergeven {#view-original-issue-information-on-projects-and-tasks}

U kunt de originele uitgifteinformatie in project en taaklijsten en rapporten of in het gebied van de Details van het Project bekijken. Voor informatie over bouwrapporten, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

In de volgende tabel wordt aangegeven welke velden zichtbaar zijn van de omgezette projecten en taken.

| Probleemvelden | Project- of taakveld | Projectlijst of -rapport | Het gebied Projectdetails | Taaklijst of rapport | Taakdetails, gebied |
|---|---|---|---|---|---|
| [!UICONTROL Issue Name] | [!UICONTROL Converted Issue Name] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Primary Contact] | [!UICONTROL Converted Issue Originator Name] | ✔ | ✔ | ✔ |
| [!UICONTROL Entry Date] | [!UICONTROL Converted Issue Entry Date] | ✔ |  | ✔ |


>[!CAUTION]
>
>Als de [!UICONTROL Primary Contact] van een emissie verandert of als de uitgave loskomt van het project of de taak nadat de uitgave is omgezet, [!UICONTROL Converted Issue Originator Name ]wordt niet bijgewerkt en het origineel wordt weergegeven [!UICONTROL Primary Contact] van de emissie op het tijdstip van omzetting van de emissie.
