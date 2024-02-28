---
navigation-topic: notifications
title: E-mailonderwerpen aanpassen voor gebeurtenismeldingen
description: U kunt de onderwerpregel van de e-mails die worden geactiveerd door gebeurtenismeldingen aanpassen.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '608'
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

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>Planner of hoger, met administratieve toegang tot herinneringsmeldingen</p> <p>Voor informatie over het geven van een de gebruikers administratieve toegang van het Plan, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## E-mailonderwerpregel aanpassen voor gebeurtenismeldingen {#customize-email-subject-lines-for-event-notifications}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **E-mail** > **Meldingen**.

1. Klik op de knop **Gebeurtenismeldingen** tab.
1. Klik op de naam van het gebeurtenisbericht dat u wilt aanpassen om het dialoogvenster **Melding gebeurtenis** doos.
1. In de **Onderwerpregel e-mail** de tekst en velden, inclusief aangepaste velden, in het e-mailonderwerp wijzigen.

   De namen van de toegevoegde velden moeten overeenkomen met de hoofdlettersyntaxis van de kameel-database. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Klikken **Bijwerken** om de nieuwe onderwerpregel voor uw e-mails op te slaan.

## E-mailonderwerpregel aanpassen voor e-mails met meerdere objecten

Sommige gebeurtenismeldingen hebben meerdere onderwerpregel&#39;s, afhankelijk van de objecten die ze activeren.

&#39;Iemand neemt mij bijvoorbeeld op in een gestuurde update&#39; heeft twee verschillende onderwerpregel: ten eerste voor taken, uitgaven, sjabloontaken en documenten (ook wel &#39;referenceObject&#39; genoemd) en ten tweede voor objecten waarmee gebruikers opmerkingen kunnen maken, zoals een portfolio, programma, enzovoort (ook wel &#39;topReferenceObject&#39; genoemd).

![](assets/Ev-not-mult-subj-lines.png)

Als een gebruiker in een gesprek over de taak, de kwestie, de malplaatjetaak, of het document inbegrepen is, zal een e-mail met de eerste onderwerpregel produceren. De onderwerpregel bevat &quot;referenceObject:name&quot; en het systeem definieert het object en geeft de juiste naam weer in het onderwerpveld. De e-mailonderwerpregel zou er ongeveer als volgt uitzien: &quot;Opmerking bij taak 123 op project ABC.&quot;

Als toegevoegd aan een projectgesprek zal een e-mail met het tweede onderwerp produceren. Hier bevat de onderwerpregel &quot;topReferenceObject:name&quot; en Workfront identificeert opnieuw welk object werd genoemd en retourneert die objectnaam in plaats van &quot;topReferenceObject:name&quot; in het onderwerp. De onderwerpregel van de e-mail ziet er ongeveer als volgt uit: &quot;Opmerking over project ABC.&quot;

Als u de onderwerpregel van de e-mail wilt bewerken en aanvullende velden wilt toevoegen aan de onderwerpregel, raadpleegt u [E-mailonderwerpregel aanpassen voor gebeurtenismeldingen](#customize-email-subject-lines-for-event-notifications) in dit artikel.

## E-mailonderwerpregel aanpassen voor e-mailberichten met meerdere acties

Sommige gebeurtenismeldingen hebben ook meerdere e-mailonderwerpen om de verschillende acties te beschrijven die op de objecten worden uitgevoerd.

Het aanvragen van een document om aan een uitgave toe te voegen, is bijvoorbeeld een gebeurtenis die twee verschillende e-mails kan activeren: een gebeurtenis die aangeeft wanneer het document wordt toegevoegd en een gebeurtenis die aangeeft wanneer het document wordt bewerkt.

![](assets/ev-not-mult-subj-lines-diff-actions.png)

Als u de onderwerpregel van de e-mail wilt bewerken en aanvullende velden wilt toevoegen aan de onderwerpregel, raadpleegt u [E-mailonderwerpregel aanpassen voor gebeurtenismeldingen](#customize-email-subject-lines-for-event-notifications) in dit artikel.
