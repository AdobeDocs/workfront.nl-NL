---
title: Toegang tot merkrechten verlenen
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u merkmachtigingen configureren door een gebruikersgroep in de Admin Console te maken en het productprofiel van de GenStudio-systeembeheerder toe te wijzen.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: ebc342b65bee6a8c5ba0edbe2e990ec2775a9055
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Toegang tot merkrechten verlenen

{{highlighted-preview-article-level}}

Gebruikers krijgen de machtiging om Adobe GenStudio-systeembeheerders te maken, te bewerken en te publiceren wanneer ze aan een gebruikersgroep worden toegevoegd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console-machtigingen</td> 
   <td> <p>U moet systeembeheerder in Adobe Admin Console zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

* Uw instantie van Workfront moet Verenigde Goedkeuringen hebben toegelaten.

* Uw organisatie moet GenStudio Foundation hebben.
   * Content Reviewer in Workfront biedt de functionaliteit die in GenStudio Foundation beschikbaar is voor workflows voor het beoordelen en goedkeuren van bedrijfsmiddelen. U hoeft GenStudio Foundation niet rechtstreeks te openen om uw werk te voltooien. Je toegang tot GenStudio Foundation-functionaliteit via Content Reviewer valt onder de voorwaarden van je Workfront-contract.
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.
Voor meer informatie bij het ondertekenen van de overeenkomst, zie [&#x200B; Ondertekenen de overeenkomst van Adobe Gen AI &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## &#x200B;1. Stel merkmachtigingen in de Admin Console in

### Stap 1: Een gebruikersgroep maken

Maak een nieuwe gebruikersgroep in de Admin Console voor het beheer van machtigingen voor het maken en bewerken van merken.

### Stap 2: Een productprofiel toewijzen aan de gebruikersgroep

De machtiging die aan het toegewezen profiel is gekoppeld, geeft alle gebruikers in deze groep GenStudio Brands-machtigingen (merken maken, bijwerken en verwijderen).

Een profiel toewijzen:

1. Navigeer naar de nieuwe gebruikersgroep.
1. Klik de **Toegewezen productprofielen** tabel.
1. Klik **toewijzen profiel**.
1. In popup, uitgezochte **Adobe GenStudio** van de productlijst, dan klik **&#x200B;**&#x200B;van toepassing zijn.
1. Selecteer het **profiel van de systeemmanager van Adobe GenStudio**.
1. Klik **toepassen**.
1. Klik **sparen**.

### Stap 3: Gebruikers toevoegen aan de gebruikersgroep

Als u gebruikersmachtigingen wilt toewijzen om merken te maken, bewerken en publiceren, voegt u deze toe aan de gebruikersgroep.

>[!NOTE]
>
>U moet minstens één gebruiker toevoegen alvorens de groep aan een project toe te voegen zoals die in stap 4 wordt beschreven.

Gebruikers toevoegen:

1. Ga naar **Admin Console** > **Gebruikers** > **Gebruikersgroepen**.
1. Selecteer uw gebruikersgroep.
1. Voeg gebruikers toe op gebruikersnaam of e-mailadres.
1. Selecteer uit voorgestelde overeenkomsten voor bestaande gebruikers.

### Stap 4: Een Brands-project maken

Een project biedt een opslaglocatie waar gebruikers merkelementen kunnen opslaan.

Een project maken:

1. Navigeer aan het **lusje van de Opslag** in Admin Console.
1. Klik **Projecten**.
1. Klik **creëren Project**.
1. In popup, ga de projectnaam in: **Adobe GenStudio Merken**.

   >[!IMPORTANT]
   >
   >Ga precies de projectnaam in zoals getoond. Voeg geen extra spaties toe of wijzig het hoofdlettergebruik.

1. Klik **creëren**.

### Stap 5: Nodig de gebruikersgroep aan het project uit

Voeg de gebruikersgroep aan het project van Banden toe zodat kunnen zij tot activa toegang hebben en leiden.

1. In **Uitnodiging aan project** popup, voeg de gebruikersgroep toe u creeerde.
1. Selecteer **kan** toestemmingen uitgeven.
1. Klik **Uitnodigen**.

### Resultaat

Gebruikers in de groep hebben nu machtigingen om in Workfront merkmiddelen te maken, bewerken en publiceren.

## &#x200B;2. Toegang verlenen aan merken in Workfront

U moet alle stappen in de vorige sectie voltooien voordat u afzonderlijke gebruikers toegang verleent tot merken in Workfront-toegangsniveaus.

>[!IMPORTANT]
>
>* Alleen gebruikers die met het GenStudio-productprofiel voor systeembeheer in de Admin Console aan de gebruikersgroep zijn toegewezen, kunnen in Workfront merken maken, bewerken en publiceren, zelfs als andere gebruikers toegang tot merken hebben die in hun instellingen voor toegangsniveaus zijn ingeschakeld.
>* Gebruikers die aan het toegangsniveau zijn toegevoegd met Brands-toegang ingeschakeld, maar die niet aan de gebruikersgroep in de Admin Console zijn toegevoegd, kunnen alleen merken weergeven.


Toegang verlenen tot merken in Workfront:

{{step-1-to-setup}}

1. Klik **Niveaus van de Toegang** in het linkerpaneel.
1. Vind het toegangsniveau u wilt uitgeven, dan klik uitgeven pictogram ![&#x200B; pictogram &#x200B;](assets/edit-icon.png) uitgeven om het uit te geven.

   of

   Klik **Nieuw Niveau van de Toegang** om een nieuw toegangsniveau tot stand te brengen. Voor meer informatie over het creëren van toegangsniveaus, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.
1. De rol neer aan **vastgestelde extra beperkingen**, dan uitgezocht **staat gebruikers toe om tot Banden** toegang te hebben.
   ![&#x200B; staat toegang tot brands toe die &#x200B;](assets/access-for-brands.png) plaatsen
1. Klik **sparen**.

Als u merken hebt geconfigureerd, kunt u een Content Reviewer maken om elementen te controleren aan de hand van de richtlijnen van het merk in de revisie- en goedkeuringswerkstroom. Voor meer informatie, zie [&#x200B; AI Medewerkers &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md) vormen.