---
product-area: reporting
navigation-topic: reporting-elements
title: Filters, weergaven en groepen verwijderen
description: U kunt een filter, weergave of groep verwijderen uit lijsten en rapporten als u deze hebt gemaakt of als ze met u zijn gedeeld. U kunt standaardfilters, -weergaven of -groepen niet verwijderen.
author: Lisa
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: b56e6591c7da166bd1548420b562b838cc7fe0f2
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Filters, weergaven en groepen verwijderen

<span class="preview">In de voorvertoningsomgeving is de verbeterde filterervaring (voorheen &quot;bèta&quot; genoemd) nu de standaardinstelling. Deze verbeterde filters zijn nu &#39;standaard&#39; en de oudere filterervaring is &#39;verouderd&#39;.</span>

U kunt een filter, weergave of groep verwijderen uit lijsten en rapporten als u deze hebt gemaakt of als ze met u zijn gedeeld. U kunt standaardfilters, -weergaven of -groepen niet verwijderen.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen weergeven of vergroten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Machtigingen weergeven met toegang tot het filter, de weergave of de groep die u wilt verwijderen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een filter, weergave of groep verwijderen met de standaardbuilder

Met de standaardbuilderinterface kunt u een filter, weergave of groepering voor alle lijsten met objecten verwijderen.

### Overwegingen bij het verwijderen van filters, weergaven en groepen

Hoe u een rapporteringselement verwijdert, hangt af van het feit of u het eerst hebt gemaakt of dat het met u is gedeeld.

De volgende scenario&#39;s bestaan wanneer u een groepering verwijdert:

* **Als u de groep hebt gemaakt en u deze verwijdert**, wordt de groepering verwijderd uit het Workfront-systeem. De groepering is niet meer beschikbaar voor gebruikers met wie u deze eerder hebt gedeeld.
* **Als de groep met u is gedeeld en u deze verwijdert**, wordt de groepering alleen voor u verwijderd. De gebruiker die het oorspronkelijk creeerde en om het even welke andere gebruikers het met is gedeeld hebben nog toegang tot de groepering.

### Een filter, weergave of groep verwijderen met de standaardbuilder

1. Ga naar een lijst met objecten of een rapport.
1. (Voorwaardelijk) Klik in een lijst op de knop **Filter**, **Weergave**, of **Groepering** klikt u op de knop **Meer** pictogram ![](assets/more-icon.png)vervolgens **Verwijderen**. Het filter, de weergave of de groep wordt verwijderd.
1. (Voorwaardelijk) Klik in een rapport op de knop **Groepering**, **Filter**, of **Weergave** vervolgkeuzelijst en selecteert u **Groepering verwijderen**, **Filter verwijderen**, of **Weergave verwijderen**.

   De **Mijn groepen**, **Mijn filters,** of **Mijn weergaven** wordt weergegeven.

   Alle rapportelementen die u kunt verwijderen, kunt u verwijderen. Andere rapportelementen worden weergegeven als grijs.

1. Klik op de knop **x** pictogram naast om het even welk rapporteringselement dat u wilt verwijderen.
1. (Voorwaardelijk) Klik **Ja, verwijderen** als u hebt geselecteerd om een filter, weergave of groep te verwijderen die u hebt gemaakt en later met anderen hebt gedeeld. Hiermee verwijdert u het filter, de weergave of de groep uit het Workfront-systeem.

   >[!TIP]
   >
   >Als u een filter, weergave of groep verwijdert die u hebt gemaakt zonder het met anderen te delen, wordt het filter of de groep uit het systeem verwijderd zonder om bevestiging te vragen.

1. Klikken **Gereed**.

## Een filter verwijderen of verwijderen met de bètabuilder

U kunt een filter verwijderen dat met u van lijsten van projecten, taken, of kwesties gebruikend de bèta bouwerinterface werd gedeeld. De bètabuilderinterface is niet beschikbaar voor andere objecten of voor weergaven of groepen.

U kunt filters ook schrappen die u van lijsten van projecten, taken, of kwesties het gebruiken van de bèta bouwerinterface bezit.

Standaardfilters van systeem kunnen niet worden verwijderd of verwijderd.

### Overwegingen bij het verwijderen of verwijderen van filters met de bètabuilder

De volgende scenario&#39;s bestaan wanneer u een filter verwijdert of verwijdert:

* Als het filter met u is gedeeld en u het verwijdert, wordt het filter alleen voor u verwijderd. De gebruiker die het oorspronkelijk creeerde en om het even welke andere gebruikers het met is gedeeld hebben nog toegang tot de filter.
* Als u eigenaar bent van het filter en het verwijdert, wordt het filter verwijderd uit het Workfront-systeem. Het filter is niet meer beschikbaar voor gebruikers met wie u het eerder hebt gedeeld.
* Als u een Workfront-beheerder bent, kunt u het filter verwijderen en het wordt permanent verwijderd voor alle gebruikers, inclusief de eigenaar.

### Een filter verwijderen met de bètabuilder

1. Ga naar een lijst met projecten, taken of problemen.
1. Klik op de knop **Filter** pictogram ![Filterpictogram](assets/filter-nwepng.png) en schakelt u de bètabuilder indien nodig in.
1. Houd de muisaanwijzer boven een filter onder **Gedeeld met mij** klikt u op de knop **Meer** menu ![Meer pictogram](assets/more-icon-spectrum.png)en klik vervolgens op **Verwijderen**.

   ![Filter verwijderen](assets/new-filters-more-menu-remove-filter.png)

1. Selecteren **Verwijderen** in het bevestigingsbericht om het filter permanent te verwijderen.

### Een filter verwijderen met de bètabuilder

1. Ga naar een lijst met projecten, taken of problemen.
1. Klik op de knop **Filter** pictogram ![Filterpictogram](assets/filter-nwepng.png) en schakelt u de bètabuilder indien nodig in.
1. Klik op de knop **Meer** menu ![Meer pictogram](assets/more-icon-spectrum.png)en klik vervolgens op **Verwijderen**.

   ![Filter verwijderen](assets/new-filters-more-menu-options-with-delete.png)

1. (Optioneel) Klik op **Annuleren** op het bevestigingsbericht om te voorkomen dat de filters worden verwijderd en dat de lijst van filters wordt teruggestuurd.
1. Klikken **Verwijderen** op het bevestigingsbericht om de verwijdering te bevestigen.

   Het filter wordt verwijderd voor u en alle gebruikers die hiervoor machtigingen hadden.

