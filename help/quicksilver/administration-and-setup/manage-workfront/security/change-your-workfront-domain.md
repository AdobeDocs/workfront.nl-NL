---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Adobe Workfront-domein wijzigen
description: Als Adobe Workfront-beheerder en geautoriseerde contactpersoon voor Workfront-ondersteuning kunt u hulp aanvragen bij het Workfront-ondersteuningsteam om het Workfront-domein van uw organisatie te wijzigen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Je Adobe Workfront-domein wijzigen

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn. Als uw organisatie is aangemeld bij de Adobe Admin Console, is het niet mogelijk om uw Workfront-domein te wijzigen.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfsplatform) ](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-beheerder en geautoriseerde contactpersoon voor Workfront-ondersteuning kunt u hulp aanvragen bij het Workfront-ondersteuningsteam om het Workfront-domein van uw organisatie te wijzigen.

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

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een domeinwijziging aanvragen

1. Beginnen met het maken van een ondersteuningsticket op Experience League.
1. In het **vakje van de Beschrijving**, omvat het nieuwe domein u wilt, evenals timeframe wanneer u het nieuwe domein live wilt gaan.
1. Voltooi het invullen van de dozen voor het steungeval, dan klik **voorleggen**.

U kunt ook Workfront Support bellen om hulp bij het wijzigen van uw domein te krijgen.

<!--

## Update the new domain if you are an SSO customer

If your company utilizes SSO, the following steps are required after you have your Workfront domain changed.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

{{step-1-to-setup}}

1. In the left sidebar, click **System** > **Customer Info** and make sure that your domain is updated on the Customer Info page.

1. In the left sidebar, click **System** > **Single Sign-On (SSO)**.

1. Click **Download SAML 2.0 Metadata**.
1. After the file is downloaded, open it and make sure of the following:

   1. **entityID** is pointing to the new domain.
   1. All locations within **`<md:AssertionConsumerService>`** point to the new domain.

1. Provide the downloaded metadata file to your Identity Provider so that they can update it on their end.
1. Make sure the domain is updated for all Workfront integrations used by your organization.


-->
