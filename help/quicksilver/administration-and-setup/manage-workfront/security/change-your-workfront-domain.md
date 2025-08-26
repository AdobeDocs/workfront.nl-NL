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
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '421'
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

## Een domeinwijziging aanvragen

1. Beginnen met het maken van een ondersteuningsticket op Experience League.
1. In het **vakje van de Beschrijving**, omvat het nieuwe domein u wilt, evenals timeframe wanneer u het nieuwe domein live wilt gaan.
1. Voltooi het invullen van de dozen voor het steungeval, dan klik **voorleggen**.

U kunt ook Workfront Support bellen om hulp bij het wijzigen van uw domein te krijgen.

## Werk het nieuwe domein bij als u een klant SSO bent

Als uw bedrijf SSO gebruikt, worden de volgende stappen vereist nadat u uw Workfront domein hebt veranderd.

>[!NOTE]
>
>Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

{{step-1-to-setup}}

1. In linkerzijbalk, klik **Systeem** > **Info van de Klant** en zorg ervoor dat uw domein op de pagina van Info van de Klant wordt bijgewerkt.

1. In linkerzijbalk, klik **Systeem** > **Enige Sign-On (SSO)**.

1. Klik **Download SAML 2.0 Meta-gegevens**.
1. Nadat het bestand is gedownload, opent u het en controleert u het volgende:

   1. **entityID** richt aan het nieuwe domein.
   1. Alle locaties in **`<md:AssertionConsumerService>`** verwijzen naar het nieuwe domein.

1. Geef het gedownloade metagegevensbestand op aan uw Identiteitsprovider zodat deze het op hun einde kan bijwerken.
1. Zorg ervoor dat het domein wordt bijgewerkt voor alle Workfront-integraties die door uw organisatie worden gebruikt.
