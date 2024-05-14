---
title: Vorm [!DNL Workfront] en [!DNL Frame.io] integratie
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als [!DNL Adobe Workfront] beheerder, kunt u integreren [!DNL Workfront] with [!DNL Frame.io] en bieden uw organisatie een naadloze manier om middelen te beoordelen en goed te keuren.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: 089173acb8fecd920ca096c5bf9c6ee61910c20b
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---


# Vorm [!DNL Workfront] en [!DNL Frame.io] integratie

De beheerder van Workfront laat de integratie tussen Workfront en Frame.io toe door de standaardrekening Frame.io in het gebied van de Opstelling te vormen en dan gebruikers Frame.io in Workfront aan te wijzen. Op die manier kan de projectcoördinator met Workfront-projecten plannen en werkzaamheden initiëren en workflows evalueren en goedkeuren.


## Toegangsvereisten

>[!IMPORTANT]
>
>Deze functionaliteit is alleen beschikbaar voor organisaties die aan de [!DNL Adobe Admin Console].

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td>Alle
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenties</strong>
   </td>
   <td>Huidige: [!UICONTROL Plan] <br>
   Nieuw: [!UICONTROL Standard]
   </td>
  </tr>

<tr>
   <td><strong>Configuraties op toegangsniveau</strong>
   </td>
   <td>U moet een [!DNL Workfront] beheerder.
   </td>
  </tr>

</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Een standaard configureren [!DNL Frame.io] account [!BADGE Binnenkort beschikbaar]{type=Informative}

Eenmaal een standaard [!DNL Frame.io] account is ingesteld, alle projecten die zijn gemaakt in [!DNL Workfront] hebben een spiegelproject dat in Frame.io wordt gecreeerd.

>[!IMPORTANT]
>
>Deze functie is binnenkort beschikbaar. Momenteel worden Frame.io-accounts handmatig toegevoegd door het Workfront-team. Neem contact op met uw accountvertegenwoordiger van de Adobe voor hulp.

## Eén Frame.io-account configureren met een Workfront-groep

U kunt één Workfront-groep verbinden met één Frame.io-account die afwijkt van de standaardaccount.

Eén Frame.io-account configureren met een Workfront-groep:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Groepen**.
1. Kies een bestaande groep of klik op **Groep maken**.
1. Klik in het linkerdeelvenster op **Verbinding maken met Frame.io**.
1. Voer het API-ontwikkelaarstoken in.
1. Klikken **Verbinding starten**.
1. (Voorwaardelijk) Als u de beheerder bent van meer dan één Frame.io-account, selecteert u de account die u wilt gebruiken.

## Gebruikers van Frame.io inschakelen

Workfront-gebruikers die regelmatig Frame.io gebruiken, moeten worden gemarkeerd als Frame.io-gebruikers. Workfront-beheerders kunnen Frame.io-gebruikers aanwijzen in het Workfront-gebruikersprofiel.

>[!TIP]
>
>We raden gebruikers aan die regelmatig met creatieve gereedschappen werken, middelen te uploaden om deze te beoordelen en goed te keuren als gebruikers van Frame.io.

Wanneer een gebruiker duidelijk als gebruiker Frame.io in Workfront is en aan een project wordt toegevoegd:

* Zij worden toegevoegd als Medewerker in Frame.io. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Ze kunnen middelen van Frame.io naar Workfront verzenden voor formele controle en goedkeuring.
* Ze kunnen informatie bekijken in de map voor one-way sync vanuit Workfront. [!BADGE Binnenkort beschikbaar]{type=Informative}

Gebruikers van Frame.io inschakelen:

{{step-1-to-users}}

1. Selecteer een of meer gebruikers en klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png).
1. In de sectie van de Toegang, laat toe toevoegt aan projecten in Frame.io checkbox, dan uitgezocht **Ja** in het vervolgkeuzemenu.
   ![](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Als deze doos wordt ongecontroleerd, behoudt de gebruiker toegang tot vroegere taken en toegevoegd aan projecten Frame.io die zich door:sturen.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->

