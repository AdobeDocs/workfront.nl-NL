---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: De integratie met JumpSeat configureren
description: U kunt  [!DNL JumpSeat]  met  [!DNL Workfront]  integreren om douane, in-productbegeleiding tot stand te brengen.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# De integratie met JumpSeat configureren

U kunt [!DNL JumpSeat] integreren met [!DNL Workfront] om aangepaste, in-product begeleiding te maken.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Product</strong></td> 
   <td>U moet een actief [!DNL JumpSeat] plan hebben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p> U moet een [!DNL Workfront] beheerder zijn. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u begint, moet u

* Voeg [!DNL Workfront] toe en activeer dit als een toepassing in [!DNL JumpSeat] . Voor meer informatie, zie [ hoe te om een toepassing ](https://support.jumpseat.io/article/how-to-add-an-application/) toe te voegen of te schrappen.

## De integratie met [!DNL JumpSeat] configureren

We raden u aan een [!DNL JumpSeat] -integratie in te stellen in zowel uw voorvertoning- als productieomgeving.

>[!TIP]
>
>U moet twee aparte [!DNL Workfront] -toepassingen toevoegen en activeren in [!DNL JumpSeat] : een voor Voorvertoning en een voor Productie. Zie [ hoe te om een toepassing ](https://support.jumpseat.io/article/how-to-add-an-application/) voor meer informatie toe te voegen of te schrappen.

U configureert de integratie met [!DNL JumpSeat] als volgt:

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** .
1. Klik in het linkerdeelvenster op **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat] Integration]** .
1. Voer de **[!UICONTROL [!DNL JumpSeat] URL]** in die u vindt op het extensiepictogram in [!DNL JumpSeat] .

   **Voorbeeld:** [!DNL https]://{mycompanyname} .spronseats.io

1. Voer de **[!UICONTROL [!DNL JumpSeat] integration token]** in. U vindt dit op de pagina **[!UICONTROL Configuration]** in [!DNL JumpSeat] .

   **Voorbeeld:** $2y$10$BevsKeQ8...OYR.LurSg2U64O

1. Klik op **[!UICONTROL Test configuration]**.
1. Kies of de integratie **[!UICONTROL Active]** of **[!UICONTROL Inactive]** moet zijn.

   >[!IMPORTANT]
   >
   >De in stap 5 uitgevoerde configuratietest moet slagen om de integratie te activeren.

   ![ JumpSeat de pagina van de Integratie ](assets/jumpseat-integration-page.png)

1. Klik op **[!UICONTROL Save]**.

>[!TIP]
>
>Voor meer informatie over het vormen van uw [!DNL JumpSeat] integratie, zie de [!DNL JumpSeat] documentatie voor [ JumpSeat+Workfront ](https://jumpseat.io/landing-page/jumpseat-workfront/).
