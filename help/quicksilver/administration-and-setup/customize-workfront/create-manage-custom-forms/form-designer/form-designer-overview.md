---
title: Overzicht van de formulierontwerper
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een aangepast formulier ontwerpen dat gebruikers aan een Workfront-object kunnen koppelen. Gebruikers die aan het object werken, kunnen het aangepaste formulier invullen om informatie over het object te geven.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 061d1a08a8c99b2770491ce2fcea63a9dad7a63f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Overzicht van de formulierontwerper

>[!IMPORTANT]
>
>De formulierontwerper is op 24 mei 2023 tijdelijk uitgeschakeld. Met de verouderde formulierontwikkelaar kunt u aangepaste formulieren maken en bewerken. Zie [Een aangepast formulier maken of bewerken met de oudere formulierbuilder](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/use-the-custom-form-builder.md).

Met de nieuwe formulierontwerper kunt u een aangepast formulier ontwerpen dat gebruikers aan een Workfront-object kunnen koppelen. Gebruikers die aan het object werken, kunnen het aangepaste formulier invullen om informatie over het object te geven.

De nieuwe formulierontwerper heeft een nieuwe werkruimte in canvasstijl waarmee u de velden, het canvas en de veldinstellingen tegelijkertijd kunt bekijken. U kunt ook velden in de secties slepen en neerzetten terwijl u het formulier ontwerpt.

<!-- add screenshot when field settings empty state is ready -->

## Toegang tot de nieuwe formulierontwerper

Er is een nieuwe knop boven aan zowel de nieuwe formulierontwerper als de verouderde formulierontwerper. U kunt deze knoop gebruiken om tussen de erfenisbouwer en de nieuwe ontwerper te schakelen.

![](assets/switch-views.png)

## Nieuwe functionaliteit beschikbaar bij de formulierontwerper

Met de nieuwe formulierontwerper hebben we de mogelijkheid toegevoegd om

* **Een veld kopiëren**: U kunt bestaande velden nu kopiëren door rechtstreeks vanaf het canvas op het pictogram Kopiëren op de velden te klikken.

* **De grootte voor beschrijvende tekst wijzigen**: U kunt nu kleine, middelgrote of grote formaten toewijzen aan beschrijvende tekstvelden. U kunt ze ook op dezelfde rij gebruiken met andere velden.

* **Standaardsectie gebruiken**: Als de maker van het formulier geen sectie boven aan het formulier heeft toegevoegd, wordt nu een sectie Standaard weergegeven op het canvas, zodat gebruikers de machtigingen kunnen aanpassen voor velden waaraan geen aangepaste sectie is toegewezen.

   >[!NOTE]
   >
   >De standaardsectie is niet zichtbaar binnen objecten als het formulier eenmaal aan het object is gekoppeld.

## Functionaliteit binnenkort beschikbaar

De volgende opties zijn momenteel niet beschikbaar in de formulierontwerper, maar worden binnenkort toegevoegd:

* Logica weergeven/overslaan

* Filteren voor velden van typekop

>[!IMPORTANT]
>
>De bestaande configuraties voor logica- en typerefilters worden niet beïnvloed wanneer u met de nieuwe formulierontwerper werkt.

## Functionaliteit verwijderd van de formulierontwerper

De volgende functionaliteit is verwijderd uit de formulierontwerper:


* Formulierinstellingen, Formulier delen, tabbladen voor delen van velden

   * De formulierinstellingen zijn nu beschikbaar boven aan het canvas

   * Het hoofdtabblad Formulier delen en het subtabblad Veld delen
   >[!NOTE]
   >
   >U kunt het delen van formulieren en velden besturen via Instellen > Aangepaste Forms > Forms of het tabblad Velden.

* Wijzigingen in veld bijhouden in updateffeeds
   >[!NOTE]
   >
   >U vindt dit in Setup > Interface > feeds bijwerken
