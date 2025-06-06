---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Creeer een  [!DNL Adobe Workfront]  verzoek van een e-mail van Vooruitzichten
description: U kunt a  [!DNL Adobe Workfront]  verzoek van een e-mail in Vooruitzichten tot stand brengen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Een [!DNL Adobe Workfront] -aanvraag maken op basis van een [!UICONTROL Outlook] -e-mail

>[!IMPORTANT]
>
>[ Microsoft is in het proces om steun voor de online tokens van de erfenisUitwisseling ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar te maken, die momenteel door de toe:voegen-binnen van Workfront Vooruitzichten voor authentificatie worden gebruikt. Deze verandering door Microsoft is al begonnen met gevolgen voor de klanten en zal tot oktober 2025 in fasen blijven doorlopen.
>
>* **nadat Microsoft volledig deze tokens onbruikbaar maakt, zal Workfront voor de integratie van Microsoft Outlook niet meer functioneren.**
>
>Als onderdeel van deze wijziging heeft Microsoft besloten om de manier te wijzigen waarop tokens opnieuw worden ingeschakeld. Na **Juni 30, 2025**, zullen de beheerders niet meer tokens kunnen re-toelaten zelf-slechts de Steun van Microsoft kan uitzonderingen verlenen. **Op 1 Oktober, 2025, zullen de erfenistokens voor alle huurders worden uitgezet. Er worden geen uitzonderingen toegestaan.**

U kunt een [!DNL Adobe Workfront] -aanvraag maken op basis van een e-mailbericht in Outlook.

Wanneer u een [!DNL Workfront] -aanvraag maakt op basis van een e-mail, wordt de inhoud van de e-mail (inclusief het onderwerp en de tekst) standaard in de aanvraag opgenomen.

>[!NOTE]
>
>U kunt geen [!DNL Workfront] verzoek van een gedeelde [!UICONTROL Outlook] brievenbus tot stand brengen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

Uw [!DNL Workfront] beheerder moet [!DNL Outlook for Office] with [!DNL Workfront] inschakelen voordat u deze integratie kunt gebruiken.

## Een aanvraag maken op basis van een [!DNL Outlook]-e-mail

Een [!DNL Workfront] aanvraag maken van [!DNL Outlook] :

1. Selecteer het e-mailbericht dat de gegevens bevat die u wilt opnemen in een [!DNL Workfront] -aanvraag.
1. Klik op het pictogram **[!DNL Workfront]** rechtsboven in het e-mailbericht om de invoegtoepassing Workfront weer te geven.\
   Mogelijk moet u op de pijl omlaag in de rechterbovenhoek van uw e-mail klikken om het pictogram [!DNL Workfront] te openen.

1. Klik het **[!UICONTROL Menu]** pictogram ![ o365_addin_menu2_icon.png ](assets/o365-addin-menu2-icon.png) om de lijst van beschikbare [!DNL Workfront] opties te tonen.

1. Klik op **[!UICONTROL Submit Request]**.
1. Selecteer in het veld **[!UICONTROL Select a Request Type]** de aanvraagwachtrij waar u de aanvraag wilt verzenden.

1. Geef de volgende informatie op:\
   Afhankelijk van hoe de aanvraagwachtrij is ingesteld, kunnen de beschikbare velden variëren. Voor een volledige lijst en een beschrijving van mogelijke gebieden, zie [  [!DNL Adobe Workfront]  verzoeken ](../../manage-work/requests/create-requests/create-submit-requests.md) artikel creëren en voorleggen.

   * **[!UICONTROL Subject]:** specificeer een onderwerp voor het verzoek. Standaard wordt het onderwerp van de e-mail gebruikt.
   * **[!UICONTROL Description]:** specificeer een beschrijving voor het verzoek. Standaard wordt de e-mailhoofdtekst gebruikt.
   * **[!UICONTROL Documents]:** voeg om het even welke documenten bij die u in het verzoek wilt omvatten. U kunt documenten bijvoegen door te slepen en neer te zetten of door te klikken op **[!UICONTROL Select File]** en naar het document te bladeren en het te selecteren.\

     Alle documenten die bij de e-mail horen, worden standaard in de aanvraag opgenomen.

1. Klik op **[!UICONTROL Submit Request]**.\
   Het verzoek wordt verzonden naar [!DNL Workfront], in de opgegeven aanvraagwachtrij.

1. (Optioneel) Navigeer terug naar [!DNL Outlook] en selecteer het oorspronkelijke e-mailadres.\
   Boven aan het venster voor de [!DNL Workfront] invoegtoepassing ziet u de bevestiging met een koppeling dat het e-mailbericht als een aanvraag aan Workfront is toegevoegd. De koppeling bevat de datum waarop deze is geconverteerd.\
