---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Outlook inschakelen voor gebruik met Workfront en SAML 2.0
description: Als u SAML 2.0 authentificatie toelaat en u uw gebruikers aan login aan Workfront van Microsoft Outlook wilt kunnen gebruikend hun geloofsbrieven van SAML 2.0, moet u SAML 2.0 toelaten om in toe:voegen-ins van het Bureau voor authentiek te verklaren.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Outlook inschakelen voor gebruik met Workfront en SAML 2.0

1. Klikken **Instellen** in de rechterbovenhoek van Adobe Workfront op de algemene navigatiebalk.
1. Klikken **Systeem** > **Voorkeuren**.

1. In de **Beveiliging** in, zorg ervoor dat **SAML 2.0-verificatie toestaan in Office 365 add-ins** is ingeschakeld.

   Met deze optie wordt het insluiten van Workfront alleen voor Office 365-invoegtoepassingen in een iFrame ingeschakeld. Dit opent geen klik-jacking breuk aangezien er geen klikbare inhoud in kwestie is.

   Deze optie is standaard ingeschakeld.

   >[!NOTE]
   >
   >Als u de optie inschakelt **Insluiten van Workfront in een iframe toestaan**, de optie **SAML 2.0-verificatie toestaan in Office 365 add-ins** is grijs en ingeschakeld.
   >
   >![](assets/if-you-enable.png)

1. Klikken **Opslaan**.

   De wijzigingen die u hier hebt opgeslagen, zijn van invloed op de ervaring van alle gebruikers in Workfront.
