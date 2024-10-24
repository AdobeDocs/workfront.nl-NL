---
content-type: overview
title: Overzicht van samenvattingen
description: U kunt het Summiere paneel gebruiken om de informatie van het het werkpunt van een lijst van taakkwesties, documenten, of van andere gebieden van  [!DNL Adobe Workfront]  te herzien en bij te werken die taken en kwesties tonen.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# [!UICONTROL Summary] overzicht

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

U kunt het deelvenster [!UICONTROL Summary] gebruiken om de gegevens van het werkitem rechtstreeks vanuit een lijst met taken, problemen, documenten of andere gebieden van [!DNL Adobe Workfront] die taken en problemen weergeven, te bekijken en bij te werken.

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



In de volgende tabel worden de gebieden weergegeven waar u het deelvenster [!UICONTROL Summary] kunt vinden en gebruiken:

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
   <td>Taken in de werkgebieden [!UICONTROL Unassigned] en [!UICONTROL Assigned] van het dialoogvenster [!UICONTROL Workload Balancer]</td> 
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
   <td>Problemen in het gebied [!UICONTROL Assigned Work] van het dialoogvenster [!UICONTROL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemen in de [!UICONTROL Submitted] -sectie van het [!UICONTROL Requests] -gebied</td> 
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

In dit artikel wordt beschreven hoe u het deelvenster [!UICONTROL Summary] kunt openen en gebruiken voor taken en problemen in lijsten.

Voor informatie over de toegang tot van [!UICONTROL Summary] in [!UICONTROL Workload Balancer], zie [ werk punten in [!UICONTROL Workload Balancer] bijwerken gebruikend [!UICONTROL Summary]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Voor informatie over de toegang tot van [!UICONTROL Summary] voor documenten, zie [[!UICONTROL Summary] voor documentoverzicht ](../../documents/managing-documents/summary-for-documents.md).

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
   <p>Huidig:[!UICONTROL Request] of hoger</p> </td> 
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

*Neem contact op met de [!DNL Workfront] -beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Het deelvenster [!UICONTROL Summary] weergeven in een lijst met taken of problemen

1. Ga naar een taak of kwestie en selecteer een punt in de lijst.
1. Klik op het pictogram **[!UICONTROL Summary]** ![](assets/qs-summary-in-new-toolbar-small.png)

   of

   Klik op het pictogram **[!UICONTROL Open Summary]** ![](assets/open-summary-with-text-nwe.png) in de sectie [!UICONTROL Submitted] van het [!UICONTROL Requests] -gebied.

   Nadat u het Overzicht opent, blijft het open aangezien u klikt of andere taken of kwesties selecteert en blijft open tot u het manueel sluit.

   >[!TIP]
   >
   >U kunt slechts één taak of één uitgave tegelijk selecteren om hun details in het deelvenster [!UICONTROL Summary] weer te geven.

   ![ Samenvattings paneel ](assets/summary-panel-for-task-new-comments.png)

1. (Optioneel) Voer een van de volgende handelingen uit om het deelvenster [!UICONTROL Summary] te sluiten:

   * Klik in een taak- of uitgavelijst op het pictogram **[!UICONTROL Open Summary]** ![](assets/summary-panel-icon.png)

     of

     Klik het **X** pictogram in de hoger-juiste hoek van het [!UICONTROL Summary] paneel.

   * Klik in de sectie [!UICONTROL Submitted] van het [!UICONTROL Requests] -gebied op het pictogram **[!UICONTROL Close Summary]** ![](assets/close-summary-with-text-nwe.png) .

     of

     Klik het **X** pictogram in de hoger-juiste hoek van het Summiere paneel.

## [!UICONTROL Percent Complete]

Gebruik de voortgangsbalk boven aan de [!UICONTROL Summary] om het percentage bij te werken dat is voltooid voor de taak of uitgave die u hebt geselecteerd. Voer een getal in of sleep de balk naar het juiste percentage.

![ Percentage volledig in Samenvattend paneel ](assets/summary-overview-percent-complete.png)

## [!UICONTROL Updates]

In de sectie [!UICONTROL Updates] van [!UICONTROL Summary] kunt u recente updates weergeven en updates uitvoeren op de taak of uitgave die u hebt geselecteerd. Klik op **[!UICONTROL See all]** om rechtstreeks naar het tabblad [!UICONTROL Updates] van de taak te gaan.

![ sectie van Updates in Samenvattend paneel ](assets/summary-updates-section.png)

## [!UICONTROL Documents]

Gebruik de sectie [!UICONTROL Documents] van de [!UICONTROL Summary] om documenten te bekijken die aan de taak zijn gekoppeld of die u hebt geselecteerd. Klik op de miniatuur om een documentvoorbeeld te openen. Als u rechtstreeks naar het tabblad [!UICONTROL Documents] van de taak of uitgave wilt gaan, klikt u op de titel **[!UICONTROL Documents]** .

![ sectie van Documenten in Samenvattend paneel ](assets/summary-documents-section.png)

## [!UICONTROL Details]

In de sectie [!UICONTROL Details] van de [!UICONTROL Summary] kunt u gedetailleerde gegevens van het tijdelijke item weergeven, toewijzingen maken of begindatums toevoegen. Klik op **[!UICONTROL See all]** om rechtstreeks naar het tabblad [!UICONTROL Details] van de taak of uitgave te gaan.



![ sectie van Details in Samenvattend paneel ](assets/summary-details-section.png)

## [!UICONTROL Subtasks]

Deze sectie is alleen beschikbaar voor taken. In de sectie [!UICONTROL Subtasks] van de subtaken [!UICONTROL Summary] kunt u de subtaken [!UICONTROL New] , [!UICONTROL In Progress] en [!UICONTROL Closed] weergeven voor de taak die u hebt geselecteerd. Klik op het vervolgkeuzemenu **[!UICONTROL Status]** om te schakelen tussen statussen. Als u rechtstreeks naar het tabblad [!UICONTROL Subtasks] van de taak wilt gaan, klikt u op de titel **[!UICONTROL Subtasks]** &#x200B;.

Als u geen subtaken aan de taak hebt toegevoegd, klikt u op **[!UICONTROL Add one here]** om rechtstreeks naar het tabblad [!UICONTROL Subtasks] van de taak te gaan.

![ subtasks sectie in Samenvattend paneel ](assets/summary-subtasks-section.png)

## [!UICONTROL Hours]

Gebruik de sectie [!UICONTROL Hours] van [!UICONTROL Summary] om uren aan de taak of de kwestie te registreren u selecteerde. Klik op **[!UICONTROL Log Time]** en voer uw uren in. Als u rechtstreeks naar het tabblad Uren van de taak of uitgave wilt gaan, klikt u op de titel **[!UICONTROL Hours]** .

Het aantal uren in [!UICONTROL Summary] toont de uren u registreert. Andere gebruikers hebben verschillende totalen per uur in de [!UICONTROL Summary] , afhankelijk van de tijd waarop zij zich aanmelden voor de taak.

Als er geen gepland [!UICONTROL hours] op de taak of de kwestie zijn en u tijd hebt geregistreerd, toont de urenbar rood.

![ sectie van Uren in Samenvattend paneel ](assets/summary-hours-section.png)

## Goedkeuringen

Gebruik de sectie [!UICONTROL Approvals] van [!UICONTROL Summary] om goedkeuringen te bekijken verbonden aan de taak of de kwestie u selecteerde. Als u geen goedkeuringen hebt toegevoegd, selecteert u een bestaande goedkeuring in het keuzemenu of klikt u op **[!UICONTROL Create single-use approval process]** om rechtstreeks naar het tabblad [!UICONTROL Approvals] te gaan in de taak of uitgave.

Als u rechtstreeks naar het tabblad [!UICONTROL Approvals] van de taak of uitgave wilt gaan, klikt u op de titel **[!UICONTROL Approvals]** .

![ goedkeurt sectie in Samenvattend paneel ](assets/summary-approvals-section.png)
