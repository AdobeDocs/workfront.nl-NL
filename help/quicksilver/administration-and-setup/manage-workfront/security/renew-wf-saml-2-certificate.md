---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,beveiliging,certificaat,beheerder,vrijstelling,configuratie,metagegevens
navigation-topic: security
title: Het Adobe Workfront SAML 2.0-metagegevenscertificaat verlengen
description: De Adobe Workfront-servers gebruiken het SAML 2.0-protocol voor verificatie en verificatie. Zodra bijgewerkt, blijft het nieuwe certificaat één jaar geldig. Wanneer het tijd is voor u om het certificaat op uw identiteitsleverancier te vernieuwen, ontvangt u een waarschuwing in Workfront die u waarschuwt dat deze verandering moet voorkomen. Als Workfront-beheerder kunt u deze wijziging op systeemniveau beheren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Het Adobe Workfront SAML 2.0-metagegevenscertificaat verlengen

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan de Admin Console zijn geregistreerd. Als uw organisatie is aangemeld bij de Adobe Admin Console, is geen actie nodig.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfs Platform) ](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

De Adobe Workfront-servers gebruiken het SAML 2.0-protocol voor verificatie en verificatie. Zodra bijgewerkt, blijft het nieuwe certificaat één jaar geldig. Wanneer het tijd is voor u om het certificaat op uw identiteitsleverancier te vernieuwen, ontvangt u een waarschuwing in Workfront die u waarschuwt dat deze verandering moet voorkomen. Als Workfront-beheerder kunt u deze wijziging op systeemniveau beheren.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

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
  <td> <p>Nieuw: Standaard </p>
 <p>of</p> 
<p>Huidig: Plan </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## SAML 2.0 configureren in Workfront

U kunt als volgt het waarschuwingsbericht bekijken en de update van de SAML 2.0-metagegevens in uw identiteitsprovider bevestigen:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. Klik **Systeem** > **Enige Sign-On**.

1. In het **Type** drop-down menu, uitgezochte **SAML 2.0**.

1. Klik **Download SAML 2.0 Meta-gegevens**.

   Hiermee wordt het vernieuwde Workfront-certificaat voor SAML 2.0 gedownload, dat de juiste metagegevens voor uw server bevat.

1. Kopieer in uw identiteitsprovider de huidige ACS-URL (ook wel de antwoordURL genoemd) voor de service voor de bevestiging van de consument naar een veilige plaats.

   >[!CAUTION]
   >
   >Voordat u de Workfront-metagegevens uploadt naar uw Single Sign-On (SSO) provider in Stap 6, kopieert u de huidige URL van de Service voor consumenten van de Bevestiging (ACS) naar een veilige plaats. Deze URL, ook wel de antwoordURL genoemd, staat op de Workfront-configuratiepagina van uw SSO-provider.
   >
   >
   >Als de ACS-URL verandert nadat u de Workfront-metagegevens hebt geüpload, betekent dit dat de metagegevens mogelijk een onjuiste ACS-URL bevatten. U moet deze terugzetten naar de versie die u hebt gekopieerd om te voorkomen dat de Single Sign-On-verbinding wordt verbroken. Het bijgewerkte certificaat is nog steeds correct nadat u dit hebt gedaan.

1. Werk het nieuwe certificaat dat u hebt gedownload bij op uw server voor identiteitsproviders.
1. (Voorwaardelijk) als URL van de Dienst van de Consument van de Bevestiging (ACS) of Reageren URL in uw identiteitsleverancier is veranderd, verander het terug naar URL u in Stap 5 kopieerde.
1. In Workfront, op de **Enige Sign-On (SSO) pagina**, zorg ervoor dat deze optie wordt geselecteerd: **het nieuwe certificaat van Workfront is reeds geupload aan de Leverancier van de Identiteit**.

   >[!NOTE]
   >
   >* Deze optie is alleen zichtbaar als alle volgende opties van toepassing zijn:
   >   * Uw organisatie is reeds opstelling voor SAML 2.0
   >   * Het huidige certificaat is gereed om te verlopen
   >   * Het nieuwe certificaat is beschikbaar
   >* Als dit veld is geselecteerd, kunnen Workfront-beheerders zich aanmelden bij Workfront met hun SSO-gegevens of hun Workfront-gegevens.

1. Klik **sparen**.

   Het waarschuwingsbericht wordt niet meer weergegeven omdat u de verlenging van het SAML 2.0-certificaat hebt bevestigd op de server van uw identiteitsprovider.

1. Klik **Verbinding van de Test** om uw configuratie te testen.

   Er wordt een bericht weergegeven waarin wordt bevestigd dat de verbinding tot stand is gebracht.

Voor meer informatie, of voor hulp met de handconfiguratie van meta-gegevens, gelieve ons Team van de Steun te contacteren, zoals die in [ de Steun van de Klant van het Contact ](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md) wordt verklaard.
