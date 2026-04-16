---
title: Toegang tot financiële gegevens in aangepaste velden beperken
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wanneer u een aangepast veld maakt, kunt u optionele instellingen definiëren om de toegang tot financiële gegevens te beperken.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3380cce6-8372-43c0-8520-473442ea0eb4
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Toegang tot financiële gegevens in aangepaste velden beperken

Wanneer u een aangepast veld maakt, kunt u optionele instellingen definiëren om de toegang tot financiële gegevens te beperken. Op deze manier kunnen gebruikers die bepaalde machtigingen hebben ingesteld in hun toegangsniveaus de gegevens zien en kunnen ze geen financiële gegevens zien waartoe ze geen toegang zouden moeten hebben.

Voor informatie over het creëren van een douanegebied, zie [ een douanevorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

Voor informatie over toegangsniveaus, zie [ overzicht van de Niveaus van de Toegang ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md). Voor informatie over het delen en toestemmingen, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr>  
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Administratieve toegang tot aangepaste formulieren</td> 
  </tr>  
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Toegang tot financiële gegevens op een aangepast veld beperken

1. Maak een nieuw aangepast formulier of open een bestaand formulier.

   Voor informatie, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. Voeg een aangepast veld toe aan het formulier of selecteer een bestaand veld.

   Deze veldtypen kunnen worden beperkt op basis van de toegang tot financiële gegevens:

   * Tekst met één regel
   * Alinea
   * Vervolgkeuzelijst met één keuze
   * Vervolgkeuzelijst met meerdere selecties
   * Groep selectievakjes
   * Keuzerondjes
   * Externe zoekopdracht
   * Externe zoekopdracht met meerdere selecties
   * Berekend

1. Op het **gebied van het Formaat**, uitgezochte **Valuta**.

   >[!NOTE]
   >
   >Voor berekende velden is elke indeling toegestaan. Alle andere gebiedstypes moeten het **formaat van de Valuta** gebruiken, of het **toestemmingstype van de Financiën** gebied zal niet beschikbaar zijn.

1. (Facultatief) voor berekende gebieden slechts, zet de **Automatische toestemmings** optie aan om de financiële toestemmingen toe te staan om automatisch uit de gebieden in de formule te komen.

1. Selecteer een optie voor het **toestemmingstype van de Financiën**.

   Gebruikers moeten beschikken over dit type financiële machtigingen voordat ze dit aangepaste veld op het formulier kunnen weergeven of bewerken.

   * **Geen vereiste toestemmingen:** Alle gebruikers kunnen dit gebied zien
   * **Algemeen:** de gebruikers moeten toestemmingen hebben om Algemene Financiën uit te geven of te bekijken
   * **Rekening:** de gebruikers moeten toestemmingen hebben om het factureren tarieven uit te geven of te bekijken
   * **Kosten:** de gebruikers moeten toestemmingen hebben om kostentarieven uit te geven of te bekijken

   Voor berekende velden:

   * Het **toestemmingstype van de Financiën** gebied is niet beschikbaar voor het manueel plaatsen van toestemmingen als het **Automatische toestemmings** gebied wordt aangezet.
   * De velden die in de formule worden gebruikt, bepalen of het veld voor machtigingen actief is. Als het machtigingsveld leeg is (en automatische machtigingen niet zijn ingeschakeld), ondersteunen de velden in de formule de financiële machtigingen niet.
   * Toegang is vereist voor alle velden in de formule. Bijvoorbeeld, als twee gebieden op een berekend gebied worden gebruikt, en één van hen toegepaste het factureren toestemmingen heeft en de tweede toegepaste kostentoestemming heeft, dan moet de gebruiker toestemmingen hebben om zowel het factureren als kostentarieven te bekijken om de berekende waarde te zien.

1. Om uw veranderingen te bewaren, klik **van toepassing zijn** en blijven bouwend uw vorm.

   of

   Klik **sparen en Sluiten**.

## Voorbeeld

Twee projecten worden gedeeld met een gebruiker:

* De gebruiker heeft toestemmingen om alle financieringsopties op het eerste project uit te geven
* De gebruiker heeft toestemmingen om factureringstarieven en algemene financiering op het tweede project te bekijken

Wanneer de gebruiker het eerste project bewerkt, zijn alle financiële velden in het aangepaste formulier bewerkbaar. Wanneer de gebruiker het tweede project uitgeeft, zijn de gebieden die aan **worden geplaatst Rekening** of **Algemeen** mening-slechts, en de gebieden die aan **worden geplaatst Kosten** niet zichtbaar.

Wanneer de gebruiker de projecten in een lijst of een rapport bekijkt:

* De financiële gebieden zijn viewable of editable volgens de toestemmingen en de rapportmontages
* Financiële velden zijn leeg als de gebruiker geen machtigingen heeft om deze te bekijken

Bij het exporteren van projectdetails worden dezelfde waarden voor financiële velden (of lege velden) weergegeven als in de lijst.

Wanneer het bulkuitgeven van beide projecten, tonen de facturerings en algemene financieringsgebieden als read-only, en de kostengebieden tonen n.a.
