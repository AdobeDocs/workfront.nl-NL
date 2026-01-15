---
title: Het deelvenster Samenvatting aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: U kunt een Malplaatje van de Lay-out gebruiken om te vormen wat de gebruikers zien wanneer zij een taak of een kwestie in het Overzicht klikken. Elke configuratie die u uitvoert met de onderstaande stappen, is van invloed op het deelvenster Samenvatting. Deze aanpassingen zijn niet van toepassing op het deelvenster Documentoverzicht.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# Het deelvenster Samenvatting aanpassen met een lay-outsjabloon

<!--Audited: 11/2024-->

U kunt een Lay-outsjabloon gebruiken om te configureren wat gebruikers in het deelvenster Overzicht zien wanneer ze op een taak of een probleem klikken. Elke configuratie die u uitvoert met de onderstaande stappen, is van invloed op het deelvenster Samenvatting. Deze aanpassingen zijn niet van toepassing op het deelvenster Documentoverzicht.

U kunt configureren:

* Welke velden worden weergegeven voor een taak of uitgave in het gebied Details en in welke volgorde
* Of updates, geregistreerde tijd, bijgevoegde documenten, en tijdstempels voor een geselecteerde taak of kwestie tonen

U kunt de gebieden ook aanpassen die de gebruikers in het gebied van het Huis zien wanneer de gebruikers een projectgoedkeuring, documentgoedkeuring, of de goedkeuring van de documentversie klikken die aan hen wordt toegewezen.

Voor informatie over het Summiere paneel, zie [&#x200B; Overzicht &#x200B;](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Voor informatie over het creëren van lay-outmalplaatjes, zie [&#x200B; lay-outmalplaatjes &#x200B;](../use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

Voor informatie over lay-outmalplaatjes voor groepen, zie [&#x200B; tot stand brengen en wijzigen de lay-outmalplaatjes van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outmalplaatje aan gebruikers, zie [&#x200B; gebruikers aan een lay-outmalplaatje &#x200B;](../use-layout-templates/assign-users-to-layout-template.md) toewijzen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.</p>
        <p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het deelvenster Samenvatting aanpassen met een lay-outsjabloon

1. Begin werkend aan een lay-outmalplaatje, zoals die in [&#x200B; wordt beschreven creeer en beheer lay-outmalplaatjes &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klik de benedenpijl ![&#x200B; benedenpijl &#x200B;](assets/dropdown-arrow.png) onder **aanpassen welke gebruikers** zien, dan klik **Samenvattend paneel**.

1. Klik in de lijst die eronder wordt weergegeven op het objecttype waarvoor u het deelvenster Samenvatting wilt aanpassen.

   In de onderstaande tabel wordt uitgelegd wat u voor elk object kunt aanpassen

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Taken</td> 
      <td> <p>In een takenlijst beïnvloedt deze instelling het deelvenster Samenvatting dat aan de rechterkant van de pagina wordt weergegeven wanneer een gebruiker een taak selecteert en vervolgens op het pictogram Samenvatting openen <img src="assets/summary-panel-icon.png"> klikt.</p>

   <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemen</td> 
      <td><p>In een lijst met problemen beïnvloedt deze instelling het deelvenster Samenvatting dat aan de rechterkant van de pagina wordt weergegeven wanneer een gebruiker een probleem selecteert en vervolgens op het pictogram Samenvatting openen <img src="assets/summary-panel-icon.png"> klikt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

<!--These were removed with the new Home: 

<tr> 
      <td role="rowheader">Projects</td> 
      <td><ul><li><p>In Home, when a user clicks a project approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p>This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documents</td> 
      <td>
     <ul><li><p>In Home, when a user clicks a document approval assigned to them, your configuration for this setting affects the area to the right of the approval.</p>
      <p><b>IMPORTANT:</b> </p><p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Document Versions</td> 
      <td><ul><li><p>In Home, when a user clicks an approval assigned to them for a particular version of a document, your configuration for this setting affects the area to the right of the approval.</p>
      <p><p><b>IMPORTANT:</b></p> This is a deprecated feature. Any changes you make to this area are related to a feature that Workfront has removed. This option will be removed from Workfront with a later maintenance update.</p></li>
      </ul>
      </td> 
     </tr> -->


>[!IMPORTANT]
>
>Als een taak niet toegewezen is, zal de gebruiker die aan het lay-outmalplaatje wordt toegewezen niet de gebiedsaanpassingen in de Samenvatting zien.

1. (Voorwaardelijk) als u Taken of Kwesties in de vorige stap klikte, selecteer de categorie van taak of kwestie die u wilt aanpassen.

   ![&#x200B; verkies categorie om aan te passen &#x200B;](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Voorwaardelijk) als de **Vastgestelde primaire actieknoop** drop-down menu verschijnt (als u **Taken** of **Kwesties** in de lijst op de linkerzijde) selecteert, klik de primaire actie (**Gedaan** of **Status**) die u beschikbaar voor gebruikers in het Samenvattende paneel wilt wanneer zij een taak of een kwestie bekijken.

   ![&#x200B; plaats primaire actie &#x200B;](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Voeg ![&#x200B; punt &#x200B;](assets/add-item-plus-in-circle-blue.png) toe of verberg ![&#x200B; punt &#x200B;](assets/close-or-hide---x.png) gebieden van de Huid voor het geselecteerde objecten type.

   ![&#x200B; voeg en verberg gebieden toe &#x200B;](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Herhaal stap 3-6 om het deelvenster Samenvatting aan te passen voor andere objecttypen.
1. Klik **Globale montages**, dichtbij de lagere linkerhoek, dan toelaten of onbruikbaar maken om het even welke volgende opties met betrekking tot de voorwerpen van Adobe Workfront in de Samenvatting:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Updates tonen voor werk</td> 
      <td>Hiermee geeft u updates weer voor een geselecteerde taak of uitgave in het deelvenster Samenvatting. Dit omvat zowel systeemupdates als updates die door een gebruiker zijn gemaakt. De gebruikers kunnen systeemupdates nog uit filtreren, zoals die in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref"> worden beschreven toelaten of systeemupdates </a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref"> werk van de Update </a> onbruikbaar maken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logtijd van arbeid</td> 
      <td>Hiermee geeft u de optie Logtijd weer tegen het werk als een taak of uitgave is geselecteerd, zodat gebruikers zich rechtstreeks vanuit het gebied Home en Summary kunnen aanmelden bij werkitems.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten weergeven die zijn gekoppeld aan werk</td> 
      <td>Hiermee geeft u een gebied Documenten in het deelvenster Samenvatting weer wanneer een taak of uitgave is geselecteerd en alle documenten worden weergegeven die aan de taak of uitgave zijn gekoppeld. Gebruikers kunnen op documenten klikken om deze weer te geven in een voorvertoningsvenster.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tijdstempel verbergen</td> 
      <td>Hiermee verbergt u tijdstempels voor de volgende datumvelden in het deelvenster Samenvatting:
       <ul>
        <li>Geplande afsluitdatum</li>
        <li>Vastlegdatum</li>
        <li>Verzenddatum</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Blijf het lay-outmalplaatje aanpassen. U kunt **klikken** op elk ogenblik van toepassing zijn om uw vooruitgang te bewaren.

   of

   Als u wordt gebeëindigd aanpassend, klik **sparen en sluit**.

Voor meer informatie over lay-outmalplaatjes, zie [&#x200B; lay-outmalplaatjes &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.
