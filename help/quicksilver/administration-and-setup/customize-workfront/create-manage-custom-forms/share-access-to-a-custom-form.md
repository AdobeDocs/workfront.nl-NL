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
source-git-commit: a7be72f0a594a21baed2592d8a2e467118ab1b7f
workflow-type: tm+mt
source-wordcount: '1531'
ht-degree: 0%

---

# Een aangepast formulier delen

U kunt toegang voor een douaneformulier vormen om te controleren wie-persoon, rol, groep, team, bedrijf-kan bekijken, delen, en het uitgeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Toegang tot aangepaste formulieren {#access-to-custom-forms}

Wanneer u een nieuw aangepast formulier maakt en iemand dit aan een object koppelt, kan elke gebruiker die aan het object is toegewezen het formulier weergeven en invullen. Dit geldt ook voor gebruikers met aanvraaglicenties en externe gebruikers.

Op een object waaraan het aangepaste formulier nog niet is gekoppeld, kan een gebruiker het echter niet koppelen via het vervolgkeuzemenu Aangepaste Forms, zelfs niet bij een Planner-toegangsniveau:

* Iemand heeft het aangepaste formulier gedeeld met de gebruiker of met het team, de rol, de groep of het bedrijf van de gebruiker en geeft minimaal toestemming voor Weergave met de optie Bijvoegen bij aangepaste gegevens geselecteerd
* De gebruiker heeft een vergunning van het Plan en hun toegangsniveau verleent administratieve toegang tot douaneformulieren

## Een aangepast formulier delen vanuit de lijst met formulieren

Eerder dan het verlaten van een douanevorm in het gebrek delend staat (die in [&#x200B; Toegang tot douanevormen &#x200B;](#access-to-custom-forms) in dit artikel wordt beschreven), kunt u specifieke niveaus van toegang tot de vorm voor bepaalde gebruikers, baanrollen, groepen, teams, en bedrijven vormen.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Selecteer de douanevorm, dan klik het ![&#x200B; pictogram van het Aandeel &#x200B;](assets/share-icon.png).
1. In de doos die toont, onder **geef de toegang van de douanevorm tot**, begin de naam van de gebruiker, het team, de baanrol, de groep, of het bedrijf u de douanevorm met wilt delen, dan **binnengaan** wanneer de naamvertoningen.
1. Als u de toegang wilt aanpassen voor de gebruiker, het team, de taakrol, de groep of het bedrijf dat u net hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en configureert u vervolgens een van de volgende beschikbare opties en een van de geavanceerde instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>Met deze optie kunt u het aangepaste formulier weergeven en invullen op objecten. Op het objecten niveau, moeten de gebruikers minstens Contribute toegang met <strong> hebben uitgeeft de geavanceerd plaatsen van de douanevorm </strong>. Als het formulier bijvoorbeeld is gekoppeld aan een project, moeten gebruikers Contribute-toegang hebben tot dat project, anders kunnen ze het formulier niet invullen.</p>

   <p><b> NOTA </b>: Voor gebruikers met Lichte en Medewerker vergunningen (of het Werk, het Overzicht, en de vergunningen van het Verzoek), is dit de hoogste beschikbare optie.</p>

   <p>Klik <strong> Geavanceerde Montages </strong> om te specificeren of u het volgende wilt toestaan:</p> 
       <ul> 
        <li><strong> Band aan douanegegevens </strong>: Mogelijkheid om de douanevorm aan projecten, taken, en kwesties vast te maken waarvoor zij hebben leiden toegang</li> 
        <li> <p><strong> Aandeel </strong>: Mogelijkheid om de douanevorm met anderen in het systeem te delen</p> <p>Gebruikers met een licentie voor licht of contribuant (of een licentie voor werken, revisie of aanvragen) kunnen een aangepast formulier alleen delen via de API of een aangepast formulierrapport.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Deze optie is alleen beschikbaar voor gebruikers met een Standard- of Plan-licentie. </p> <p>Gebruikers kunnen het formulier niet alleen toevoegen aan objecten die ze kunnen bewerken, maar kunnen ook het aangepaste formulier volledig bewerken, zoals velden toevoegen, bewerken en verwijderen.</p> <p>Klik <strong> Geavanceerde Montages </strong> om te specificeren of u het volgende wilt toestaan:</p> 
       <ul> 
        <li> <p><strong> Band aan douanegegevens </strong>: Mogelijkheid om de douanevorm aan projecten, taken, en kwesties vast te maken waarvoor zij hebben leiden toegang</p> </li> 
        <li><strong> Schrapping </strong>: Schrap de douanevorm van het systeem</li> 
        <li><strong> Aandeel </strong>: Deel de douanevorm met anderen in het systeem</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal stap 4-5 om andere namen aan de lijst toe te voegen en de opties te configureren.
1. (Facultatief) als u toegang tot de douanevorm (op voorwerpen wilt beperken waar het) aan die u in de vorige stappen hebt gespecificeerd, klik het tandwielpictogram ![](assets/gear-icon-settings-with-dn-arrow.jpg) in de hogere juiste hoek van de het delen doos, dan klik **verwijderen systeem-brede toegang**.

   Als u uw mening verandert, kunt u **klikken maakt dit zichtbare systeem-breed** (de standaardoptie).

   >[!NOTE]
   >
   >* Wanneer u een aangepast formulier systeembreed zichtbaar maakt, staat u gebruikers toe het formulier alleen te bekijken en in te vullen op objecten waaraan ze zijn toegewezen, en niet het aan andere objecten te koppelen. U kunt de mogelijkheid bieden om het aangepaste formulier aan objecten te koppelen met de optie &quot;Bijvoegen aan aangepaste gegevens&quot; die in stap 5 wordt beschreven.
   >* De meeste organisaties willen ervoor zorgen dat iedereen in het systeem een douaneformulier kan invullen wanneer het aan voorwerpen wordt vastgemaakt zij werken en zijn gegevens in rapporten bekijken. Als dit voor uw organisatie waar is, adviseren wij dat u **dit zichtbare systeem-breed** maakt. Wanneer de optie deze manier wordt gevormd, &quot;Zichtbare systeem-brede&quot;vertoningen in de dialoogdoos:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Als u zich over een douaneformulier bezorgd bent waar de gebruikers gevoelige gegevens zouden kunnen ingaan wanneer het aan bepaalde voorwerpen in bijlage is, zou het beperken van het delen voor die *voorwerpen* beter kunnen zijn eerder dan het beperken van toegang tot de vorm zelf.

1. Klik **sparen**.

## Een aangepast formulier delen vanuit de formulierontwerper

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Open een aangepast formulier of maak een nieuw aangepast formulier.
1. Klik **Aandeel** op het hoogste recht van de vormontwerper wanneer u bereid bent om de vorm te delen.
1. In de doos die toont, onder **de toegang van de douanevorm van de Verlening tot**, begint de naam van de gebruiker, het team, de baanrol, de groep, of het bedrijf te typen u de douanevorm met wilt delen, dan **binnengaan** wanneer de naamvertoningen.
1. Als u de toegang wilt aanpassen voor de gebruiker, het team, de taakrol, de groep of het bedrijf dat u net hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en configureert u vervolgens een van de volgende beschikbare opties en een van de geavanceerde instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>Met deze optie kunt u het aangepaste formulier weergeven en invullen op objecten. Op het objecten niveau, moeten de gebruikers minstens Contribute toegang met <strong> hebben uitgeeft de geavanceerd plaatsen van de douanevorm </strong>. Als het formulier bijvoorbeeld is gekoppeld aan een project, moeten gebruikers Contribute-toegang hebben tot dat project, anders kunnen ze het formulier niet invullen.</p>

   <p><b> NOTA </b>: Voor gebruikers met Lichte en Medewerker vergunningen (of het Werk, het Overzicht, en de vergunningen van het Verzoek), is dit de hoogste beschikbare optie.</p> <p>Klik <strong> Geavanceerde Montages </strong> om te specificeren of u het volgende wilt toestaan:</p> 
       <ul> 
        <li><strong> Band aan douanegegevens </strong>: Mogelijkheid om de douanevorm aan projecten, taken, en kwesties vast te maken waarvoor zij hebben leiden toegang</li> 
        <li> <p><strong> Aandeel </strong>: Mogelijkheid om de douanevorm met anderen in het systeem te delen</p> <p>Gebruikers met een licentie voor licht of contribuant (of een licentie voor werken, revisie of aanvragen) kunnen een aangepast formulier alleen delen via de API of een aangepast formulierrapport.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>Deze optie is alleen beschikbaar voor gebruikers met een Standard- of Plan-licentie. </p> <p>Gebruikers kunnen het formulier niet alleen toevoegen aan objecten die ze kunnen bewerken, maar kunnen ook het aangepaste formulier volledig bewerken, zoals velden toevoegen, bewerken en verwijderen.</p> <p>Klik <strong> Geavanceerde Montages </strong> om te specificeren of u het volgende wilt toestaan:</p> 
       <ul> 
        <li> <p><strong> Band aan douanegegevens </strong>: Mogelijkheid om de douanevorm aan projecten, taken, en kwesties vast te maken waarvoor zij hebben leiden toegang</p> </li> 
        <li><strong> Schrapping </strong>: Schrap de douanevorm van het systeem</li> 
        <li><strong> Aandeel </strong>: Deel de douanevorm met anderen in het systeem</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal stap 5-6 om andere namen aan de lijst toe te voegen en hun opties te configureren.
1. (Facultatief) als u toegang tot de douanevorm (op voorwerpen wilt beperken waar het) aan die u in de vorige stappen hebt gespecificeerd, klik de drop-down pijl onder **die toegang** heeft, dan selecteren **slechts uitgenodigde mensen kunnen toegang hebben**.

   Als u uw mening verandert, kunt u **iedereen in het systeem selecteren kan** bekijken.

   >[!NOTE]
   >
   >* Wanneer u een aangepast formulier systeembreed zichtbaar maakt, staat u gebruikers toe het formulier alleen te bekijken en in te vullen op objecten waaraan ze zijn toegewezen, en niet het aan andere objecten te koppelen. U kunt de mogelijkheid bieden om het aangepaste formulier aan objecten te koppelen met de optie &quot;Bijvoegen aan aangepaste gegevens&quot; die in stap 6 wordt beschreven.
   >* De meeste organisaties willen ervoor zorgen dat iedereen in het systeem een douaneformulier kan invullen wanneer het aan voorwerpen wordt vastgemaakt zij werken en zijn gegevens in rapporten bekijken. Als dit voor uw organisatie waar is, adviseren wij dat u **iedereen in het systeem** kunt bekijken. Wanneer de optie deze manier wordt gevormd, &quot;Zichtbare systeem-brede&quot;vertoningen in de dialoogdoos:
   >   
   >![&#x200B; Aangepaste vorm van het Aandeel &#x200B;](assets/share-custom-form-in-designer.png)
   >   
   >Als u zich over een douaneformulier bezorgd bent waar de gebruikers gevoelige gegevens zouden kunnen ingaan wanneer het aan bepaalde voorwerpen in bijlage is, zou het beperken van het delen voor die *voorwerpen* beter kunnen zijn eerder dan het beperken van toegang tot de vorm zelf.

1. Klik **sparen**.

## Toegang tot een aangepast formulier verwijderen uit de lijst met formulieren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Selecteer de douanevorm, dan klik het ![&#x200B; pictogram van het Aandeel &#x200B;](assets/share-icon.png).
1. Klik in het vak dat wordt weergegeven op de X rechts van de naam van de gebruiker, het team, de rol, de groep of het bedrijf waartoe u geen speciale toegang meer wilt hebben.
1. (Optioneel) Herhaal de vorige stap naar voor andere namen die u wilt verwijderen.
1. Klik **sparen**.
