---
product-area: requests
navigation-topic: create-requests
title: Gebruikers toestaan een probleem te e-mailen naar een aanvraagwachtrij-project
description: U kunt een project vormen om gebruikers toe te staan om kwesties aan het project via e-mail toe te voegen.
author: Becky
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---

# Gebruikers toestaan een uitgave per e-mail te verzenden naar een aanvraagwachtrij-project

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

U kunt een project vormen om gebruikers toe te staan om kwesties aan het project via e-mail toe te voegen. U kunt kwesties slechts toestaan om in een project worden gemaild als het project als Rij van het Verzoek wordt aangewezen. Voor meer informatie over het creëren van een project van de Rij van het Verzoek, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>U moet Adobe Workfront Planning hebben om de verzoeken van de Planning te bekijken of om formulieren te verzoeken</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

De volgende voorwaarden worden vereist om een project te vormen om gebruikers toe te staan om kwesties aan het project via e-mail toe te voegen:

* Gebruikers die problemen naar dit account e-mailen, moeten actieve gebruikers zijn met een licentie voor Workfront.
* Gebruikers die problemen naar deze account e-mailen, moeten beschikken over de machtiging Uitgave toevoegen voor het project.
* Externe gebruikers kunnen geen problemen per e-mail verzenden naar een aanvraagwachtrij omdat zij geen toegang hebben om problemen te maken.
* Alleen e-mails die afkomstig zijn van een e-mailadres dat is gekoppeld aan een actieve Workfront-gebruiker, mogen problemen verzenden naar het project. E-mails die via een e-mailbericht dat niet aan een Workfront-account is gekoppeld naar een actieve Workfront-gebruiker worden doorgestuurd, kunnen geen problemen in het kader van het project veroorzaken, omdat het e-mailadres van de oorspronkelijke afzender aan een actief Workfront-account moet worden gekoppeld.
* Het project is opstelling als Rij van het Verzoek.
* De e-mailaccount die aan het project is gekoppeld, is niet gekoppeld aan een Workfront-gebruikersaccount.

## Het project in Workfront configureren

>[!NOTE]
>
>Houd rekening met het volgende wanneer u instellingen voor e-mailwachtrijen inschakelt:
>
>* Workfront staat één unieke e-mail per aanvraagwachtrij toe voor alle clusters. Als u ervoor kiest om uw aanvraagwachtrij uit te schakelen, behoudt u het e-mailadres dat u hebt gemaakt zolang dit zich nog in het vak E-mailadres invoegen bevindt. Als u ervoor kiest het gebruik van de inname-e-mail te beëindigen, moet u deze verwijderen uit het veld E-mailbericht innemen, zodat deze later kan worden gebruikt.
>
>* Als de verzoekrij veelvoudige rijonderwerpen of onderwerpgroepen heeft, zal Workfront willekeurig het rijonderwerp selecteren dat de gemailde verzoeken zullen gaan naar, makend gemailde verzoeken moeilijk te beheren.
>Wij adviseren dat het project dat u opstelling om verzoeken door e-mail te ontvangen niet meer dan één rijonderwerp zou moeten hebben. Als de voorgelegde verzoeken voor verschillende middelen of projecten bedoeld zijn zou u hen moeten leiden of manueel bewegen, nadat zij zijn voorgelegd.

1. Ga naar het project dat u wilt inschakelen om problemen via e-mail te ontvangen.
1. Klik **Details van de Rij** in het linkerpaneel.
1. In het **gebied van het Type van Rij 0}, uitgezocht** publiceer als Rij van het Verzoek van de Hulp **.**

1. De rol neer aan het **gebied van de Montages van de Rij 0} E-mail, dan selecteert** laat de opname van het Verzoek via e-mail **toe.**

1. Ga het begin van het e-mailadres in het **Inname E-mailadres** vakje in.

   U moet een uniek e-mailadres maken. We raden u aan uw bedrijfsnaam te gebruiken als onderdeel van uw e-mailadres voor inname.

   >[!CAUTION]
   >
   >* Dit e-mailadres kan niet uit de prullenbak worden teruggekregen als het project dat de verzoekrij bevat wordt geschrapt.
   >
   >* Omdat dit e-mailadres uniek moet zijn, is het mogelijk niet meer beschikbaar als het wordt verwijderd.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in Workfront. Only emails created from this email address are added as issues.
   -->

1. (Facultatief) selecteer **door:sturen alle kwesties die er niet in slagen via e-mail** voor te leggen, dan ga een het door:sturen e-mailadres in de doos hieronder in.

   Dit e-mailadres ontvangt informatie over e-mailberichten die niet zijn verzonden naar het project.

1. Klik **sparen**. Wanneer gebruikers met een actieve Workfront-account nu een e-mail naar dit e-mailadres sturen, wordt er een uitgave gemaakt in het Workfront-project.

   >[!NOTE]
   >
   >Gebruikers moeten toegang hebben om uitgaven in het project te maken om via e-mail te kunnen verzenden. U kunt deze toegang verlenen in het dialoogvenster Delen onder Geavanceerde instellingen.
   >
   >Externe gebruikers kunnen geen problemen per e-mail verzenden naar een aanvraagwachtrij omdat zij geen toegang hebben om problemen te maken.

## Ontvang het probleem in Workfront

Wanneer een Workfront-gebruiker een e-mailbericht naar Workfront verzendt, gebeurt het volgende:

* De onderwerpregel van de e-mail wordt de Naam van de Uitgave.
* De hoofdtekst van de e-mail wordt de beschrijving van de uitgave.
* Als er documenten bij het e-mailbericht horen, worden deze documenten in Workfront bij de uitgave gevoegd.

  >[!NOTE]
  >
  > MSG-bestanden worden niet ondersteund en worden niet aan het probleem gekoppeld in Workfront.

* De gebruiker die het e-mailbericht verzendt, wordt de primaire contactpersoon van de nieuwe uitgave in Workfront.
* De hoofdtekst van de e-mail mag niet meer dan 4000 tekens bevatten.
* E-mailbijlagen mogen in totaal niet groter zijn dan 7 MB.
