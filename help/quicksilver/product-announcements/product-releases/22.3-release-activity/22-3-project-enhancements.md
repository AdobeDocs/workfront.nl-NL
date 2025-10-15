---
title: projectupdates tijdens de releaseperiode van 22.3
description: projectupdates tijdens de releaseperiode van 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1535'
ht-degree: 0%

---

# 22.3 Projectverbeteringen

Op deze pagina worden alle projectverbeteringen beschreven die zijn aangebracht met de release 22.3 voor de voorvertoningsomgeving. Deze verbeteringen zijn in de week van 11 juli 2022 beschikbaar gesteld in de productieomgeving. Voor een lijst van alle veranderingen beschikbaar met de versie 22.3, zie [ overzicht van de Versie 22.3 ](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Delegatie van werkzaamheden buiten het kantoor

Nu, kunt u de taken en de kwesties tijdelijk delegeren die aan u aan andere gebruikers worden toegewezen wanneer u van plan bent om uit het bureau voor een korte periode te zijn. Dit zorgt ervoor dat uw afwezigheid geen wegbelemmering wordt om het werk te voltooien.

Voorafgaand aan deze verbetering, kon u goedkeuringen slechts delegeren.

Hier volgen enkele functies die we met deze update hebben toegevoegd:

* Een instelling in het gedeelte met voorkeuren voor Taken en problemen van Setup voor de systeembeheerder of de groepsbeheerder om delegatie in uw omgeving in te schakelen.

* Een nieuwe optie voor &quot;Taken en kwesties van de Delegatie&quot;in het gebied van het Huis voor gebruikers met een Overzicht of hogere vergunning om hun het werkpunten te delegeren.

* Vermelding in het Thuis en in het gebied Toewijzingen van taak en geef kopteksten uit die punten aan anderen worden gedelegeerd.

* Gebeurtenismeldingen in het gedeelte Setup en e-mailmeldingen in het gebruikersprofiel om e-mailmeldingen over gedelegeerde werkzaamheden te beheren


>[!NOTE]
>
>Alleen gebruikers met een licentie Revisie of hoger kunnen hun werk delegeren aan anderen. Het werk kan aan om het even welke gebruiker, ongeacht hun toegangsniveau worden gedelegeerd. Gedelegeerde gebruikers ontvangen dezelfde machtigingen als de toewijzingen voor de gedelegeerde items. Als deze toestemmingen lager zijn dan de configuratie van het de toegangsniveau van een gebruiker, zouden de gedelegeerde gebruikers kunnen worden verhinderd om sommige activiteiten op de taken en de kwesties uit te voeren die aan hen worden gedelegeerd.


Voor meer informatie, zie [ de taak van de Afgevaardigde en geven overzicht ](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md) uit.

## Nieuwe ervaring bij het converteren van een uitgave naar een taak

Om uw gebruik van Workfront consistent te maken met de nieuwe Workfront-ervaring, hebben we de interface voor het converteren van een uitgave naar een taak opnieuw ontworpen.

Deze update bevat:

* Een bijgewerkte gebruikersinterface die overeenkomt met de rest van de nieuwe Workfront-ervaring.

* Toegang om een kwestie in taken van een lijst of een rapport om te zetten.

* De standaard aangepaste formulieren die zijn gedefinieerd in het gedeelte Taken van het doelproject dat aan de nieuwe taak is toegevoegd.


Voor meer informatie, zie [ Bekeerling een kwestie in een taak ](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## Nieuwe ervaring wanneer het omzetten van een kwestie in een project zonder een malplaatje

Om uw gebruik van Workfront in overeenstemming te brengen met de nieuwe ervaring van Workfront, hebben wij de interface voor het omzetten van een kwestie in een project zonder een malplaatje te gebruiken opnieuw ontworpen.

Naast een bijgewerkte gebruikersinterface die de rest van de nieuwe ervaring van Workfront aanpast, hebben wij ook de capaciteit toegevoegd om een kwestie in lege projecten van een lijst of een rapport om te zetten.

Voor meer informatie, zie [ Bekeerling een kwestie in een project in Adobe Workfront ](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## Slimme tags toepassen in de updatestream

De codering van gebruikers in de updatestream is verbeterd wanneer u een nieuwe update maakt of op een bestaande update reageert. Wanneer u nu een gebruiker codeert om deze in een update op te nemen, naast zijn of haar naam en avatar, geven we ook zijn of haar primaire rol en e-mail weer. Zo kunt u beter onderscheid maken tussen meerdere gebruikers met dezelfde of vergelijkbare namen.

Voor meer informatie, zie [ Tags anderen op updates ](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## Nieuwe syntaxis voor berekeningen in aangepaste velden

Ter voorbereiding op toekomstige verbeteringen die u helpen berekeningen toe te voegen aan aangepaste formulieren, hebben we de syntaxis gestandaardiseerd voor velden waarnaar wordt verwezen en die u toevoegt aan een berekening. Het is eenvoudig om deze nieuwe syntaxis te gebruiken omdat het systeem het voor u ingaat wanneer u begint de naam van een gebied te typen en dan het te selecteren.

## Houd nauwkeurige informatie wanneer twee gebruikers met een gemeenschappelijke rol bij een goedkeuringsproces betrokken zijn

Om ervoor te zorgen dat uw gegevens voor het goedkeuren van uw werk accuraat zijn, hebben we een wijziging aangebracht in de manier waarop goedkeuringsgegevens worden vastgelegd voor een onderdeel wanneer er een goedkeuringsproces met meerdere rollen aan het onderdeel is gekoppeld.

Sommige goedkeuringsprocessen vereisen goedkeuring van twee verschillende rollen, en twee verschillende fiatteurs zouden één van die rollen in gemeenschappelijk kunnen hebben. Wanneer dit gebeurt, registreert Workfront, nadat de goedkeuringsbesluiten zijn genomen, elke fiatteur en zijn respectieve rol verbonden aan het goedkeuringsproces.

Vóór deze wijziging werden beide goedkeuringen vastgelegd voor de tweede gebruiker omdat deze een van de goedkeuringsrollen deelde met de eerste fiatteur. In dit geval heeft de tweede fiatteur de informatie van de eerste fiatteur overschreven.

Voor meer informatie over goedkeuringsprocessen in Workfront, zie [ overzicht van het proces van de Goedkeuring ](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## Toewijzingstijden worden niet meer verwijderd wanneer u wijzigingen aanbrengt in toewijzingen

>[!NOTE]
>
>Deze functie was oorspronkelijk bedoeld om te worden uitgebracht met de release 22.2. Het werd op 21 april 2022 aan Production vrijgegeven.


Om de nauwkeurigheid van uw gegevens te verzekeren, hebben wij een verandering aangebracht om toewijzingstijden te bewaren en taak Geplande Uren ongewijzigd te houden wanneer het aanbrengen van veranderingen in taken op de taak.

De volgende wijzigingen zijn aangebracht in taken met het type Eenvoudige duur:

* Geplande uren blijven behouden wanneer alle toewijzingen worden verwijderd.

* Individuele toewijzingen blijven behouden wanneer gebruikers en rollen worden vervangen.

* Individuele toewijzingen blijven behouden op de rol wanneer de gebruiker wordt verwijderd. (Verwijderd uit de release. Geplande uren worden nu ingesteld op 0 nadat alle toegewezen uren zijn verwijderd.)


Voor meer informatie over Geplande Uren, zie [ Gepland overzicht van Uren ](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## Verbeteringen voor borden

De volgende verbeteringen zijn toegevoegd aan Adobe Workfront-borden:

* Filteropties - U kunt nu filteren op de gewenste datum of status op een board. Het filter is ook bijgewerkt met inklapbare secties om de opties te scheiden.

* Archiefbord - U kunt nu een board archiveren terwijl u in het bord bent, in plaats van naar het dashboard van Borden te moeten gaan.

* Voeg een team aan een raad toe - wanneer u naar leden zoekt, kunt u een volledig team toevoegen. Als u een team kiest, wordt iedereen aan het team toegevoegd.

* Dropzones in kolommen - Wanneer u een kaart van de ene naar de andere bordkolom sleept en neerzet, wordt nu met een grijze &#39;dropzone&#39; aangegeven waar de kaart wordt geplaatst. Voorheen was er geen visuele indicator van de kaartplaatsing.

* Verbonden kaarten - U kunt nu kaarten toevoegen die zijn verbonden met Workfront-taken en -problemen. Als u de naam, beschrijving of toegewezen naam in de kaart of taak bijwerkt, worden dezelfde velden op de andere locatie bijgewerkt.

* Statusveld op alle kaarten - Er zijn een statusveld en een knop Voltooien markeren toegevoegd aan zowel ad-hockaarten als aan gekoppelde kaarten. Wanneer u op Markeren voltooid klikt, verandert de status automatisch in Voltooien.

* Ad-hockaart converteren naar aangesloten kaart - U kunt nu een ad-hockaart converteren naar een aangesloten kaart via de kaartgegevens.

* Verbinding met verbonden kaart verbreken - Als u de verbinding met een aangesloten kaart verbreekt, wordt de verbinding met het Workfront-object verbroken. De kaart blijft als een ad-hockaart op het bord en het Workfront-object wordt hierdoor niet beïnvloed.

* Statustoewijzing in kolommen - Met de nieuwe kolominstellingen en het nieuwe beleid kunt u een status, toewijzing of tag definiëren die wordt toegepast op kaarten die naar die kolom worden verplaatst. Ook, zijn de standaardkolomnamen op een nieuwe raad veranderd in Kolom 1, Kolom 2, en Kolom 3.

* Update-indicator voor velden - Er wordt nu een indicator weergegeven wanneer u een kaart opslaat om te bevestigen dat uw updates zijn opgeslagen.


Voor meer informatie, zie [ begonnen worden met raden in Adobe Workfront ](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## Alleen mappen delen in de bovenste vijf niveaus van een mappenhiërarchie

Voor de beste prestaties voor gebruikers die mappen delen, beperken we het delen momenteel tot de bovenste vijf niveaus in een mappenhiërarchie van een object.

Elke map op het zesde niveau of erft de configuraties voor delen van de map direct erboven.

Voor meer informatie over het delen van omslagen, zie [ een top-level documentomslag ](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md) delen.

## Workfront Campaigns (Beta) - een nieuwe manier om uw werk te beheren

>[!NOTE]
>
>Deze functie wordt verwijderd uit Voorvertoning op 9 januari 2023. Voor meer informatie, zie de [ 23.1 overzichtspagina van de Versie ](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>Dit onderdeel wordt niet opgenomen in de productierelease 2.3. Deze wordt vrijgegeven aan Production met een toekomstige release.


>[!NOTE]
>
>Deze functionaliteit is alleen beschikbaar als een bètaversie en wordt momenteel ontwikkeld. We blijven functies toevoegen voor de Campagne-workflow met toekomstige releases. De deelname aan het bètaprogramma voor Workfront Campaigns is vrijwillig.

We introduceren een nieuw object aan Adobe Workfront dat de manier waarop u het werk beheert, kan veranderen.

Met Workfront Campaigns kunt u projecten organiseren vanuit verschillende portfolio&#39;s en programma&#39;s in een nieuwe werkcontainer. Deze nieuwe container zal in toekomstige versies evolueren om uiteindelijk alle het werkvoorwerpen te omvatten die momenteel in afzonderlijke silo&#39;s worden beheerd.

De volgende functies zijn in deze release opgenomen:

* Een nieuw Workfront-object genaamd Campagne

* Een nieuw gebied Campagnes (Beta) in het Hoofdmenu

* Een lijst met campagnes in het gebied Campagnes

* Een pagina van de Details van de Campagne die extra informatie over een campagne toont

* Mogelijkheid om projecten toe te voegen aan een campagne

* Informatie over een campagne bewerken

* Mogelijkheid om de naam van het Campagneobject te wijzigen via de lay-outsjabloon

  Systeem- en groepsbeheerders van Workfront kunnen het gebied Campagnes (Beta) toevoegen in het Hoofdmenu van een lay-outsjabloon. Dit maakt het beschikbaar voor alle gebruikers die aan het malplaatje worden toegewezen. Iedereen in Workfront kan een campagne maken nadat deze beschikbaar is.




