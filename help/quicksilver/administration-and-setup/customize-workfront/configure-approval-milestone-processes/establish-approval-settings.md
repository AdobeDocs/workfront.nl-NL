---
title: Algemene goedkeuringsinstellingen configureren
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Als Adobe Workfront-beheerder kunt u de algemene instellingen voor goedkeuringsprocessen in Workfront bepalen. Deze instellingen zijn van invloed op alle goedkeuringsprocessen voor werkitems in uw systeem.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: 7f719c903ad4079470a6dbd046dce445ba227a5b
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Algemene goedkeuringsinstellingen configureren

Als Adobe Workfront-beheerder kunt u de algemene instellingen voor goedkeuringsprocessen in Workfront bepalen. Deze instellingen zijn van invloed op alle goedkeuringsprocessen voor werkitems in uw systeem.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet of een Beheerder van het Systeem zijn of een vergunning van het Plan met administratieve toegang tot de processen van de Goedkeuring hebben</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

+++

## Algemene goedkeuringsinstellingen configureren

{{step-1-to-setup}}

1. Klik **Processen** > **goedkeurt**.

1. Klik het **pictogram van Montages** pictogram ![&#x200B; Gear montagespictogram &#x200B;](assets/gear-icon-settings.png) naast de **goedkeurt** gebiedsnaam.

1. In het **vakje van de Montages van de Goedkeuring** dat verschijnt, specificeer de volgende informatie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">&lt;number&gt; dagen toevoegen aan geplande voltooiingsdatum om aan goedkeuringsprocessen te voldoen</td> 
      <td> <p>Geef het aantal minuten, uren, dagen, weken of maanden op om tijd toe te voegen aan de geplande voltooiingsdatum van de taak waarvoor goedkeuring nodig is. Selecteer "Verstreken" minuten, uren, dagen of weken om tijd toe te voegen die alle weekends, feestdagen en niet-werkuren bevat die zijn toegewezen in de agenda voor het systeemwerk.</p> 
      <p>Als een taak bijvoorbeeld op vrijdag is toegewezen en een duur van 3 verstreken dagen heeft, wordt de voltooiingsdatum van de taak ingesteld op maandag (ervan uitgaande dat zaterdag en zondag een weekend zijn). Als de taak drie dagen duurt (niet is verstreken), is de datum waarop de taak is voltooid, vastgesteld op woensdag.</p>
      <p><b> NOTA </b>: Het toelaten van de toevoeging van extra tijd om voor goedkeuring op taken aan te passen zal de chronologie van de taak en die van het project beïnvloeden.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fiatteur niet vereist om op het projectteam (voor goedkeuringsprocessen te zijn die een rol omvatten)</td> 
      <td> <p>Selecteer dit als een fiatteur niet op het projectteam moet zijn wanneer een goedkeuringsproces een rol omvat. Om het even welke gebruiker met die baanrol ontvangt het goedkeuringsverzoek of zij op het projectteam of niet zijn, hoewel zij niet automatisch toegang tot het project worden verleend. Voor informatie over het uitgeven van het projectrol van een gebruiker, zie <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref"> het Team van het Project beheren </a>. </p> 
      <p><b> TIP </b>: Wanneer u een goedkeuring aan een rol toewijst en de optie <b> fiatteur niet op het projectteam (voor goedkeuringsprocessen moet zijn die een rol omvatten) </b> is gehandicapt, maar er zijn geen rollen in het projectteam die de rol op de goedkeuring aanpassen, wordt de goedkeuring opnieuw toegewezen aan de Eigenaar van het Project. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Goedkeuringsdelegatie uitschakelen</td> 
      <td> <p>Selecteer deze optie om de functionaliteit voor gebruikers in uw systeem om goedkeuringen aan een andere gebruiker te delegeren onbruikbaar te maken. Als deze optie is geselecteerd, wordt de optie om goedkeuringen te delegeren uit Workfront verwijderd en worden bestaande goedkeuringsdelegaties gestopt.</p> <p>Voor meer informatie over het delegeren van goedkeuringen in Workfront, zie <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref"> de goedkeuringsverzoek van de Afgevaardigde </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Het bewerken van het aangepaste formulier toestaan wanneer de goedkeuringsstatus voor het project, de taak of het probleem in behandeling is</td> 
      <td> <p>Selecteer deze optie als u wilt dat gebruikers de aangepaste vorm van projecten, taken en problemen kunnen bewerken in de status In afwachting van goedkeuring. Dit is de standaardinstelling.</p> 
      <p>Wanneer deze optie is geselecteerd:</p> 
       <ul> 
       <li>Alle fiatteurs (en alle andere gebruikers die toegang hebben om het aangepaste formulier te bewerken) kunnen wijzigingen aanbrengen in het aangepaste formulier wanneer het object in afwachting is van goedkeuring, ongeacht het huidige goedkeuringspad of de huidige goedkeuringsstap.</li> 
       <li>Wijzigingen die tijdens een goedkeuringsproces in het aangepaste formulier worden aangebracht, hebben geen invloed op goedkeuringsbesluiten die vóór de wijziging zijn genomen.</li> 
       <li> <p>Alle wijzigingen die in het project, de taak of het probleem zijn aangebracht, worden op dezelfde manier bijgehouden, ongeacht deze instelling. </p> <p>Als u bijvoorbeeld aangepaste formuliervelden hebt toegevoegd die in de updatestream moeten worden bijgehouden, worden wijzigingen in het formulier bijgehouden in de updatestream van het object.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers toestaan om nieuwe aanvragen in afwachting van goedkeuring in herinnering te roepen</td> 
      <td> <p>Selecteer deze optie om te vormen of de gebruikers een kwestie of een verzoek in afwachting van goedkeuring voor hun eerste status kunnen herinneren. U kunt de eerste status van een kwestie of een verzoek met een goedkeuringsproces associëren door verzoekrijen te vormen. </p> 
      <p>Voor meer informatie over verzoekrijen, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref"> een Rij van het Verzoek </a> creëren.</p> 
      <p>Voer een van de volgende handelingen uit:</p> 
       <ul> 
       <li>Selecteer deze optie als u wilt dat gebruikers een goedkeuring voor de eerste status van een uitgave of een verzoek kunnen onthouden. In dit geval zien ze een knop Opnieuw&lt; op een nieuwe uitgave of aanvraag in afwachting van de goedkeuringsstatus. Wanneer zij ervoor kiezen het probleem te melden, wordt hen gewaarschuwd dat het probleem ook wordt verwijderd. De kwestie wordt geschrapt nadat zij het herinneren hebben bevestigd. </li> 
       <li> <p>Schakel deze optie uit als u wilt voorkomen dat gebruikers een probleem of een verzoek terugroepen waarvan de eerste status in afwachting is van goedkeuring. Ze kunnen geen knop Recall&lt; zien op de nieuwe uitgave of aanvraag en de goedkeuring moet worden verleend. Dit is de standaardoptie.</p> 
       <p>Voor meer informatie over het herzien van punten die op goedkeuring wachten, zie <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref"> goedkeuringen van de Mening </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen Veranderingen.**
