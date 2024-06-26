---
title: Een aangepast formulier delen
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt toegang voor een douaneformulier vormen om te controleren wie-persoon, rol, groep, team, bedrijf-kan bekijken, delen, en het uitgeven.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 6c43d836c24f893d1b7d7d01c1dd0b1cc3fba357
workflow-type: tm+mt
source-wordcount: '1408'
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
   <td role="rowheader"> <p>Adobe Workfront-plan</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Toegang tot aangepaste formulieren {#access-to-custom-forms}

Wanneer u een nieuw aangepast formulier maakt en iemand dit aan een object koppelt, kan elke gebruiker die aan het object is toegewezen het formulier weergeven en invullen. Dit geldt ook voor gebruikers met aanvraaglicenties en externe gebruikers.

Op een object waaraan het aangepaste formulier nog niet is gekoppeld, kan een gebruiker het echter niet koppelen via het vervolgkeuzemenu Aangepaste Forms, zelfs niet bij een Planner-toegangsniveau:

* Iemand heeft het aangepaste formulier gedeeld met de gebruiker of met het team, de rol, de groep of het bedrijf van de gebruiker en geeft minimaal toestemming voor Weergave met de optie Bijvoegen bij aangepaste gegevens geselecteerd
* De gebruiker heeft een vergunning van het Plan en hun toegangsniveau verleent administratieve toegang tot douaneformulieren

## Een aangepast formulier delen vanuit de lijst met formulieren

In plaats van een aangepast formulier in de standaard deelstatus te laten (beschreven in [Toegang tot aangepaste formulieren](#access-to-custom-forms) in dit artikel), kunt u specifieke niveaus van toegang tot het formulier voor bepaalde gebruikers, baanrollen, groepen, teams, en bedrijven vormen.

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Selecteer het aangepaste formulier en klik op ![Pictogram Delen](assets/share-icon.png).
1. In het vak dat wordt weergegeven, onder **Aangepaste formuliertoegang verlenen aan** typt u de naam van de gebruiker, het team, de taakrol, de groep of het bedrijf waarmee u het aangepaste formulier wilt delen. Druk vervolgens op **Enter** wanneer de naam wordt weergegeven.
1. Als u de toegang wilt aanpassen voor de gebruiker, het team, de taakrol, de groep of het bedrijf dat u net hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en configureert u vervolgens een van de volgende beschikbare opties en een van de geavanceerde instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>U kunt het aangepaste formulier weergeven en invullen op objecten.</p> <p><b>OPMERKING</b>: Voor gebruikers met lichte licenties en bijdragelicenties (of Work-, Review- en Request-licenties) is dit de hoogst beschikbare optie.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u het volgende wilt toestaan:</p> 
       <ul> 
        <li><strong>Koppelen aan aangepaste gegevens</strong>: Mogelijkheid om het aangepaste formulier te koppelen aan projecten, taken en problemen waarvoor zij toegang hebben tot Beheren</li> 
        <li> <p><strong>Delen</strong>: Mogelijkheid om het aangepaste formulier te delen met anderen in het systeem</p> <p>Gebruikers met een licentie voor licht of contribuant (of een licentie voor werken, revisie of aanvragen) kunnen een aangepast formulier alleen delen via de API of een aangepast formulierrapport.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Alleen beschikbaar voor gebruikers met een Standard- of Plan-licentie. </p> <p>Gebruikers kunnen het formulier niet alleen toevoegen aan objecten die ze kunnen bewerken, maar kunnen ook het aangepaste formulier volledig bewerken, zoals velden toevoegen, bewerken en verwijderen.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u het volgende wilt toestaan:</p> 
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
   >* De meeste organisaties willen ervoor zorgen dat iedereen in het systeem een douaneformulier kan invullen wanneer het aan voorwerpen wordt vastgemaakt zij werken en zijn gegevens in rapporten bekijken. Als dit voor uw organisatie waar is, adviseren wij dat u gebruikt **Dit voor het hele systeem zichtbaar maken**. Wanneer de optie deze manier wordt gevormd, &quot;Zichtbare systeem-brede&quot;vertoningen in de dialoogdoos:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Als u zich zorgen maakt over een aangepast formulier waarin gebruikers vertrouwelijke gegevens kunnen invoeren wanneer deze aan bepaalde objecten zijn gekoppeld, beperkt u het delen voor deze objecten *objecten* Het zou beter kunnen zijn dan de toegang tot het formulier zelf te beperken.

1. Klikken **Opslaan**.

## Een aangepast formulier delen vanuit de formulierontwerper

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Open een aangepast formulier of maak een nieuw aangepast formulier.
1. Klikken **Delen** rechtsboven in de formulierontwerper als u klaar bent om het formulier te delen.
1. In het vak dat wordt weergegeven, onder **Aangepaste formuliertoegang verlenen aan** typt u de naam van de gebruiker, het team, de taakrol, de groep of het bedrijf waarmee u het aangepaste formulier wilt delen. Druk vervolgens op **Enter** wanneer de naam wordt weergegeven.
1. Als u de toegang wilt aanpassen voor de gebruiker, het team, de taakrol, de groep of het bedrijf dat u net hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en configureert u vervolgens een van de volgende beschikbare opties en een van de geavanceerde instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>U kunt het aangepaste formulier weergeven en invullen op objecten.</p> <p><b>OPMERKING</b>: Voor gebruikers met lichte licenties en bijdragelicenties (of Work-, Review- en Request-licenties) is dit de hoogst beschikbare optie.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u het volgende wilt toestaan:</p> 
       <ul> 
        <li><strong>Koppelen aan aangepaste gegevens</strong>: Mogelijkheid om het aangepaste formulier te koppelen aan projecten, taken en problemen waarvoor zij toegang hebben tot Beheren</li> 
        <li> <p><strong>Delen</strong>: Mogelijkheid om het aangepaste formulier te delen met anderen in het systeem</p> <p>Gebruikers met een licentie voor licht of contribuant (of een licentie voor werken, revisie of aanvragen) kunnen een aangepast formulier alleen delen via de API of een aangepast formulierrapport.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Alleen beschikbaar voor gebruikers met een Standard- of Plan-licentie. </p> <p>Gebruikers kunnen het formulier niet alleen toevoegen aan objecten die ze kunnen bewerken, maar kunnen ook het aangepaste formulier volledig bewerken, zoals velden toevoegen, bewerken en verwijderen.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u het volgende wilt toestaan:</p> 
       <ul> 
        <li> <p><strong>Koppelen aan aangepaste gegevens</strong>: Mogelijkheid om het aangepaste formulier te koppelen aan projecten, taken en problemen waarvoor zij toegang hebben tot Beheren</p> </li> 
        <li><strong>Verwijderen</strong>: Het aangepaste formulier verwijderen van het systeem</li> 
        <li><strong>Delen</strong>: Het aangepaste formulier delen met anderen in het systeem</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal stap 5-6 om andere namen aan de lijst toe te voegen en hun opties te configureren.
1. (Optioneel) Als u de toegang tot het aangepaste formulier (op objecten waaraan het is gekoppeld) wilt beperken tot de objecten die u in de vorige stappen hebt opgegeven, klikt u op de vervolgkeuzepijl onder **Wie toegang heeft** selecteert u vervolgens **Alleen uitgenodigde personen hebben toegang**.

   Als u van gedachten verandert, kunt u selecteren **Iedereen in het systeem kan bekijken**.

   >[!NOTE]
   >
   >* Wanneer u een aangepast formulier systeembreed zichtbaar maakt, staat u gebruikers toe het formulier alleen te bekijken en in te vullen op objecten waaraan ze zijn toegewezen, en niet het aan andere objecten te koppelen. U kunt de mogelijkheid bieden om het aangepaste formulier aan objecten te koppelen met de optie &quot;Bijvoegen aan aangepaste gegevens&quot; die in stap 6 wordt beschreven.
   >* De meeste organisaties willen ervoor zorgen dat iedereen in het systeem een douaneformulier kan invullen wanneer het aan voorwerpen wordt vastgemaakt zij werken en zijn gegevens in rapporten bekijken. Als dit voor uw organisatie waar is, adviseren wij dat u gebruikt **Iedereen in het systeem kan bekijken**. Wanneer de optie deze manier wordt gevormd, &quot;Zichtbare systeem-brede&quot;vertoningen in de dialoogdoos:
   >   
   >![Aangepast formulier delen](assets/share-custom-form-in-designer.png)
   >   
   >Als u zich zorgen maakt over een aangepast formulier waarin gebruikers vertrouwelijke gegevens kunnen invoeren wanneer deze aan bepaalde objecten zijn gekoppeld, beperkt u het delen voor deze objecten *objecten* Het zou beter kunnen zijn dan de toegang tot het formulier zelf te beperken.

1. Klikken **Opslaan**.

## Toegang tot een aangepast formulier verwijderen uit de lijst met formulieren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Selecteer het aangepaste formulier en klik op ![Pictogram Delen](assets/share-icon.png).
1. Klik in het vak dat wordt weergegeven op de X rechts van de naam van de gebruiker, het team, de rol, de groep of het bedrijf waartoe u geen speciale toegang meer wilt hebben.
1. (Optioneel) Herhaal de vorige stap naar voor andere namen die u wilt verwijderen.
1. Klikken **Opslaan**.
