---
title: Een aangepast formulier delen
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt toegang voor een douaneformulier vormen om te controleren wie-persoon, rol, groep, team, bedrijf-kan bekijken, delen, en het uitgeven.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# Een aangepast formulier delen

U kunt toegang voor een douaneformulier vormen om te controleren wie-persoon, rol, groep, team, bedrijf-kan bekijken, delen, en het uitgeven.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Voor informatie over hoe de beheerders van Workfront deze toegang verlenen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Toegang tot aangepaste formulieren {#access-to-custom-forms}

Wanneer u een nieuw aangepast formulier maakt en iemand dit aan een object koppelt, kan elke gebruiker die aan het object is toegewezen het formulier weergeven en invullen. Dit geldt ook voor gebruikers met aanvraaglicenties en externe gebruikers.

Op een object waaraan het aangepaste formulier nog niet is gekoppeld, kan een gebruiker het echter niet koppelen via het vervolgkeuzemenu Aangepaste Forms, zelfs niet bij een Planner-toegangsniveau:

* Iemand heeft het aangepaste formulier gedeeld met de gebruiker of met het team, de rol, de groep of het bedrijf van de gebruiker en geeft minimaal toestemming voor Weergave met de optie Bijvoegen bij aangepaste gegevens geselecteerd
* De gebruiker heeft een vergunning van het Plan en hun toegangsniveau verleent administratieve toegang tot douaneformulieren

## Een aangepast formulier delen

In plaats van een aangepast formulier in de standaard deelstatus te laten (beschreven in [Toegang tot aangepaste formulieren](#access-to-custom-forms) in dit artikel), kunt u specifieke niveaus van toegang tot het formulier voor bepaalde gebruikers, baanrollen, groepen, teams, en bedrijven vormen.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Selecteer het aangepaste formulier en klik op **Delen**.
1. In het vak dat wordt weergegeven, onder **Aangepaste formuliertoegang verlenen aan** typt u de naam van de gebruiker, het team, de taakrol, de groep of het bedrijf waarmee u het aangepaste formulier wilt delen. Druk vervolgens op **Enter** wanneer de naam wordt weergegeven.
1. Als u de toegang wilt aanpassen voor de gebruiker, het team, de taakrol, de groep of het bedrijf dat u net hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en configureert u vervolgens een van de volgende beschikbare opties en een van de geavanceerde instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>U kunt het aangepaste formulier weergeven en invullen op objecten.</p> <p><b>OPMERKING</b>: Voor gebruikers met een licentie voor werk, revisie en aanvragen is dit de hoogst beschikbare optie.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u het volgende wilt toestaan:</p> 
       <ul> 
        <li><strong>Koppelen aan aangepaste gegevens</strong>: Mogelijkheid om het aangepaste formulier te koppelen aan projecten, taken en problemen waarvoor zij toegang hebben tot Beheren</li> 
        <li> <p><strong>Delen</strong>: Mogelijkheid om het aangepaste formulier te delen met anderen in het systeem</p> <p>Gebruikers met een licentie voor werk, revisie of aanvragen kunnen een aangepast formulier alleen delen via de API of een aangepast formulierrapport. Zie voor meer informatie.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Alleen beschikbaar voor gebruikers met een licentie voor abonnementen. </p> <p>Gebruikers kunnen het formulier niet alleen toevoegen aan objecten die ze kunnen bewerken, maar kunnen ook het aangepaste formulier volledig bewerken, zoals velden toevoegen, bewerken en verwijderen.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u het volgende wilt toestaan:</p> 
       <ul> 
        <li> <p><strong>Koppelen aan aangepaste gegevens</strong>: Mogelijkheid om het aangepaste formulier te koppelen aan projecten, taken en problemen waarvoor zij toegang hebben tot Beheren</p> </li> 
        <li><strong>Verwijderen</strong>: Het aangepaste formulier verwijderen van het systeem</li> 
        <li><strong>Delen</strong>: Het aangepaste formulier delen met anderen in het systeem</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal stap 4-5 om andere namen aan de lijst toe te voegen en de opties te configureren.
1. (Optioneel) Als u de toegang tot het aangepaste formulier (op objecten waaraan het is gekoppeld) wilt beperken tot de objecten die u in de vorige stappen hebt opgegeven, klikt u op het tandwielpictogram ![](assets/gear-icon-settings-with-dn-arrow.jpg) in de rechterbovenhoek van het dialoogvenster voor delen klikt u op **Toegang voor het hele systeem verwijderen**.

   Als u van mening verandert, kunt u klikken **Dit voor het hele systeem zichtbaar maken** (de standaardoptie).

   >[!NOTE]
   >
   >* Wanneer u een aangepast formulier systeembreed zichtbaar maakt, staat u gebruikers toe het formulier alleen te bekijken en in te vullen op objecten waaraan ze zijn toegewezen, en niet het aan andere objecten te koppelen. U kunt de mogelijkheid bieden om het aangepaste formulier aan objecten te koppelen met de optie &quot;Bijvoegen aan aangepaste gegevens&quot; die in stap 5 wordt beschreven.
   >* De meeste organisaties willen ervoor zorgen dat iedereen in het systeem een douaneformulier kan invullen wanneer het aan voorwerpen wordt vastgemaakt zij werken en zijn gegevens in rapporten bekijken. Als dit voor uw organisatie waar is, adviseren wij dat u &quot;**Dit voor het hele systeem zichtbaar maken**.&quot; Wanneer de optie deze manier wordt gevormd, &quot;Zichtbare systeem-brede&quot;vertoningen in de dialoogdoos:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Als u zich zorgen maakt over een aangepast formulier waarin gebruikers vertrouwelijke gegevens kunnen invoeren wanneer deze aan bepaalde objecten zijn gekoppeld, beperkt u het delen voor deze objecten *objecten* Het zou beter kunnen zijn dan de toegang tot het formulier zelf te beperken.

1. Klikken **Opslaan**.

## Toegang tot een aangepast formulier verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Selecteer het aangepaste formulier en klik op **Delen**.
1. Klik in het vak dat wordt weergegeven op de X rechts van de naam van de gebruiker, het team, de rol, de groep of het bedrijf waartoe u geen speciale toegang meer wilt hebben.
1. (Optioneel) Herhaal de vorige stap naar voor andere namen die u wilt verwijderen.
1. Klikken **Opslaan**.
