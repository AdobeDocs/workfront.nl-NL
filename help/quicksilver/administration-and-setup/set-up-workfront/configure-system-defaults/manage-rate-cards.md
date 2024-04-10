---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Creditcards beheren
description: Met tariefkaarten kunt u meerdere factureringssnelheden per rol definiëren, op basis van locatie.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: a61635022da9eed7c2fc61bad1cbca0f7f23d7ec
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Creditcards beheren

{{highlighted-preview-article-level}}

Met tariefkaarten kunt u meerdere factureringssnelheden per rol definiëren, op basis van locatie. U zou een baan van Ontwerper kunnen hebben die in Parijs wordt gevestigd en een tweede Ontwerper die in New York wordt gebaseerd, elk met verschillende factureringstarieven. Nochtans, wordt een plaats niet vereist voor baanrollen op een tariefkaart. Een factureringstarief voor een baanrol (en misschien plaats) op een tariefkaart kan efficiënte data ook omvatten.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw plan: [!UICONTROL Standard] </p>
       <p>of</p> 
       <p>Huidig plan: [!UICONTROL Plan] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang bewerken tot [!UICONTROL Financial Data]</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Als u een tariefkaart wilt bewerken die met u wordt gedeeld, moet u beheerdersmachtigingen voor de tariefkaart hebben.</td> 
  </tr> 
 </tbody> 
</table>

## Creditcard toevoegen

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op [!UICONTROL **Snelheidskaarten**].
1. Klikken [!UICONTROL **Nieuwe tariefkaart**] Typ vervolgens een naam voor de tariefkaart in het dialoogvenster [!UICONTROL New rate card] doos, om &quot;Kaart van het Ontiteltarief te vervangen.&quot;
1. (Optioneel) Voeg een [!UICONTROL **Beschrijving**].
1. (Optioneel) Als u een aangepast formulier aan de tariefkaart wilt koppelen, klikt u op de knop [!UICONTROL **Aangepast formulier toevoegen**] in de rechterbovenhoek en selecteer een aangepast formulier in de lijst die wordt weergegeven.

   Zie voor meer informatie over het bijvoegen van een aangepast formulier [Een aangepast formulier toevoegen aan een object](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klikken [!UICONTROL **Functierollen en -tarieven**] in het linkernavigatievenster.
1. Klik op het scherm Taken en sneltoetsen voor kaart beoordelen op [!UICONTROL **Functie toevoegen**].
1. Selecteer een [!UICONTROL **Functie**] om factureringstarieven te bepalen voor.

   Het standaardFactureringstarief toont het systeem-vlakke tarief voor deze baanrol, als wordt bepaald.

   ![Dialoogvenster Nieuwe factureringsfrequentie](assets/location-rate-for-rate-card.png)

1. Selecteer een [!UICONTROL **Valuta**] voor de functie.
1. (Optioneel) Selecteer een [!UICONTROL **Locatie**] voor de functie.
1. In de [!UICONTROL **Factureringsfrequentie 1**] Voer de factureringssnelheid voor deze locatie in. Klik vervolgens op [!UICONTROL **Opslaan**] om de factureringssnelheid één keer te overschrijven.

   of

   Klikken [!UICONTROL **Snelheid toevoegen**] om meer locatie-specifieke factureringstarieven met effectieve data toe te voegen.

1. (Voorwaardelijk) Als u meer dan één factureringstarief voor deze plaats toevoegt, ga de volgende informatie in:

   * **[!UICONTROL Billing Rate 1], 2, enz.:** De waarde van de factureringssnelheid voor de tijdsperiode.
   * **[!UICONTROL Start Date]:** De datum waarop de tariefoverschrijving begint.
   * **[!UICONTROL End Date]:** De datum waarop de rate override eindigt.

     Factureringsgraad 1 zal geen begindatum hebben en het laatste factureringstarief zal geen einddatum hebben. Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als het Facturerings Tarief 1 geen einddatum heeft, en u het Facturerings Tarief 2 met een begindatum van 1 mei 2023 toevoegt, wordt een einddatum van 30 april, 2023 toegevoegd aan het Facturerings Tarief 1 zodat geen hiaten bestaan.

1. Klikken [!UICONTROL **Opslaan**].
1. (Optioneel) Als u nog een factureringsniveau wilt toevoegen, voor dezelfde taakrol op een andere locatie of voor een aparte taakrol, klikt u op [!UICONTROL **Functie toevoegen**].
1. (Optioneel) Als u een tariefkaart wilt bewerken, klikt u op de naam van de tariefkaart in de lijst Sneltoetsen in Setup. Als u een factureringssnelheid wilt bewerken, klikt u op [!UICONTROL **Functierollen en -tarieven**] in het linkernavigatievenster van de tariefkaart. Selecteer vervolgens de snelheid en klik op de knop **Bewerken** pictogram ![Pictogram Bewerken](assets/edit-icon.png).

## Een creditcard kopiëren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op [!UICONTROL **Snelheidskaarten**].
1. Schakel het selectievakje naast de tariefkaart in de lijst in en klik op de knop **Kopiëren** pictogram ![Pictogram kopiëren](assets/copy-icon.png).
1. Typ een naam voor de tariefkaart in het dialoogvenster [!UICONTROL Copy rate card] doos, om &quot;Kaart van het Ontiteltarief te vervangen.&quot; Klik vervolgens op **Opslaan**.

   De nieuwe tariefkaart wordt opgeslagen. Bewerk indien nodig de gegevens van de tariefkaart, de taakrollen en de tarieven.

## Een volledige tariefkaart verwijderen

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op [!UICONTROL **Snelheidskaarten**].
1. Schakel het selectievakje naast de tariefkaart in de lijst in en klik op de knop **Verwijderen** pictogram ![Pictogram Verwijderen](assets/delete.png).

   >[!NOTE]
   >
   >Een aan een project gekoppelde tariefkaart wordt uit het project verwijderd.
