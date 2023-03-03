---
title: Verborgen bestand
description: Verborgen van zoekopdracht en van linkernav
hidefromtoc: true
hide: true
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: a151fa70a1093db3d9a0af1f4024d5d4cb5fd317
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# Overzicht van uitgebreide verificatie

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront wijzigt het systeembeheer van gebruikers en wachtwoorden. Deze veranderingen zullen uit in een gefaseerde geroepen versie uitrollen **Verbeterde verificatie** ervaring. De verbeterde Authentificatie biedt gebruikers een consistentere en veilige login ervaring over alle producten en de diensten van Workfront.

De volgende tabel bevat details over de huidige en toekomstige functionaliteit:

>[!IMPORTANT]
>
>De meeste klanten gebruiken momenteel Verouderde Authentificatie en sommige gebruiken Verbeterde Authentificatie 1.0.
> 
>Ga naar *your_domain*.my.workfront.com/login. Als u aan /auth/login opnieuw wordt gericht, dan gebruikt u Verbeterde Authentificatie 1.0.
> 
>Als u wordt omgeleid naar https://login-a-xx.workfront.com/, waar &#39;xx&#39; VS (Verenigde Staten), EU (Europa), of GCP (het Platform van de Wolk van Google) afhankelijk van uw plaats/platform zou kunnen zijn, dan gebruikt u Verbeterde Authentificatie 2.0.
>
>Alle klanten zullen naar Verbeterde Authentificatie 2.0 tegen eind 2021 overgaan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Functie</strong> </p> </th> 
   <th><strong>Oudere verificatie</strong> </th> 
   <th><strong>Verbeterde verificatie 1.0</strong> </th> 
   <th> <p>Verbeterde verificatie 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Aanmeldingsopties</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eén gebruikersnaam inschakelen voor alle Workfront-producten en -services, waaronder training, ondersteuning en andere</p> </td> 
   <td>Niet beschikbaar</td> 
   <td> <p>Niet beschikbaar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hetzelfde e-mailadres gebruiken in Workfront-instanties</p> </td> 
   <td> <p>✓</p> <p>Beschikbaar vanaf de release 2019.3</p> </td> 
   <td> <p>✓</p> <p>Beschikbaar vanaf de release 2019.3</p> </td> 
   <td> <p>✓</p> <p>Beschikbaar vanaf de release 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>E-mailadressen zijn hoofdlettergevoelig</p> </td> 
   <td> <p>✓</p> <p>Beschikbaar vanaf de release 2019.3</p> </td> 
   <td> <p>✓</p> <p>Meerdere gebruikers kunnen niet hetzelfde e-mailadres hebben als het adres alleen per geval verschilt. </p> </td> 
   <td> <p>✓</p> <p>Meerdere gebruikers kunnen niet hetzelfde e-mailadres hebben als het adres alleen per geval verschilt. </p> <p>Workfront-beheerders zullen eind 2019 op de hoogte worden gesteld om dubbele e-mailadressen op te lossen.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Opties voor wachtwoordbeheer</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een e-mailbericht voor het opnieuw instellen van wachtwoorden voor een gebruiker uitnodigen als Workfront-beheerder</p> </td> 
   <td> <p>Niet beschikbaar </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een tijdelijk wachtwoord instellen voor een gebruiker als Workfront-beheerder</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Niet gepland</p> <p>Deze functionaliteit is geen best practice voor beveiliging</p> </td> 
   <td> <p>Niet gepland</p> <p>Deze functionaliteit is geen best practice voor beveiliging</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Wachtwoordbeleidsvereisten</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gebruikers moeten hun wachtwoorden opnieuw instellen na een bepaald tijdsbestek</p> </td> 
   <td>✓</td> 
   <td> <p>Niet gepland</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gebruikers beperken tot het gebruik van een vorig wachtwoord </p> </td> 
   <td>✓</td> 
   <td>Niet gepland </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Beveiliging tegen pogingen tot onjuiste invoer van wachtwoord </p> </td> 
   <td> <p>✓ </p> <p>Hiermee vergrendelt u het account nadat 5 pogingen tot het invoeren van een onjuist wachtwoord zijn uitgevoerd. De wachttijd die vereist is nadat de vergrendeling is geconfigureerd door de Workfront-beheerder</p> </td> 
   <td> <p>✓</p> <p>De wachttijd wordt exponentieel verhoogd na elk opeenvolgend onjuist wachtwoord op basis van best practices van de branche. de vereiste tijd kan niet worden geconfigureerd door de Workfront-beheerder</p> </td> 
   <td> <p>✓</p> <p>Gebruikt een lock-out algoritme die proactief een verscheidenheid van verdacht gedrag blokkeert.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Combinatie van kleine letters, hoofdletters, cijfers en speciale tekens vereisen</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Meer flexibiliteit bij het kiezen van specifieke vereisten</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Minimumlengte voor wachtwoorden instellen </p> </td> 
   <td> Niet beschikbaar </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Ondersteuning voor Single Sign-On Protocol</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Ondersteunt SSO-integratie die compatibel is met Active Directory- en LDAP-protocollen</p> </td> 
   <td> ✓ </td> 
   <td> <p> Vervangen</p> <p>Active Directory-, Azure- en LDAP-systemen moeten SAML 2.0 gebruiken</p> </td> 
   <td> <p>Vervangen</p> <p>Active Directory-, Azure- en LDAP-systemen kunnen worden geconfigureerd met gecodeerde SAML 2.0- of OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Steunt protocollen SSO die met SAML 2.0 volgzaam zijn </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ondersteunt geopende ID Connect-protocollen</p> </td> 
   <td> <p>Niet beschikbaar</p> </td> 
   <td> <p>Niet beschikbaar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> De Workfront-aanmeldingspagina configureren om altijd om te leiden naar de aanmeldingspagina van de identiteitsprovider </p> </td> 
   <td> Deze optie is standaard ingeschakeld en kan niet worden uitgeschakeld</td> 
   <td> <p>✓</p> <p>De Workfront-beheerder kan de aanmeldingspagina zo configureren dat deze wordt omgeleid naar de aanmeldingspagina van de identiteitsprovider, of kan een of meer aanmeldknoppen configureren.</p> </td> 
   <td> <p>✓</p> <p> Workfront-beheerders kunnen de aanmeldingspagina zo configureren dat deze wordt omgeleid naar de aanmeldingspagina van de identiteitsprovider, of ze kunnen een of meer aanmeldknoppen configureren.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Elke instantie toestaan om meerdere SSO-providers in te schakelen</p> </td> 
   <td> <p>N.v.t.</p> </td> 
   <td> <p>Niet gepland</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Omgevingsondersteuning</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Eén gebruikersnaam en wachtwoord voor voorvertoningsomgevingen</p> </td> 
   <td> <p>Niet beschikbaar</p> </td> 
   <td> <p>Niet beschikbaar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eén gebruikersnaam en wachtwoord voor Sandbox-omgevingen</p> </td> 
   <td> <p>Niet beschikbaar</p> </td> 
   <td> <p>Niet beschikbaar</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
