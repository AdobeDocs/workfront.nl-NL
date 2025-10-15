---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Outlook inschakelen voor gebruik met Workfront en SAML 2.0
description: Als u SAML 2.0 authentificatie toelaat en u uw gebruikers aan login aan Workfront van Microsoft Outlook wilt kunnen gebruikend hun geloofsbrieven van SAML 2.0, moet u SAML 2.0 toelaten om in toe:voegen-ins van het Bureau voor authentiek te verklaren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Outlook inschakelen voor gebruik met Workfront en SAML 2.0

>[!IMPORTANT]
>
>[&#x200B; Microsoft is in het proces om steun voor de online tokens van de erfenisUitwisseling &#x200B;](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar te maken, die momenteel door de toe:voegen-binnen van Workfront Vooruitzichten voor authentificatie worden gebruikt. Deze verandering door Microsoft is al begonnen met gevolgen voor de klanten en zal tot oktober 2025 in fasen blijven doorlopen.
>
>* **nadat Microsoft volledig deze tokens onbruikbaar maakt, zal Workfront voor de integratie van Microsoft Outlook niet meer functioneren.**
>
>Als onderdeel van deze wijziging heeft Microsoft besloten om de manier te wijzigen waarop tokens opnieuw worden ingeschakeld. Na **Juni 30, 2025**, zullen de beheerders niet meer tokens kunnen re-toelaten zelf-slechts de Steun van Microsoft kan uitzonderingen verlenen. **Op 1 Oktober, 2025, zullen de erfenistokens voor alle huurders worden uitgezet. Er worden geen uitzonderingen toegestaan.**

Als u SAML 2.0 authentificatie toelaat en u uw gebruikers aan login aan Workfront van Microsoft Outlook wilt kunnen gebruikend hun geloofsbrieven van SAML 2.0, moet u SAML 2.0 toelaten om in toe:voegen-ins van het Bureau voor authentiek te verklaren.

>[!NOTE]
>
>Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie een aangepast SSO-portaal gebruikt.>
><!--
>or is enabled with Adobe IMS>
>-->
>Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Outlook inschakelen voor gebruik met Workfront en SAML 2.0

{{step-1-to-setup}}

1. Klik **Systeem** > **Voorkeur**.

1. In de **sectie van de Veiligheid**, zorg ervoor dat **SAML 2.0 authentificatie in Bureau 365 toe:voegen-ins** wordt toegelaten.

   Met deze optie wordt het insluiten van Workfront alleen voor Office 365-invoegtoepassingen in een iFrame ingeschakeld. Dit opent geen klik-jacking breuk aangezien er geen klikbare inhoud in kwestie is.

   Deze optie is standaard ingeschakeld.

   >[!NOTE]
   >
   >Als u de optie **toelaat het inbedden van Workfront in een iframe**, staat de optie **SAML 2.0 authentificatie in Bureau 365 toe:voegen-ins** toe en wordt toegelaten.
   >
   >![&#x200B; staat het inbedden optie &#x200B;](assets/if-you-enable.png) toe
   >

1. Klik **sparen**.

   De wijzigingen die u hier hebt opgeslagen, zijn van invloed op de ervaring van alle gebruikers in Workfront.
