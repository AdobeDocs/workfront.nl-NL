---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: De integratie met JumpSeat configureren
description: U kunt [!DNL JumpSeat] with [!DNL Workfront] om aangepaste, in-product begeleiding te creëren.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# De integratie met JumpSeat configureren

U kunt [!DNL JumpSeat] with [!DNL Workfront] om aangepaste, in-product begeleiding te creëren.

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
   <td>U moet een actieve [!DNL JumpSeat] plannen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p> U moet een [!DNL Workfront] beheerder. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u begint, moet u

* Toevoegen en activeren [!DNL Workfront] als een toepassing in [!DNL JumpSeat]. Zie voor meer informatie [Een toepassing toevoegen of verwijderen](https://support.jumpseat.io/article/how-to-add-an-application/).

## Vorm [!DNL JumpSeat] integratie

We raden u aan een [!DNL JumpSeat] integratie in zowel uw voorvertoning- als productieomgeving.

>[!TIP]
>
>U moet twee aparte items toevoegen en activeren [!DNL Workfront] toepassingen in [!DNL JumpSeat]—één voor Voorproef en één voor Productie. Zie [Een toepassing toevoegen of verwijderen](https://support.jumpseat.io/article/how-to-add-an-application/) voor meer informatie .

Om te vormen [!DNL JumpSeat] integratie:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]**.
1. Klik in het linkerdeelvenster op **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat] Integration]**.
1. Voer uw **[!UICONTROL [!DNL JumpSeat] URL]**, die u vindt op het extensiepictogram in [!DNL JumpSeat].

   **Voorbeeld:** [!DNL https]://{mycompanyname}.sprongSeoel.io

1. Voer de **[!UICONTROL [!DNL JumpSeat] integration token]**. U vindt dit op de **[!UICONTROL Configuration]** pagina in [!DNL JumpSeat].

   **Voorbeeld:** $2y$10$BevsKeQ8...OYR.LurSg2U64O

1. Klik op **[!UICONTROL Test configuration]**.
1. Kies of u de integratie wilt **[!UICONTROL Active]** of **[!UICONTROL Inactive]**.

   >[!IMPORTANT]
   >
   >De in stap 5 uitgevoerde configuratietest moet slagen om de integratie te activeren.

   ![JumpSeat Integration-pagina](assets/jumpseat-integration-page.png)

1. Klik op **[!UICONTROL Save]**.

>[!TIP]
>
>Voor meer informatie over het configureren van uw [!DNL JumpSeat] integratie, zie [!DNL JumpSeat] documentatie voor [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
