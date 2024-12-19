---
navigation-topic: get-started-with-workfront
title: Filter en groepeer uw werk met Prioriteiten
description: Met filters kunt u zoeken naar werk en vervolgens een groep toepassen om de werkruimte te organiseren.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: 8eb9dcaf-bba3-466d-b06d-5383991bc4ea
source-git-commit: 7a6a34ee5b4986137a04d654cf58bfa5f2465715
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Filter en groepeer uw werk met Prioriteiten

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef.</span>

U kunt filters gebruiken om het werk te vinden u zoekt en dan een groepering toepast om het te houden georganiseerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> 
   <p>Huidig: Verzoek of hoger</p>
   <p>Nieuw: Medewerker of hoger</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>Toegang weergeven of bewerken voor het object waarop de update betrekking heeft</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Toegang tot het object weergeven</p></td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter en groepeer uw werk met Prioriteiten in Productie

### Uw werk filteren

U kunt taken en kwesties filtreren die aan u worden toegewezen.

{{step1-to-priorities}}

1. Klik **Filters** in het hoogste recht van de werklijst.
1. Selecteer een of meerdere filters om uw werkitems te beperken.
   ![](assets/filters.png)

+++Uitbreiden om gedetailleerde informatie over beschikbare filters te zien
<table>
  <tbody>
   <tr>
   <th>Filter</th>
   <th>Beschrijving</th>
   </tr>
    <tr>
      <td>eraan werken</td>
      <td>Hiermee geeft u items weer waaraan u momenteel werkt</td>
    </tr>
    <tr>
      <td>Gereed om te starten</td>
      <td>Items weergeven met 
      <ul>
      <li>Geen onvolledige voorgangers of taakbeperkingen</li>
      <p>en</p>
      <li>De geplande begindatum ligt in het verleden of maximaal twee weken in de toekomst</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Niet klaar</td>
      <td>Hiermee geeft u items weer die
       <ul>
      <li>Onvolledige voorgangers of taakbeperkingen die verhinderen dat het item wordt bewerkt</li>
      <p>of</p>
      <li>De geplande begindatum meer dan twee weken in de toekomst</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Gevraagd</td>
      <td>Hier worden problemen weergegeven waaraan u nog niet hebt gewerkt</td>
    </tr>
      <td>Gereed</td>
      <td>Hiermee geeft u werk weer dat in de laatste twee weken is voltooid. Deze filteroptie omvat geen goedkeuringen.</td>
    </tr>
    <tr>
    <td>Project</td>
    <td>De projecten van vertoningen die taken of kwesties bevatten u aan bent toegewezen</td>
    </tr>
    <tr>
    <td>Vervaldatum</td>
    <td>Hiermee wordt het werk weergegeven op de geplande voltooiingsdatum</td>
    </tr>
    <tr>
    <td>Status</td>
    <td>Hiermee geeft u taken of problemen in nieuwe, actieve en volledige status weer</td>
    </tr>
    <tr>
    <td>Mijn focus</td>
    <td>Hiermee worden taken of problemen weergegeven waaraan focusniveaus zijn toegewezen. Focusniveaus worden toegewezen en beheerd door de individuele gebruiker.</td>
    </tr>
  </tbody>
</table>

+++

1. (Facultatief) klik **terug aan gebrek** om uw selectie terug te stellen.

### Uw werk groeperen

{{step1-to-priorities}}

1. Klik **Groepen** in het hoogste recht van de werklijst.
1. Selecteer een groep om uw werklijst te ordenen
   ![](assets/groups.png)

+++Uitbreiden om gedetailleerde informatie over beschikbare groepen te zien

| Groep | Beschrijving |
|-----------|-------------|
| Geen | Hiermee verwijdert u groepen uit de werklijst. |
| Mijn focus | Hiermee worden items gegroepeerd op basis van het focusniveau dat u toewijst. |
| Te betalen week | Deze groepeert items op basis van de week waarin ze verschuldigd zijn. Vervaldata worden bepaald door de geplande afsluitdatum. |
| Status | Deze groepeert items op de volgende statussen: Nieuw, Bezig, Voltooid. <br> Nota: U kunt douanestatus op dit ogenblik niet gebruiken in Prioriteiten. |
| Project | Dit groepeert punten door project. |

+++

### Uw werk sorteren

Om uw werk te sorteren, open **Groep** en klik **Soort oplopend** of **Soort aflopend**.

![](assets/expand-sort-groups.png)

>[!IMPORTANT]
>
>De sorteeroptie is tijdelijk niet beschikbaar als u een groep hebt toegepast.



### Alle secties uitvouwen of samenvouwen

Om alle secties uit te breiden of te doen ineenstorten, open **Groep {en klik** breid allen **uit of** invouwt allen **.**

![](assets/expand-sort-groups.png)

<div class="preview">

## Uw werk filteren en groeperen met Prioriteiten in Voorvertoning

### Uw werk filteren met standaardfilters

U kunt taken en kwesties filtreren die aan u worden toegewezen.

{{step1-to-priorities}}

1. Klik **Filters** in de hoogste linkerzijde van de werklijst.
1. klik **Standaardfilters**.
1. Selecteer een of meerdere filters om uw werkitems te beperken.
   ![](assets/filter-new.png)

+++Uitbreiden om gedetailleerde informatie over beschikbare filters te zien
<table>
  <tbody>
   <tr>
   <th>Filter</th>
   <th>Beschrijving</th>
   </tr>
    <tr>
      <td>eraan werken</td>
      <td>Hiermee geeft u items weer waaraan u momenteel werkt</td>
    </tr>
    <tr>
      <td>Gereed om te starten</td>
      <td>Items weergeven met 
      <ul>
      <li>Geen onvolledige voorgangers of taakbeperkingen</li>
      <p>en</p>
      <li>De geplande begindatum ligt in het verleden of maximaal twee weken in de toekomst</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Niet klaar</td>
      <td>Hiermee geeft u items weer die
       <ul>
      <li>Onvolledige voorgangers of taakbeperkingen die verhinderen dat het item wordt bewerkt</li>
      <p>of</p>
      <li>De geplande begindatum meer dan twee weken in de toekomst</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Gevraagd</td>
      <td>Hier worden problemen weergegeven waaraan u nog niet hebt gewerkt</td>
    </tr>
      <td>Gereed</td>
      <td>Hiermee geeft u werk weer dat in de laatste twee weken is voltooid. Deze filteroptie omvat geen goedkeuringen.</td>
    </tr>
    <tr>
    <td>Project</td>
    <td>De projecten van vertoningen die taken of kwesties bevatten u aan bent toegewezen</td>
    </tr>
    <tr>
    <td>Vervaldatum</td>
    <td>Hiermee wordt het werk weergegeven op de geplande voltooiingsdatum</td>
    </tr>
    <tr>
    <td>Status</td>
    <td>Hiermee geeft u taken of problemen in nieuwe, actieve en volledige status weer</td>
    </tr>
    <tr>
    <td>Mijn focus</td>
    <td>Hiermee worden taken of problemen weergegeven waaraan focusniveaus zijn toegewezen. Focusniveaus worden toegewezen en beheerd door de individuele gebruiker.</td>
    </tr>
  </tbody>
</table>

+++

1. (Facultatief) klik **terug aan gebrek** om uw selectie terug te stellen.

<!--### Filter your work with Smart filters

Use natural language to filter quickly filter work.

{{step1-to-priorities}}

1. Click **Filters** in the top left of the worklist.
1. Click **Smart filters**. 
1. Type how you want to filter your work. 

    You can type things like

    * Show me late tasks
    * Show my top priorities
    * Show work due today

-->

### Uw werk groeperen

{{step1-to-priorities}}

1. Klik **Groepen** in de hoogste linkerzijde van de werklijst.
1. Selecteer een groep om uw werklijst te ordenen
   ![](assets/groups-new.png)

+++Uitbreiden om gedetailleerde informatie over beschikbare groepen te zien

| Groep | Beschrijving |
|-----------|-------------|
| Project | Dit groepeert punten door project. |
| Mijn focus | Hiermee worden items gegroepeerd op basis van het focusniveau dat u toewijst. |
| Te betalen week | Deze groepeert items op basis van de week waarin ze verschuldigd zijn. Vervaldata worden bepaald door de geplande afsluitdatum. |
| Status | Deze groepeert items op de volgende statussen: Nieuw, Bezig, Voltooid. <br> Nota: U kunt douanestatus op dit ogenblik niet gebruiken in Prioriteiten. |

+++



### Uw werk sorteren

**Soort in groepen**

Om uw werk binnen een groep te sorteren, open **Groep** en klik **Soort oplopend** of **Soort aflopend**.

![](assets/sort-in-groups.png)

**de kolommen van de Soort**

Als u afzonderlijke kolommen wilt sorteren, gaat u naar de kolom en klikt u op de pijl omlaag.

![ benedenpijl in kolom ](assets/sort-columns.png)



### Alle groepssecties uitvouwen of samenvouwen

Om alle groepssecties uit te breiden of te doen ineenstorten, open **Groep** en klik **breid allen uit** of **samen allen**.

![](assets/expand-collapse-groups.png)

</div>