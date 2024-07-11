---
product-area: requests
navigation-topic: create-requests
title: Gebruikers toestaan een uitgave per e-mail te verzenden naar een aanvraagwachtrij-project
description: Gebruikers toestaan een uitgave per e-mail te verzenden naar een aanvraagwachtrij-project
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 9cda6fd41ba7fcb9b9f412a7c2b7ffd39f3fe189
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Gebruikers toestaan een uitgave per e-mail te verzenden naar een aanvraagwachtrij-project

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

U kunt een project vormen om gebruikers toe te staan om kwesties aan het project via e-mail toe te voegen. U kunt voor kwesties toestaan om in een project worden gemaild slechts als het project als Rij van het Verzoek wordt aangewezen. Voor meer informatie over het creëren van een project van de Rij van het Verzoek, zie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

De volgende eerste vereisten worden vereist om een project te vormen om gebruikers toe te staan om kwesties aan het project via e-mail toe te voegen.

Aan deze voorwaarden moet worden voldaan voordat u deze functie kunt inschakelen:

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
1. Klikken **Wachtrij** in het linkerdeelvenster. Mogelijk moet u op **Meer weergeven** eerst.
1. In de **Type wachtrij** gebied, selecteren **Publish as Help Request-wachtrij**.

1. Omlaag schuiven naar de **E-mailwachtrijinstellingen** gebied, selecteert u vervolgens **Aanvraag via e-mail inschakelen**.

1. Voer het begin van het e-mailadres in het dialoogvenster **E-mailadres invoegen** doos.

   U moet een uniek e-mailadres maken. We raden u aan uw bedrijfsnaam te gebruiken als onderdeel van uw e-mailadres voor inname.

   >[!CAUTION]
   >
   >* Dit e-mailadres kan niet uit de prullenbak worden teruggekregen als het project dat de verzoekrij bevat wordt geschrapt.
   >
   >* Omdat dit e-mailadres uniek moet zijn, is het mogelijk niet meer beschikbaar als het wordt verwijderd.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Optioneel) Selecteer de optie **Alle problemen doorsturen die niet via e-mail worden verzonden**, dan ga een door:sturen e-mailadres in de doos hieronder in.

   Dit e-mailadres ontvangt informatie over e-mailberichten die niet zijn verzonden naar het project.

1. Klikken **Opslaan**. Wanneer gebruikers met een actieve Workfront-account nu een e-mail naar dit e-mailadres sturen, wordt er een uitgave gemaakt in het Workfront-project.

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
* De gebruiker die het e-mailbericht verzendt, wordt de primaire contactpersoon van de nieuwe uitgave in Workfront.
* De hoofdtekst van de e-mail mag niet meer dan 4000 tekens bevatten.
* E-mailbijlagen mogen in totaal niet groter zijn dan 7 MB.
