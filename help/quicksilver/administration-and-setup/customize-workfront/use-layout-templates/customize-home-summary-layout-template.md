---
title: Home en overzicht aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: U kunt een Malplaatje van de Lay-out gebruiken om te vormen wat de gebruikers zien wanneer zij een taak of een kwestie in Huis en in de Samenvatting klikken. Elke configuratie die u uitvoert met de onderstaande stappen, heeft op dezelfde manier invloed op het gebied Home en het deelvenster Samenvatting. Deze aanpassingen zijn niet van toepassing op het deelvenster Documentoverzicht.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 0%

---

# Home en overzicht aanpassen met een lay-outsjabloon

U kunt een Malplaatje van de Lay-out gebruiken om te vormen wat de gebruikers zien wanneer zij een taak of een kwestie in Huis en in de Samenvatting klikken. Elke configuratie die u uitvoert met de onderstaande stappen, heeft op dezelfde manier invloed op het gebied Home en het deelvenster Samenvatting. Deze aanpassingen zijn niet van toepassing op het deelvenster Documentoverzicht.

U kunt configureren:

* Welke velden worden weergegeven voor een taak of uitgave in het gebied Details en in welke volgorde
* Of updates, geregistreerde tijd, bijgevoegde documenten, en tijdstempels voor een geselecteerde taak of kwestie tonen

U kunt de gebieden ook aanpassen die de gebruikers in het gebied van het Huis zien wanneer de gebruikers een projectgoedkeuring, documentgoedkeuring, of de goedkeuring van de documentversie klikken die aan hen wordt toegewezen.

Voor informatie over het gebied Home raadpleegt u [Het gebied Home gebruiken](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Voor informatie over het deelvenster Samenvatting raadpleegt u [Overzicht van samenvattingen](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Voor informatie over het maken van lay-outsjablonen raadpleegt u [Lay-outsjablonen maken en beheren](../use-layout-templates/create-and-manage-layout-templates.md).

Voor informatie over lay-outsjablonen voor groepen raadpleegt u [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outsjabloon aan gebruikers raadpleegt u [Gebruikers toewijzen aan een lay-outsjabloon](../use-layout-templates/assign-users-to-layout-template.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Home en overzicht aanpassen met een lay-outsjabloon

1. Beginnen met het werken aan een lay-outsjabloon, zoals beschreven in [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klik op de pijl omlaag ![](assets/dropdown-arrow.png) krachtens **Aanpassen wat gebruikers zien** en klik vervolgens op **Home en overzicht**.

1. Klik in de lijst links op het objecttype (**Taken**, **Problemen**, **Projecten**, **Documenten**, of **Documentversies**) die u wilt aanpassen in Home en Summary.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Taken</td> 
      <td> <p>In Huis, beïnvloedt uw configuratie voor dit het plaatsen het gebied rechts van een taak wanneer een gebruiker de taak klikt. En in een takenlijst beïnvloedt dit het deelvenster Samenvatting dat aan de rechterkant van de pagina wordt weergegeven wanneer een gebruiker een taak selecteert en vervolgens op het pictogram Samenvatting openen klikt <img src="assets/summary-panel-icon.png">.</p> <p>U kunt bijvoorbeeld bepalen welke velden gebruikers zien in het gebied Details wanneer gebruikers taken selecteren in Home:</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>En wanneer zij een taak in het Overzicht selecteren:</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemen</td> 
      <td> <p>In Home beïnvloedt uw configuratie voor dit het plaatsen het gebied rechts van een kwestie wanneer een gebruiker de kwestie klikt.</p> <p>In een lijst met problemen beïnvloedt deze instelling het deelvenster Samenvatting dat aan de rechterkant van de pagina wordt weergegeven wanneer een gebruiker een probleem selecteert en vervolgens op het pictogram Samenvatting openen klikt <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projecten</td> 
      <td>In Huis, wanneer een gebruiker een projectgoedkeuring klikt die aan hen wordt toegewezen, beïnvloedt uw configuratie voor dit het plaatsen het gebied rechts van de goedkeuring.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td>Wanneer een gebruiker in Home op een aan hem toegewezen documentgoedkeuring klikt, is de configuratie voor deze instelling van invloed op het gebied rechts van de goedkeuring.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentversies</td> 
      <td>Wanneer een gebruiker in Home op een goedkeuring klikt die aan hem is toegewezen voor een bepaalde versie van een document, is de configuratie voor deze instelling van invloed op het gebied rechts van de goedkeuring.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Als een taak niet toegewezen is, zal de gebruiker die aan het lay-outmalplaatje wordt toegewezen niet de gebiedsaanpassingen in de Samenvatting zien.

1. (Voorwaardelijk) als u Taken of Kwesties in de vorige stap klikte, selecteer de categorie van taak of kwestie die u wilt aanpassen.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Voorwaardelijk) Als de optie **Knop primaire handeling instellen** wordt weergegeven (als u **Taken** of **Problemen** in de lijst links), klikt u op de primaire handeling (**Gereed** of **Status**) die u beschikbaar wilt maken voor gebruikers in het gebied Home en in het deelvenster Samenvatting wanneer zij een taak of een probleem bekijken.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Toevoegen ![](assets/add-item-plus-in-circle-blue.png) of verbergen ![](assets/close-or-hide---x.png) velden voor het geselecteerde objecttype.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Herhaal stap 3-6 om het gebied Home en het deelvenster Samenvatting aan te passen voor andere objecttypen.
1. Klikken **Algemene instellingen** Schakel vervolgens in of uit bij de linkerbenedenhoek een van de volgende opties voor Adobe Workfront-objecten in Home en Summary:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Updates tonen voor werk</td> 
      <td>Hiermee geeft u updates weer voor een geselecteerde taak of uitgave in Home of Summary. Dit omvat zowel systeemupdates als updates die door een gebruiker zijn gemaakt. Gebruikers kunnen systeemupdates nog steeds uitfilteren, zoals beschreven in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Systeemupdates in- of uitschakelen</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Werk bijwerken</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logtijd van arbeid</td> 
      <td>Hiermee geeft u de optie Logtijd weer tegen het werk als een taak of uitgave is geselecteerd, zodat gebruikers zich rechtstreeks vanuit het gebied Home en Summary kunnen aanmelden bij werkitems.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten weergeven die zijn gekoppeld aan werk</td> 
      <td>Hiermee geeft u een gebied Documenten weer in Home en Overzicht wanneer een taak of uitgave is geselecteerd en geeft u een lijst weer van de documenten die aan de taak of uitgave zijn gekoppeld. Gebruikers kunnen op documenten klikken om deze weer te geven in een voorvertoningsvenster.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tijdstempel verbergen</td> 
      <td>Hiermee verbergt u tijdstempels voor de volgende datumvelden in Home en Summary:
       <ul>
        <li>Geplande afsluitdatum</li>
        <li>Vastlegdatum</li>
        <li><p>Verzenddatum</p></li>
       </ul><p><b>OPMERKING</b>: Wanneer deze optie is ingeschakeld, worden de tijdelijke items die achterstallig worden, verplaatst naar de laatste groep in de lijst met thuiswerk, die alleen op datum is gebaseerd, en niet op tijd.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u klaar bent met het aanpassen, klikt u op **Opslaan**.

Voor meer informatie over lay-outsjablonen raadpleegt u [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
