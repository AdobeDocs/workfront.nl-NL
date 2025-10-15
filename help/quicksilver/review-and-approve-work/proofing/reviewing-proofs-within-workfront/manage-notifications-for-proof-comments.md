---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Meldingen beheren voor proefopmerkingen en -beslissingen
description: Wanneer u aan een proefdruk werkt, of u een gebruiker van Adobe Workfront of een externe medewerker bent, kunt u specificeren welke e-mailberichten u over commentaren en besluiten over de proefdruk wilt ontvangen. Voor meer informatie, zie Berichten voor het proefdrukcommentaren en besluitoverzicht.
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 385f4a6663cacfdcf519bf5699fc1840c2cb2adc
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 0%

---

# Meldingen beheren voor proefopmerkingen en -beslissingen

<!-- Audited: 4/2025 -->

Wanneer u aan een proefdruk werkt, of u een gebruiker van Adobe Workfront of een externe medewerker bent, kunt u specificeren welke e-mailberichten u over commentaren en besluiten over de proefdruk wilt ontvangen. Voor meer informatie, zie [ Meldingen voor de proefdrukcommentaren en besluiten overzicht ](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>Deze meldingen verschillen van de e-mailwaarschuwingen die u kunt ontvangen over de stroom van een proefdruk onder controleurs en over de instellingen voor e-mailwaarschuwingen die u kunt configureren in Workfront.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proefdrukrol </td> 
   <td>Revisor, Reviewer en fiatteur, auteur, moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Meldingen beheren voor proefopmerkingen en -beslissingen

1. Open de proefdruk u berichten voor wilt vormen.
1. Als de linkertoolbar niet toont, klik het **pictogram van het Menu** in de upper-left hoek van de Kijker van het Bewijs van het Web.

   ![ Menu_icon_in_Proofing_Viewer.png ](assets/menu-icon-in-proofing-viewer-350x228.png)

1. In de linkertoolbar, klik het **pictogram van Montages** Settings_icon.png ![.](assets/settings-icon.png)

1. In **verzend me e-mailberichten over** sectie, selecteer het bericht dat voor deze proef plaatst.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle activiteiten</td> 
      <td>Telkens wanneer er activiteiten aan het bewijs worden toegevoegd, zoals een nieuwe opmerking, een nieuw antwoord of een nieuw besluit, wordt er een e-mail naar de controleur verzonden.<br><p>Deze instelling wordt aanbevolen voor de persoon die het proefdrukproces beheert, omdat deze de activiteit kan zien zoals deze plaatsvindt. Gebruikers ontvangen geen e-mailwaarschuwing over hun eigen activiteiten (bijvoorbeeld opmerkingen, antwoorden of genomen besluiten).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reacties op mijn opmerkingen</td> 
      <td>Een e-mail wordt alleen naar de controleur verzonden als iemand rechtstreeks op zijn opmerking reageert (zonder zijn reacties op zijn eigen opmerkingen).<p>Deze instelling wordt aanbevolen voor uw klanten, zodat deze alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen en niet van andere opmerkingen die op de proefdruk zijn gemaakt, hoewel ze alle opmerkingen in de proefdrukviewer kunnen bekijken.</p>
      <p>Voor informatie, zie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref"> Mening en antwoord aan proefdrukcommentaren </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Besluiten</td> 
      <td>Een e-mail wordt alleen naar de controleur verzonden wanneer iemand een beslissing neemt.<br><p>Deze e-mailwaarschuwing kan nuttig zijn voor de persoon die het goedkeuringsproces beheert, omdat de persoon die het goedkeuringsproces beheert, de voortgang van het bewijs kan volgen en kan zien welke gebruikers hun beslissing hebben genomen.<br></p><p>Je wordt pas op de hoogte gesteld van je eigen beslissing als je een bevestigingsoptie voor e-mail selecteert wanneer je je beslissing verzendt.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Definitief besluit</td> 
      <td>Er wordt een e-mail verzonden wanneer de definitieve beslissing op het bewijs wordt genomen.<br><p>Deze waarschuwing wordt vaak gebruikt door de ontwerper omdat de ontwerper niet aan de daadwerkelijke overzichtsbespreking hoeft deel te nemen. Wanneer het definitieve besluit wordt genomen, wordt de ontwerper op de hoogte gebracht en kan dan actie ondernemen op om het even welke noodzakelijke veranderingen.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uuroverzicht</td> 
      <td>Elk uur wordt een e-mail naar de controleur verzonden met een overzicht van alle opmerkingen, antwoorden en beslissingen die in het afgelopen uur zijn genomen.<br><p>Het e-mailbericht wordt alleen verzonden wanneer er in het afgelopen uur andere activiteiten plaatsvinden dan die van uzelf. Als andere gebruikers geen activiteiten uitvoeren, wordt geen e-mail verzonden.<br></p><p>Deze waarschuwing is een goede manier om een overzicht van het project te zien aangezien het vordert.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dagelijkse samenvatting</td> 
      <td>(Standaardinstelling): elke dag wordt een e-mail verzonden met alle opmerkingen, antwoorden en beslissingen in de lijst. Dit wordt alleen op dagen verzonden wanneer er andere activiteiten zijn dan die van uzelf.<br><p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geen e-mail</td> 
      <td>Er worden geen e-mailwaarschuwingen verzonden.<br><p>Deze instelling is handig voor een persoon die alleen ter referentie aan een proefdruk wordt toegevoegd en die niet op de hoogte hoeft te worden gesteld van wijzigingen.</p><p>Opmerking: <p>Met deze optie schakelt u alleen e-mailwaarschuwingen over proefdrukopmerkingen en -beslissingen uit. De e-mailwaarschuwingen die u kunt ontvangen over de stroom van een proefdruk, zoals de nieuwe proefdruk of de e-mail met de nieuwste proefdruk, worden niet uitgeschakeld. Raadpleeg de volgende artikelen voor meer informatie: </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">Nieuwe proefe-mail</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">Het e-mailbericht voor de nieuwe versie</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">E-mailadres voor proefdrukken</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">De e-mail met bewijs</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
