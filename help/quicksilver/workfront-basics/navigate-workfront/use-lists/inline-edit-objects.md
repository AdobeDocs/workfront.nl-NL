---
product-area: projects
navigation-topic: use-lists
title: Items inline bewerken in een lijst in  [!DNL Adobe Workfront]
description: U kunt objecten inline bewerken wanneer ze in een lijst of rapport worden weergegeven. Wanneer u de informatie over objecten bewerkt die in een lijst of rapport worden weergegeven, wordt het object direct bijgewerkt.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: f0912e4ef29d682ae3e6dd0e543b8e77fb7f29b6
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Items inline bewerken in een lijst in [!DNL Adobe Workfront]

U kunt objecten inline bewerken wanneer ze in een lijst of rapport worden weergegeven. Wanneer u de informatie over objecten bewerkt die in een lijst of rapport worden weergegeven, wordt het object direct bijgewerkt.

Als u een veld in een aangepast formulier inline bewerkt dat niet aan het object is gekoppeld, wordt het aangepaste formulier automatisch aan het object toegevoegd. Als het veld bestaat op meerdere aangepaste formulieren, wordt het aangepaste formulier dat het laatst is bijgewerkt, aan het object gekoppeld.

Voor meer informatie over lijsten, zie [ begonnen worden met lijsten in  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

De meeste objecten die in lijsten of rapporten worden weergegeven, kunnen inline worden bewerkt in [!DNL Adobe Workfront] , maar er zijn enkele beperkingen, waaronder:

* U kunt berekende velden of [!DNL Workfront] ingebouwde velden die berekeningen zijn, niet bewerken.
* U kunt alleen velden bewerken die rechtstreeks aan de objecten in de lijst zijn gekoppeld. U kunt geen velden bewerken die behoren tot objecten die zijn gekoppeld aan de objecten in de lijst.\
   Bijvoorbeeld, kunt u de status van een taak in een rapport van de Taak uitgeven, maar u kunt niet de naam van het project uitgeven de taak met in het zelfde rapport wordt geassocieerd. U kunt de naam van het project slechts in een rapport van het Project uitgeven.
* U kunt velden niet inline bewerken wanneer de standaardvaluta niet wordt weergegeven in de weergave voor een lijst.\
   Voor informatie bij het tonen van de standaardmunt, zie de sectie [ rapporten met unieke valuta ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) in het artikel [ uitgeven financiële gegevensrapporten met unieke wisselkoersen ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* U kunt markeringen en pictogrammen die in een lijst worden weergegeven niet bewerken.
* U kunt rapportvelden die afkomstig zijn uit andere rapporten niet inline bewerken.

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
   <td> <p>[!UICONTROL Edit] toegang tot het gebied in de lijst</p> <p>Als u bijvoorbeeld inline bewerkingstaken in een project wilt uitvoeren, hebt u [!UICONTROL Edit] toegang tot projecten nodig.</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld.<br> voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage]</p> <p>U moet ook machtigingen hebben om bepaalde velden te bewerken, zoals aangepaste velden, status, enzovoort.</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

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
   >   * **Paginering**: Klik achteruit en door:sturen pijlen om tussen pagina&#39;s te navigeren.\
   >     Het gebied [!UICONTROL pagination] bevindt zich in de rechterbenedenhoek van de lijst en blijft ongewijzigd wanneer u door de lijst schuift.
   >   * **Snelle filter**: Klik het filterpictogram of type Alt+F om de snelle filter te openen, dan tekst in te gaan om slechts punten te tonen die de ingegane tekst bevatten.\
   >     Het snelfilter bevindt zich op de lijstwerkbalk. Voor meer informatie, zie [ de snelle filter op een lijst ](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md) toepassen.


   Als het veld kan worden bewerkt, worden het veld en alle andere velden in de lijst omgezet in bewerkbare cellen.

   ![](assets/nwe-editable-cells-350x131.png)

1. Bewerk de informatie in deze cel en druk op [!UICONTROL Enter] .

   >[!NOTE]
   >
   >Als een aangepast veld is geconfigureerd voor opmaak, kunt u tekst vet maken, cursief maken of onderstrepen wanneer u het veld inline bewerkt in een bijgewerkte lijst.\
   >Voor informatie bij het vormen van het formatteren voor een douanegebied, zie [ een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) creëren of uitgeven.\
   >Voor informatie over bijgewerkte lijsten, zie de sectie &quot;het verschil tussen de bijgewerkte en erfenislijsten&quot;in artikel [ worden begonnen met lijsten in  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Druk op [!UICONTROL Tab] om naar de volgende bewerkbare cel te gaan.
1. (Voorwaardelijk) Als u uw bewerkingen niet kunt opslaan en de cel rood wordt weergegeven, klikt u in het veld om het validatiebericht te bekijken dat naast de cel wordt weergegeven en de juiste updates uit te voeren.

   Dit gebeurt meestal wanneer de verkeerde indeling wordt gebruikt of een vereist veld leeg is gelaten.

1. Nadat u alle cellen hebt gewijzigd, drukt u op [!UICONTROL Enter] om de wijzigingen op te slaan.
