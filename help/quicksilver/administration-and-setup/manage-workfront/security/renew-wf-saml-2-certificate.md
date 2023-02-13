---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,beveiliging,certificaat,beheerder,vrijstelling,configuratie,metagegevens
navigation-topic: security
title: Het Adobe Workfront SAML 2.0-metagegevenscertificaat verlengen
description: De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn gegaan. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Het Adobe Workfront SAML 2.0-metagegevenscertificaat verlengen

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn gegaan. Als uw organisatie is aangemeld bij de Adobe Admin Console, is geen actie nodig.
>
>Voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

De Adobe Workfront-servers gebruiken het SAML 2.0-protocol voor verificatie en verificatie. Zodra bijgewerkt, blijft het nieuwe certificaat één jaar geldig. Wanneer het tijd is voor u om het certificaat op uw identiteitsleverancier te vernieuwen, ontvangt u een waarschuwing in Workfront die u waarschuwt dat deze verandering moet voorkomen. Als Workfront-beheerder kunt u deze wijziging op systeemniveau beheren.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

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

## SAML 2.0 configureren in Workfront

U kunt als volgt het waarschuwingsbericht bekijken en de update van de SAML 2.0-metagegevens in uw identiteitsprovider bevestigen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Single Sign-On**.

1. In de **Type** vervolgkeuzelijst, selecteert u **SAML 2.0**.

1. Klikken **SAML 2.0-metagegevens downloaden**.

   Hiermee wordt het vernieuwde Workfront-certificaat voor SAML 2.0 gedownload, dat de juiste metagegevens voor uw server bevat.

   >[!CAUTION]
   >
   >Voordat u de Workfront-metagegevens uploadt naar uw Single Sign-On (SSO) provider in Stap 5, kopieert u de huidige URL van de Service voor consumenten van de Bevestiging (ACS) naar een veilige plaats. Deze URL, ook wel de antwoordURL genoemd, staat op de Workfront-configuratiepagina van uw SSO-provider.
   >
   >
   >Als de ACS-URL verandert nadat u de Workfront-metagegevens hebt geüpload, betekent dit dat de metagegevens mogelijk een onjuiste ACS-URL bevatten. U moet deze terugzetten naar de versie die u hebt gekopieerd om te voorkomen dat de Single Sign-On-verbinding wordt verbroken. Het bijgewerkte certificaat is nog steeds correct nadat u dit hebt gedaan.

1. Ga naar de server van uw identiteitsprovider en werk het nieuwe certificaat bij u downloadde.
1. In Workfront, op de **Single Sign-On (SSO) pagina** Selecteer deze optie: **Het nieuwe Workfront-certificaat is al geüpload naar de Identity Provider**.

   Als dit veld is geselecteerd, kunnen Workfront-beheerders zich aanmelden bij Workfront met hun SSO-gegevens of hun Workfront-gegevens.

1. Klikken **Opslaan**.

   Het waarschuwingsbericht wordt niet meer weergegeven omdat u de verlenging van het SAML 2.0-certificaat hebt bevestigd op de server van uw identiteitsprovider.

1. Klikken **Verbinding testen** om uw configuratie te testen.

   Er wordt een bericht weergegeven waarin wordt bevestigd dat de verbinding is gemaakt.

Voor meer informatie, of voor hulp bij de handconfiguratie van meta-gegevens, gelieve ons Team van de Steun te contacteren, zoals die in [Contact opnemen met Klantenondersteuning](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
