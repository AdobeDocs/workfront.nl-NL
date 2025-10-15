---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: De integratie met JumpSeat configureren
description: U kunt  [!DNL JumpSeat]  met  [!DNL Workfront]  integreren om douane, in-productbegeleiding tot stand te brengen.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 1%

---

# De integratie met JumpSeat configureren

U kunt [!DNL JumpSeat] integreren met [!DNL Workfront] om aangepaste, in-product begeleiding te maken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table>
  <tr>
   <td>Adobe Workfront-pakket
   </td>
    <p>Workflow Ultimate</p>
   <td> <p>Prime of Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront-licenties
   </td>
   <td>Standard
   <p>Plan</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>Product
   </td>
   <td>U moet een actief [!DNL JumpSeat] plan hebben.
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u begint, moet u

* Voeg [!DNL Workfront] toe en activeer dit als een toepassing in [!DNL JumpSeat] . Voor meer informatie, zie [ hoe te om een toepassing ](https://support.jumpseat.io/article/how-to-add-an-application/) toe te voegen of te schrappen.

>[!IMPORTANT]
>
>Als u op de Adobe Verenigde Ervaring bent, moet u volgende Application URL gebruiken: `.workfront.adobe.com`.



## De integratie met [!DNL JumpSeat] configureren

We raden u aan een [!DNL JumpSeat] -integratie in te stellen in zowel uw voorvertoning- als productieomgeving.

>[!TIP]
>
>U moet twee aparte [!DNL Workfront] -toepassingen toevoegen en activeren in [!DNL JumpSeat] : een voor Voorvertoning en een voor Productie. Zie [ hoe te om een toepassing ](https://support.jumpseat.io/article/how-to-add-an-application/) voor meer informatie toe te voegen of te schrappen.

U configureert de integratie met [!DNL JumpSeat] als volgt:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat] Integration]** .
1. Voer de **[!UICONTROL [!DNL JumpSeat] URL]** in die u vindt op het extensiepictogram in [!DNL JumpSeat] .

>[!BEGINSHADEBOX]

**Voorbeeld:**

https://{mycompanyname}.spronsit.io

>>

>[!ENDSHADEBOX]

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
