---
content-type: overview
title: Overzicht van samenvattingen
description: U kunt het deelvenster Samenvatting gebruiken om de gegevens van het werkitem rechtstreeks vanuit een lijst met taakproblemen, documenten of andere gebieden van [!DNL Adobe Workfront] die taken en problemen weergeven.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# [!UICONTROL Summary] overzicht

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

U kunt de [!UICONTROL Summary] om de gegevens van het werkitem rechtstreeks vanuit een lijst met taken, problemen, documenten of andere gebieden van [!DNL Adobe Workfront] die taken en problemen weergeven.

Uw Workfront of groepsbeheerder kan de gebieden en velden wijzigen die worden weergegeven in het deelvenster Samenvatting. Ze kunnen maximaal 16 velden toevoegen aan het deelvenster Samenvatting.

>[!IMPORTANT]
>
>U wordt aangeraden velden toe te voegen die u regelmatig moet bijwerken naar het deelvenster Overzicht, zodat u deze gemakkelijk kunt openen en bijwerken zonder de hoofdpagina van het object te openen.
>
>U kunt bijvoorbeeld de volgende veelbijgewerkte velden toevoegen aan de deelvensters Overzicht van taken en uitgaven:
>
>* Status
>* Percentage voltooid
>* Vastlegdatum
>* Geplande afsluitdatum
>* Voorwaarde



In de volgende tabel worden de gebieden weergegeven waar u de [!UICONTROL Summary] paneel:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>Taken</b></td> 
  </tr> 
  <tr> 
   <td> <p>Taaklijsten binnen een</p> 
    <ul> 
     <li>Project</li> 
     <li>Subtaak</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Taken in de [!UICONTROL Unassigned] en [!UICONTROL Assigned] Werkgebieden van de [!UICONTROL Workload Balancer]</td> 
  </tr> 
   <tr> 
   <td>Taken in een [!UICONTROL Timesheet]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>Problemen</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Uitgiftenlijsten binnen een</p> 
    <ul> 
     <li>Project</li> 
     <li>Taak</li> 
     <li>Subtaak</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemen in de [!UICONTROL Assigned Work] gebied van de [!UICONTROL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemen in de [!UICONTROL Submitted] van de [!UICONTROL Requests] gebied</td> 
  </tr> 
</tr> 
   <tr> 
   <td>Problemen in een [!UICONTROL Timesheet]</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Documenten</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Documents] gebied</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Documents] sectie van om het even welk voorwerp (project, taak, kwestie, programma, portefeuille, malplaatje, malplaatjetaak, gebruiker)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

In dit artikel wordt beschreven hoe u het dialoogvenster [!UICONTROL Summary] voor taken en problemen in lijsten.

Voor informatie over de toegang tot van [!UICONTROL Summary] in de [!UICONTROL Workload Balancer], zie [Werk-items bij in het dialoogvenster [!UICONTROL Workload Balancer] met de [!UICONTROL Summary]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Voor informatie over de toegang tot van [!UICONTROL Summary] voor documenten, zie [[!UICONTROL Summary] voor documentoverzicht](../../documents/managing-documents/summary-for-documents.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>Nieuw: Medewerker of hoger</p>
   of
   <p>Huidige:[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuratie op toegangsniveau</strong></td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Taken, Kwesties, Documenten</p> <p>[!UICONTROL View] of betere toegang tot objecten waarvoor u documenten wilt bekijken [!UICONTROL Summary]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL View] of hogere machtigingen voor een taak, uitgave of document</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw [!DNL Workfront] beheerder. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## De weergave [!UICONTROL Summary] in een lijst met taken of problemen

1. Ga naar een taak of kwestie en selecteer een punt in de lijst.
1. Klik op de knop **[!UICONTROL Summary]** pictogram ![](assets/qs-summary-in-new-toolbar-small.png)

   of

   Klik op de knop **[!UICONTROL Open Summary]** pictogram ![](assets/open-summary-with-text-nwe.png) in de [!UICONTROL Submitted] van de [!UICONTROL Requests] gebied.

   Nadat u het Overzicht opent, blijft het open aangezien u klikt of andere taken of kwesties selecteert en blijft open tot u het manueel sluit.

   >[!TIP]
   >
   >U kunt slechts één taak of één uitgave tegelijk selecteren om hun details in te zien in de [!UICONTROL Summary] deelvenster.

   ![Het deelvenster Samenvatting](assets/summary-panel-for-task-new-comments.png)

1. (Optioneel) Als u het dialoogvenster [!UICONTROL Summary] voert u een van de volgende handelingen uit:

   * Klik in een taak- of uitgavelijst op de knop **[!UICONTROL Open Summary]** pictogram ![](assets/summary-panel-icon.png)

     of

     Klik op de knop **X** in de rechterbovenhoek van het dialoogvenster [!UICONTROL Summary] deelvenster.

   * In de [!UICONTROL Submitted] van de [!UICONTROL Requests] gebied, klik **[!UICONTROL Close Summary]** pictogram ![](assets/close-summary-with-text-nwe.png)

     of

     Klik op de knop **X** in de rechterbovenhoek van het deelvenster Samenvatting.

## [!UICONTROL Percent Complete]

Gebruik de voortgangsbalk boven aan het dialoogvenster [!UICONTROL Summary] om het percentage bij te werken volledig voor de taak of kwestie die u hebt geselecteerd. Voer een getal in of sleep de balk naar het juiste percentage.

![Percentage voltooid in deelvenster Samenvatting](assets/summary-overview-percent-complete.png)

## [!UICONTROL Updates]

Gebruik de [!UICONTROL Updates] van de [!UICONTROL Summary] om recente updates weer te geven en updates uit te voeren over de taak of uitgave die u hebt geselecteerd. Klikken **[!UICONTROL See all]** om rechtstreeks naar de [!UICONTROL Updates] op de taak.

![Sectie Updates in het deelvenster Overzicht](assets/summary-updates-section.png)

## [!UICONTROL Documents]

Gebruik de [!UICONTROL Documents] van de [!UICONTROL Summary] als u documenten wilt bekijken die zijn gekoppeld aan de geselecteerde taak of uitgave. Klik op de miniatuur om een documentvoorbeeld te openen. Ga rechtstreeks naar de [!UICONTROL Documents] op de taak of uitgave klikt u op **[!UICONTROL Documents]** titel.

![Sectie Documenten in deelvenster Samenvatting](assets/summary-documents-section.png)

## [!UICONTROL Details]

Gebruik de [!UICONTROL Details] van de [!UICONTROL Summary] als u de details van het werkitem op hoog niveau wilt weergeven, toewijzingen wilt maken of begindatums wilt toevoegen. Klikken **[!UICONTROL See all]** om rechtstreeks naar de [!UICONTROL Details] op de taak of uitgave.

>[!NOTE]
>
>De velden in deze sectie zijn dezelfde velden die in het rechterdeelvenster van Home worden weergegeven. U kunt deze velden aanpassen [Aanpassen [!UICONTROL Home] en [!UICONTROL Summary] een lay-outsjabloon gebruiken](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![Sectie Details in het deelvenster Samenvatting](assets/summary-details-section.png)

## [!UICONTROL Subtasks]

Deze sectie is alleen beschikbaar voor taken. Gebruik de [!UICONTROL Subtasks] van de [!UICONTROL Summary] aan mening [!UICONTROL New], [!UICONTROL In Progress], en [!UICONTROL Closed] subtaken voor de taak u selecteerde. Klik op de knop **[!UICONTROL Status]** vervolgkeuzemenu voor het schakelen tussen statussen. Ga rechtstreeks naar de [!UICONTROL Subtasks] klikt u op de knop **[!UICONTROL Subtasks]**&#x200B; titel.

Als u geen subtaken aan de taak hebt toegevoegd, klikt u op **[!UICONTROL Add one here]** om rechtstreeks naar de [!UICONTROL Subtasks] op de taak.

![Sectie Subtaken in het deelvenster Samenvatting](assets/summary-subtasks-section.png)

## [!UICONTROL Hours]

Gebruik de [!UICONTROL Hours] van de [!UICONTROL Summary] om uren te registreren op de taak of kwestie u selecteerde. Klikken **[!UICONTROL Log Time]** en voer uw uren in. Als u rechtstreeks naar het tabblad Uren van de taak of uitgave wilt gaan, klikt u op de knop **[!UICONTROL Hours]** titel.

Het aantal uren in de [!UICONTROL Summary] geeft de uren weer die u zich aanmeldt. Andere gebruikers hebben verschillende totalen per uur in het dialoogvenster [!UICONTROL Summary] afhankelijk van de tijd die zij aan de taak registreren.

Als er geen plannen zijn [!UICONTROL hours] op de taak of de kwestie en u hebt het programma geopend, toont de urenbar rood.

![Sectie Uren in deelvenster Samenvatting](assets/summary-hours-section.png)

## Goedkeuringen

Gebruik de [!UICONTROL Approvals] van de [!UICONTROL Summary] om goedkeuringen weer te geven die zijn gekoppeld aan de geselecteerde taak of uitgave. Als u geen goedkeuring hebt toegevoegd, selecteert u een bestaande goedkeuring in het keuzemenu of klikt u op **[!UICONTROL Create single-use approval process]** om rechtstreeks naar de [!UICONTROL Approvals] op de taak of uitgave.

Ga rechtstreeks naar de [!UICONTROL Approvals] op de taak of uitgave klikt u op **[!UICONTROL Approvals]** titel.

![Sectie Goedkeuring in deelvenster Samenvatting](assets/summary-approvals-section.png)
