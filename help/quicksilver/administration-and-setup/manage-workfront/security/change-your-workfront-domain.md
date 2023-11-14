---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Je Adobe Workfront-domein wijzigen
description: Als Adobe Workfront-beheerder en geautoriseerde contactpersoon voor Workfront-ondersteuning kunt u hulp aanvragen bij het Workfront-ondersteuningsteam om het Workfront-domein van uw organisatie te wijzigen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: 22ea9b623d7bc7b216511538cf88e4d020529bd3
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Je Adobe Workfront-domein wijzigen

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan de Admin Console zijn geregistreerd. Als uw organisatie is aangemeld bij de Adobe Admin Console, is het niet mogelijk om uw Workfront-domein te wijzigen.
>
>Ga voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console naar [Platformgebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-beheerder en geautoriseerde contactpersoon voor Workfront-ondersteuning kunt u hulp aanvragen bij het Workfront-ondersteuningsteam om het Workfront-domein van uw organisatie te wijzigen.

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een domeinwijziging aanvragen

1. Beginnen met het maken van een ondersteuningsticket op het Experience League.
1. In de **Beschrijving** bevat het nieuwe domein dat u wilt gebruiken en ook het tijdframe waarin u het nieuwe domein live wilt laten gaan.
1. Vul de vakken voor de draagtas in en klik op **Verzenden**.

U kunt ook Workfront Support bellen om hulp bij het wijzigen van uw domein te krijgen.

## Werk het nieuwe domein bij als u een klant SSO bent

Als uw bedrijf SSO gebruikt, worden de volgende stappen vereist nadat u uw Workfront domein hebt veranderd.

>[!NOTE]
>
>Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in de linkerzijbalk op **Systeem** > **Klantgegevens** en zorg ervoor dat uw domein op de pagina van Info van de Klant wordt bijgewerkt.

1. Klik in de linkerzijbalk op **Systeem** > **Eenmalige aanmelding (SSO)**.

1. Klikken **SAML 2.0-metagegevens downloaden**.
1. Nadat het bestand is gedownload, opent u het en controleert u het volgende:

   1. **entityID** verwijst naar het nieuwe domein.
   1. Alle locaties binnen **`<md:AssertionConsumerService>`** verwijzen naar het nieuwe domein.

1. Geef het gedownloade metagegevensbestand op aan uw Identiteitsprovider zodat deze het op hun einde kan bijwerken.
1. Zorg ervoor dat het domein wordt bijgewerkt voor alle Workfront-integraties die door uw organisatie worden gebruikt.
