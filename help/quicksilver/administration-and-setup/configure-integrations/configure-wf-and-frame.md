---
title: Vorm  [!DNL Workfront]  en  [!DNL Frame.io]  Integratie
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als  [!DNL Adobe Workfront]  beheerder, kunt u  [!DNL Workfront]  met  [!DNL Frame.io]  integreren en uw organisatie van een naadloze manier voorzien om activa te herzien en goed te keuren.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
hide: true
hidefromtoc: true
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# De integratie van [!DNL Workfront] en [!DNL Frame.io] configureren

De beheerder van Workfront laat de integratie tussen Workfront en Frame.io toe door de standaardrekening Frame.io in het gebied van de Opstelling te vormen en dan gebruikers Frame.io in Workfront aan te wijzen. Op die manier kan de projectcoördinator met Workfront-projecten plannen en werkzaamheden initiëren en workflows evalueren en goedkeuren.


## Toegangsvereisten

>[!IMPORTANT]
>
>Deze functionaliteit is alleen beschikbaar voor organisaties die zijn aangemeld bij de [!DNL Adobe Admin Console] .

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] plan</td>
   <td>Alle</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] licenties
   </td>
   <td><p>Huidige: [!UICONTROL Plan]</p>
   <p>Nieuw: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>

</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vorm een gebrek [!DNL Frame.io] rekening [!BADGE &#x200B; Binnenkort &#x200B;]{type=Informative}

Zodra een standaard [!DNL Frame.io] rekening opstelling is, hebben om het even welke projecten die in [!DNL Workfront] worden gecreeerd een spiegelproject dat in Frame.io wordt gecreeerd.

>[!IMPORTANT]
>
>Deze functie is binnenkort beschikbaar. Momenteel worden Frame.io-accounts handmatig toegevoegd door het Workfront-team. Neem contact op met uw Adobe-accountvertegenwoordiger voor hulp.

## Eén Frame.io-account configureren met een Workfront-groep

U kunt één Workfront-groep verbinden met één Frame.io-account die afwijkt van de standaardaccount.

Eén Frame.io-account configureren met een Workfront-groep:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen**.
1. Kies een bestaande groep, of klik **creeer groep**.
1. In het linkerpaneel, klik **verbinden met Frame.io**.
1. Voer het API-ontwikkelaarstoken in.
1. Klik **initiëren Verbinding**.
1. (Voorwaardelijk) Als u de beheerder bent van meer dan één Frame.io-account, selecteert u de account die u wilt gebruiken.

## Gebruikers van Frame.io inschakelen

Workfront-gebruikers die regelmatig Frame.io gebruiken, moeten worden gemarkeerd als Frame.io-gebruikers. Workfront-beheerders kunnen Frame.io-gebruikers aanwijzen in het Workfront-gebruikersprofiel.

>[!TIP]
>
>We raden gebruikers aan die regelmatig met creatieve gereedschappen werken, middelen te uploaden om deze te beoordelen en goed te keuren als gebruikers van Frame.io.

Wanneer een gebruiker duidelijk als gebruiker Frame.io in Workfront is en aan een project wordt toegevoegd:

* Zij worden toegevoegd als Medewerker in Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Ze kunnen middelen van Frame.io naar Workfront verzenden voor formele controle en goedkeuring.
* Ze kunnen informatie bekijken in de map voor one-way sync vanuit Workfront. [!BADGE &#x200B; Binnenkort &#x200B;]{type=Informative}

Gebruikers van Frame.io inschakelen:

{{step-1-to-users}}

1. Selecteer één of meerdere gebruikers, dan klik **uitgeven** pictogram ![ pictogram ](assets/edit-icon.png) uitgeeft.
1. In de sectie van de Toegang, laat toe toevoegen aan projecten in Frame.io checkbox, dan selecteren **ja** in het drop-down menu.
   ![ voeg aan het project van het Kader toe ](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Als deze doos wordt ongecontroleerd, behoudt de gebruiker toegang tot vroegere taken en aan projecten toegevoegd Frame.io die zich door:sturen.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
