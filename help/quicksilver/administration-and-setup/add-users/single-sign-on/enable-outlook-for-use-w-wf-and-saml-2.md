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
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Outlook inschakelen voor gebruik met Workfront en SAML 2.0

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

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   >![](assets/if-you-enable.png)
   >

1. Klik **sparen**.

   De wijzigingen die u hier hebt opgeslagen, zijn van invloed op de ervaring van alle gebruikers in Workfront.
