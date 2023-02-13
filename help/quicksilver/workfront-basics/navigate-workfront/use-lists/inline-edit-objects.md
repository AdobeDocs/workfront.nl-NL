---
product-area: projects
navigation-topic: use-lists
title: Items inline bewerken in een lijst in [!DNL Adobe Workfront]
description: U kunt objecten inline bewerken wanneer ze in een lijst of rapport worden weergegeven. Wanneer u de informatie over objecten bewerkt die in een lijst of rapport worden weergegeven, wordt het object direct bijgewerkt.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---

# Items inline bewerken in een lijst in [!DNL Adobe Workfront]

U kunt objecten inline bewerken wanneer ze in een lijst of rapport worden weergegeven. Wanneer u de informatie over objecten bewerkt die in een lijst of rapport worden weergegeven, wordt het object direct bijgewerkt.

Als u een veld in een aangepast formulier inline bewerkt dat niet aan het object is gekoppeld, wordt het aangepaste formulier automatisch aan het object toegevoegd. Als het veld bestaat op meerdere aangepaste formulieren, wordt het aangepaste formulier dat het laatst is bijgewerkt, aan het object gekoppeld.

Voor meer informatie over lijsten raadpleegt u [Aan de slag met lijsten in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

De meeste objecten in lijsten of rapporten kunnen inline worden bewerkt in [!DNL Adobe Workfront], zijn er enkele beperkingen, waaronder:

* U kunt berekende velden niet bewerken of [!DNL Workfront] ingebouwde velden die berekeningen zijn.
* U kunt alleen velden bewerken die rechtstreeks aan de objecten in de lijst zijn gekoppeld. U kunt geen velden bewerken die behoren tot objecten die zijn gekoppeld aan de objecten in de lijst.\
   Bijvoorbeeld, kunt u de status van een taak in een rapport van de Taak uitgeven, maar u kunt niet de naam van het project uitgeven de taak met in het zelfde rapport wordt geassocieerd. U kunt de naam van het project slechts in een rapport van het Project uitgeven.
* U kunt velden niet inline bewerken wanneer de standaardvaluta niet wordt weergegeven in de weergave voor een lijst.\
   Zie de sectie voor informatie over het weergeven van de standaardvaluta [Rapporten bewerken met unieke valuta&#39;s](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) in het artikel [Rapporten met financiële gegevens maken met unieke wisselkoersen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* U kunt markeringen en pictogrammen die in een lijst worden weergegeven niet bewerken.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Edit] toegang tot het gebied waarin de lijst zich bevindt</p> <p>Als u bijvoorbeeld taken in een project inline wilt bewerken, hebt u [!UICONTROL Edit] toegang tot projecten.</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen.<br>Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage]</p> <p>U moet ook machtigingen hebben om bepaalde velden te bewerken, zoals aangepaste velden, status, enzovoort.</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Objecten inline bewerken

1. Ga naar een lijst met objecten die u inline wilt bewerken.

   De lijst moet velden weergeven die behoren tot de objecten of velden die horen bij objecten die zijn gekoppeld aan de objecten in de lijst.

1. Zoek het object dat u wilt bewerken en klik vervolgens in een veld in de lijst.

   >[!TIP]
   >
   >Als u meerdere pagina&#39;s hebt, kunt u een object zoeken met:
   >
   >   
   >   
   >   * **Paginering**: Klik op de pijlen naar achteren en naar voren om tussen pagina&#39;s te navigeren.\
      >     Rechtsonder in de lijst bevindt zich het gedeelte [!UICONTROL pagination] blijft ongewijzigd wanneer u door de lijst schuift.
   >   * **Snel filter**: Klik op het filterpictogram of typ Alt+F om het snelle filter te openen en voer vervolgens tekst in om alleen items weer te geven die de ingevoerde tekst bevatten.\
      >     Het snelfilter bevindt zich op de lijstwerkbalk. Zie voor meer informatie [Het snelle filter toepassen op een lijst](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   Als het veld kan worden bewerkt, worden het veld en alle andere velden in de lijst omgezet in bewerkbare cellen.

   ![](assets/nwe-editable-cells-350x131.png)

1. Bewerk de informatie in deze cel en druk vervolgens op [!UICONTROL Enter].

   >[!NOTE]
   >
   >Als een aangepast veld is geconfigureerd voor opmaak, kunt u tekst vet maken, cursief maken of onderstrepen wanneer u het veld inline bewerkt in een bijgewerkte lijst.\
   >Voor informatie over het configureren van opmaak voor een aangepast veld raadpleegt u [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >Voor informatie over bijgewerkte lijsten raadpleegt u de sectie &quot;Het verschil tussen de bijgewerkte en de verouderde lijsten&quot; in het artikel [Aan de slag met lijsten in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Druk [!UICONTROL Tab] om naar de volgende bewerkbare cel te gaan.
1. (Voorwaardelijk) Als u uw bewerkingen niet kunt opslaan en de cel rood wordt weergegeven, klikt u in het veld om het validatiebericht te bekijken dat naast de cel wordt weergegeven en de juiste updates uit te voeren.

   Dit gebeurt meestal wanneer de verkeerde indeling wordt gebruikt of een vereist veld leeg is gelaten.

1. Nadat u alle cellen hebt gewijzigd, drukt u op [!UICONTROL Enter] om uw wijzigingen op te slaan.
