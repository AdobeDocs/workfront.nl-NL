---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Rate Cards beheren
description: Met tariefkaarten kunt u meerdere factureringssnelheden per rol definiëren, op basis van locatie.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Creditcards beheren

{{highlighted-preview-article-level}}

Met tariefkaarten kunt u meerdere factureringssnelheden per rol definiëren, op basis van locatie. Je zou een baan kunnen hebben in Designer in Parijs en een tweede Designer in New York, elk met verschillende factureringssnelheden. Nochtans, wordt een plaats niet vereist voor baanrollen op een tariefkaart. Een factureringstarief voor een baanrol (en misschien plaats) op een tariefkaart kan efficiënte data ook omvatten.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td><p>Nieuw abonnement: [!UICONTROL Standard] </p>
       <p>of</p> 
       <p>Huidig abonnement: [!UICONTROL Plan] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang bewerken tot [!UICONTROL Financial Data]</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Als u een tariefkaart wilt bewerken die met u wordt gedeeld, moet u beheerdersmachtigingen voor de tariefkaart hebben.</td> 
  </tr> 
 </tbody> 
</table>

+++

## Creditcard toevoegen

{{step-1-to-setup}}

1. In het linkerpaneel, klik [!UICONTROL **kaarten van het Tarief**].
1. Klik [!UICONTROL **Nieuwe tariefkaart**], dan typ een naam voor de tariefkaart in het [!UICONTROL New rate card] vakje, om &quot;Kaart van het Ontiteltarief te vervangen.&quot;
1. (Facultatief) op het scherm van de Details van de Kaart van het Tarief, voeg a [!UICONTROL **Beschrijving**] toe.
1. (Facultatief) om een douaneformulier aan de tariefkaart vast te maken, klik [!UICONTROL **voeg douanevorm**] gebied in de hoger-juiste hoek toe en selecteer een douanevorm van de lijst die toont.

   Voor meer informatie bij het vastmaken van een douanevorm, zie [ een douanevorm aan een voorwerp ](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

1. Klik [!UICONTROL **Rollen en Tarieven van de Baan**] in het linkernavigatievenster.
1. Voor de Rollen en het scherm van de Baan van de Kaart van het Tarief, klik [!UICONTROL **baanrol**] toevoegen.
1. In de dialoog, selecteer de Rol van de a [!UICONTROL **Baan**] om het factureren tarieven voor te bepalen.

   Het standaardFactureringstarief toont het systeem-vlakke tarief voor deze baanrol, als wordt bepaald.

   ![ Nieuwe de dialoog van het Tarief van het Facturerings ](assets/location-rate-for-rate-card.png)

1. Selecteer a [!UICONTROL **Valuta**] voor de baanrol.
1. (Facultatief) selecteer a [!UICONTROL **Plaats**] voor de baanrol.
1. Op het [!UICONTROL **FactureringsTarief 1**] gebied, ga het factureringstarief voor deze plaats in. Dan, klik [!UICONTROL **sparen**] om het het factureren tarief één keer met voeten te treden.

   of

   Klik [!UICONTROL **toevoegen Tarief**] om meer plaats-specifieke het factureren tarieven met efficiënte data toe te voegen.

1. (Voorwaardelijk) Als u meer dan één factureringstarief voor deze plaats toevoegt, ga de volgende informatie in:

   * **[!UICONTROL Billing Rate 1], 2, enzovoort.:** De waarde van het factureringstarief voor de tijdspanne.
   * **[!UICONTROL Start Date]:** De datum waarop de tariefoverschrijving begint.
   * **[!UICONTROL End Date]:** De datum waarop de tariefoverschrijving eindigt.

     Factureringsgraad 1 zal geen begindatum hebben en het laatste factureringstarief zal geen einddatum hebben. Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als het Facturerings Tarief 1 geen einddatum heeft, en u het Facturerings Tarief 2 met een begindatum van 1 mei 2023 toevoegt, wordt een einddatum van 30 april, 2023 toegevoegd aan het Facturerings Tarief 1 zodat geen hiaten bestaan.

1. Klik [!UICONTROL **sparen**].
1. (Facultatief) om een ander het facturerings tarief toe te voegen, of voor de zelfde baanrol in een andere plaats of voor een afzonderlijke baanrol, klik [!UICONTROL **toevoegt baanrol**].
1. (Optioneel) Als u een tariefkaart wilt bewerken, klikt u op de naam van de tariefkaart in de lijst Sneltoetsen in Setup. Om een het factureren tarief uit te geven, klik [!UICONTROL **Rollen en Tarieven van de Baan**] in het linkernavigatievenster van de tariefkaart. Dan, selecteer het tarief en klik **uitgeven** pictogram ![ pictogram ](assets/edit-icon.png) uitgeeft.

## Een creditcard kopiëren

{{step-1-to-setup}}

1. In het linkerpaneel, klik [!UICONTROL **kaarten van het Tarief**].
1. Selecteer de controledoos naast de tariefkaart in de lijst en klik het **pictogram van het Exemplaar ![ pictogram van het Exemplaar ](assets/copy-icon.png).**
1. Typ een naam voor de tariefkaart in het vak [!UICONTROL Copy rate card] om &quot;Kaart zonder titel&quot; te vervangen. Dan, klik **sparen**.

   De nieuwe tariefkaart wordt opgeslagen. Bewerk indien nodig de gegevens van de tariefkaart, de taakrollen en de tarieven.

## Een volledige tariefkaart verwijderen

{{step-1-to-setup}}

1. In het linkerpaneel, klik [!UICONTROL **kaarten van het Tarief**].
1. Selecteer de controledoos naast de tariefkaart in de lijst, en klik het **pictogram van de Schrapping** ![ pictogram van de Schrapping ](assets/delete.png).

   >[!NOTE]
   >
   >Een aan een project gekoppelde tariefkaart wordt uit het project verwijderd.
