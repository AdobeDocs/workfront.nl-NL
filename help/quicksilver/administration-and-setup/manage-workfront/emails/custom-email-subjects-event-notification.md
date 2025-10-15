---
navigation-topic: notifications
title: E-mailonderwerpen aanpassen voor gebeurtenismeldingen
description: U kunt de onderwerpregel van de e-mails die worden geactiveerd door gebeurtenismeldingen aanpassen.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# E-mailonderwerpen aanpassen voor gebeurtenismeldingen

U kunt de onderwerpregel van de e-mailberichten die worden geactiveerd door gebeurtenismeldingen aanpassen:

Het wijzigen van de onderwerpregel beïnvloedt alle gebruikers in het systeem, ongeacht het toegangsniveau van de ontvanger. Gebruikers zien alle objecten en velden die in het e-mailonderwerp zijn opgenomen.

Sommige gebeurtenismeldingen hebben meerdere onderwerpregel&#39;s, wat betekent dat deze gebeurtenismeldingen meerdere e-mailonderwerpen kunnen hebben op basis van hun functionaliteit.

>[!IMPORTANT]
>
>Wees voorzichtig wanneer u standaardvelden verwijdert, wanneer de onderwerpregel naar meerdere objecten verwijst. Hieronder volgt een lijst met gebeurtenismeldingen die dergelijke onderwerpregel bevatten:
>
>* Iemand neemt me op een geleide update
>* Iemand neemt mijn team op een geleide update
>* Commentaar van het Punt van het werk aan de Deelnemers van de draad
>* Opmerking voor werkitem om item toe te wijzen
>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Planner of hoger, met administratieve toegang tot herinneringsmeldingen</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## E-mailonderwerpregel aanpassen voor gebeurtenismeldingen {#customize-email-subject-lines-for-event-notifications}

{{step-1-to-setup}}

1. In het linkerpaneel, klik **E-mail** > **Meldingen**.

1. Klik de **Berichten van de Gebeurtenis** tabel.
1. Klik de naam van het gebeurtenisbericht u wilt aanpassen om het **vakje van het Bericht van de Gebeurtenis** te openen.
1. In het **vakje van de Lijn van het Onderwerp van 0&rbrace; E-mail &lbrace;, verander de tekst en de gebieden, met inbegrip van douanevelden, in het e-mailonderwerp.**

   De namen van de toegevoegde velden moeten overeenkomen met de hoofdlettersyntaxis van de kameel-database. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Klik **Update** om de nieuwe onderwerplijnen voor uw e-mails te bewaren.

## E-mailonderwerpregel aanpassen voor e-mails met meerdere objecten

Sommige gebeurtenismeldingen hebben meerdere onderwerpregel&#39;s, afhankelijk van de objecten die ze activeren.

&#39;Iemand neemt mij bijvoorbeeld op in een gestuurde update&#39; heeft twee verschillende onderwerpregel: ten eerste voor taken, uitgaven, sjabloontaken en documenten (ook wel &#39;referenceObject&#39; genoemd) en ten tweede voor objecten waarmee gebruikers opmerkingen kunnen maken, zoals een portfolio, programma, enzovoort (ook wel &#39;topReferenceObject&#39; genoemd).

![&#x200B; Gebeurtenis niet veelvoudige onderwerplijnen &#x200B;](assets/ev-multiple-subject.png)

Als een gebruiker in een gesprek over de taak, de kwestie, de malplaatjetaak, of het document inbegrepen is, zal een e-mail met de eerste onderwerpregel produceren. De onderwerpregel bevat &quot;referenceObject :name&quot;en het systeem bepaalt het voorwerp en toont de aangewezen naam op het onderwerpgebied. De e-mailonderwerpregel zou er ongeveer als volgt uitzien: &quot;Opmerking bij taak 123 op project ABC.&quot;

Als toegevoegd aan een projectgesprek zal een e-mail met het tweede onderwerp produceren. Hier bevat de onderwerpregel &quot;topReferenceObject :name&quot;en opnieuw identificeert Workfront welk voorwerp werd van verwijzingen voorzien en zal die objecten naam in plaats van &quot;topReferenceObject :name&quot;in het onderwerp terugkeren. De onderwerpregel van de e-mail ziet er ongeveer als volgt uit: &quot;Opmerking over project ABC.&quot;

Om de e-mailonderwerplijnen uit te geven en extra gebieden aan één van beide onderwerplijnen toe te voegen, zie [&#x200B; onderwerplijnen e-mail voor gebeurtenisberichten &#x200B;](#customize-email-subject-lines-for-event-notifications) in dit artikel aanpassen.

## E-mailonderwerpregel aanpassen voor e-mailberichten met meerdere acties

Sommige gebeurtenismeldingen hebben ook meerdere e-mailonderwerpen om de verschillende acties te beschrijven die op de objecten worden uitgevoerd.

Het aanvragen van een document om aan een uitgave toe te voegen, is bijvoorbeeld een gebeurtenis die twee verschillende e-mails kan activeren: een gebeurtenis die aangeeft wanneer het document wordt toegevoegd en een gebeurtenis die aangeeft wanneer het document wordt bewerkt.



![&#x200B; Gebeurtenis niet veelvoudige onderwerplijnen &#x200B;](assets/Ev-not-mult-subj-lines.png)

Om de e-mailonderwerplijnen uit te geven en extra gebieden aan één van beide onderwerplijnen toe te voegen, zie [&#x200B; onderwerplijnen e-mail voor gebeurtenisberichten &#x200B;](#customize-email-subject-lines-for-event-notifications) in dit artikel aanpassen.
