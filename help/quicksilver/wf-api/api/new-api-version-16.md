---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 16
description: Adobe Workfront heeft API-versie 16 uitgebracht op 6 april 2022. API-versie 16 bevat de volgende wijzigingen ten opzichte van versie 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: acd1fe5500776b8f16c67b05048a88d0c8107079
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# Nieuwe functies in API-versie 16

Adobe Workfront heeft API-versie 16 uitgebracht op 6 april 2023. API-versie 16 bevat de volgende wijzigingen ten opzichte van versie 15.

## Toegevoegde bronnen

Er zijn geen bronnen toegevoegd voor API-versie 16.

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 16

## Gewijzigde bronnen

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Goedkeuring (goedkeuring)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Uur (UUR)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [Opmerking (OPMERKING)](#note-note)
* [OpTask/Issue (OPTASK)](#note-note)
* [Project (PROJ)](#project-proj)
* [Tarief (SNELHEID)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Rol/Taakrol (ROLE)](#role--job-role-role)
* [Taak (TASK)](#task-task)
* [Tijdschema (TSHET)](#timesheet-tshet)
* [UIFilter / Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Grouping (UIGB)](#uigroupby--grouping-uigb)
* [UIView/View (UIVW)](#uiview--view-uivw)
* [Gebruiker (GEBRUIKER)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

### Goedkeuring (goedkeuring)

Een bepaald het werkpunt, zoals een taak, een document, of een timesheet, kunnen vereisen dat een supervisor of een andere gebruiker weg op het het werkpunt ondertekent. Een voorwerp van de Goedkeuring vertegenwoordigt de actie van het ondertekenen van op een het werkpunt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> workPerDate </b>
            </p>
            <p>Dit veld is toegevoegd en bevat het aantal minuten werk per dag dat u moet doen. De notatie heeft de notatie <code>YYYY-MM-DD: (number of minutes)</code> en er wordt rekening gehouden met de tijdzone.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Toewijzing (ASSGN)

Een toewijzingsobject vertegenwoordigt de verbinding tussen een werkitem en de gebruiker, het team of de groep die is toegewezen aan het werken eraan.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> workPerDate </b>
            </p>
            <p>Dit veld is toegevoegd en bevat het aantal minuten werk per dag dat u moet doen. De notatie heeft de notatie <code>YYYY-MM-DD: (number of minutes)</code> en er wordt rekening gehouden met de tijdzone.</p>
          </li>
          <li>
            <p><b> isContouren </b>
            </p>
            <p>Dit veld is toegevoegd en is een Booleaanse waarde die aangeeft of de toewijzing contouren heeft. Als de toewijzingsminuten per dag zijn bewerkt in Workload Balancer, is de toewijzing contouren.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

Het object CustomEnum helpt bij het omzetten van statuscodes in leesbare tekst.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### CustomerPreferences (CUSTPR)

Een object CustomerPreferences vertegenwoordigt de set voorkeuren die een klant heeft ingesteld voor hun exemplaar van Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> naam </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> getIsAutoUpgradeDisabled </b>
            </p>
            <p>Deze actie retourneert een Booleaanse waarde die aangeeft of de klant de optie voor het automatisch upgraden van de Contributor-licentienemers heeft uitgeschakeld.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

Een object ExternalSection is een externe webpagina die is ingesloten in een Workfront-rapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">handelingen</td>
      <td>
        <ul>
           <li>
            <p><b> calculateIframeURL </b>
            </p>
            <p>Dit is toegevoegd en berekent de URL van een iFrame dat is ingesloten in een rapport.</p>
         </li>
          <li>
            <p><b> calculateIframeURLS </b>
            </p>
            <p>Dit is toegevoegd en berekent de URL's van iFrames die zijn ingesloten in een rapport.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Uur (UUR)

Een voorwerp van het Uur vertegenwoordigt een uur dat door een gebruiker op timesheet wordt geregistreerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> timesheetHourIdentifier </b>
            </p>
            <p>Toegevoegd. Deze parameter wordt gebruikt om de uren te identificeren die met <code>batchSave</code> worden gecreeerd. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Opmerking (OPMERKING)

Een object Note is een opmerking of update die op een Workfront-object wordt uitgevoerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> attachedDocuments </b>
            </p>
            <p>Dit veld is toegevoegd en vertegenwoordigt een lijst met documenten die aan de opmerking zijn toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask/Issue (OPTASK)

Een voorwerp OpTask is algemeen genoemd als Kwestie. Een kwestie is een het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Een probleem kan ook een verzoek van de Helpdesk zijn. Wijzigingsorders, verzoeken en bugs zijn ook problemen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> workPerDate </b>
            </p>
            <p>Dit veld is toegevoegd en bevat het aantal minuten werk per dag dat u moet doen. De notatie heeft de notatie <code>YYYY-MM-DD: (number of minutes)</code> en er wordt rekening gehouden met de tijdzone.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">handelingen</td>
      <td>
        <ul>
           <li>
            <p><b> assignMultiple </b>
            </p>
            <p>Met deze actie voegt u het veld <code>teamIDs</code> toe ter ondersteuning van de functionaliteit om meerdere teams toe te wijzen aan een taak of uitgave.</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Project (PROJ)

Projecten zijn werkitems binnen Workfront en vormen een belangrijke bouwsteen voor de manier waarop Workfront mensen helpt om te werken. Een voorwerp van het Project vertegenwoordigt een groep taken met een gemeenschappelijk, specifiek doel.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> resourcePlannerBudgetedHours </b>
            </p>
            <p>Dit veld is toegevoegd en vertegenwoordigt de som van alle begrote uren uren voor het project.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tarief (SNELHEID)

Een object Rate vertegenwoordigt een factureringssnelheid in Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Deze parameters zijn verplaatst naar het object Rate van het object Role, zodat de objecten Role en User meerdere waarden kunnen hebben (voor afzonderlijke datumbereiken).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Deze parameters vertegenwoordigen de id en de objectcode van het object waaraan de Snelheid is gekoppeld.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>Deze handeling is toegevoegd en koppelt objecten Rate aan het opgegeven object. Dit eindpunt werkt voor alle voorwerpen van het Tarief Bijvoegbaar.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Een RichTextNote-object is een opmerking of update die wordt gemaakt voor een Workfront-object en die opgemaakte tekst, zoals vette of cursieve tekst, bevat.

Het RichTextNote-object heeft de markering `REPORTABLE` verwijderd.

### Rol/Taakrol (ROLE)

Een object Role (taakrol) vertegenwoordigt een functionele capaciteit of een vaardigheid die een gebruiker zou kunnen opvullen, zoals Designer of Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
           <li>
            <p><b> tarieven </b>
            </p>
            <p>Dit is toegevoegd en vertegenwoordigt de objecten Rate die aan deze rol zijn gekoppeld.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Taak (TASK)

Een voorwerp van de Taak vertegenwoordigt een het werkpunt dat als stap naar het bereiken van een definitief doel (het voltooien van een Project) moet worden uitgevoerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> workPerDate </b>
            </p>
            <p>Dit veld is toegevoegd en bevat het aantal minuten werk per dag dat u moet doen. De notatie heeft de notatie <code>YYYY-MM-DD: (number of minutes)</code> en er wordt rekening gehouden met de tijdzone.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">handelingen</td>
      <td>
        <ul>
           <li>
            <p><b> assignMultiple </b>
            </p>
            <p>Met deze actie voegt u het veld <code>teamIDs</code> toe ter ondersteuning van de functionaliteit om meerdere teams toe te wijzen aan een taak of uitgave.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Tijdschema (TSHET)

Een voorwerp Timesheet vertegenwoordigt virtuele timecard dat Gebruikers toestaat om werkelijk gewerkte uren voor Taken, Projecten, en de Types van uren van overheaduren in te gaan.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
           <li>
            <p><b> availableActions </b>
            </p>
            <p>Deze parameter heeft de markering <code>READ_ONLY</code> verwijderd.</p>
         </li>
           <li>
            <p><b> isEditable </b>
            </p>
            <p>Deze parameter heeft de markering <code>READ_ONLY</code> verwijderd.</p>
         </li>
           <li>
            <p><b> totalDays </b>
            </p>
            <p>Deze parameter werd toegevoegd, en slaat timesheets duur in dagen ongeacht veranderingen in "Equivalent Uren voor Volledige Workday." op  Als Equivalent Hours bijvoorbeeld is ingesteld op 6 en één dag wordt geregistreerd, wordt Equivalent Hours gewijzigd in 8 uur. <code>totalDays</code> heeft nog steeds de waarde 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> addJoinForNullableFields </b>
            </p>
            <p>Deze handeling is toegevoegd en er wordt een filterquerykaart aan toegevoegd en de <code>allowingnull</code> join voor velden die kunnen worden geannuleerd, wordt toegevoegd.</p>
         </li>
         <li>
            <p><b> disableSystemWideVisibility
</b>
            </p>
            <p><b> enableSystemWideVisibility </b>
            </p>
            <p>Deze acties ondersteunen de mogelijkheid om filters, weergaven en groepen in het hele systeem te delen.</p><p>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/nl/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E"> filters, meningen, of groeperingen van de Merk beschikbaar aan alle gebruikers </a> maken.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> disableSystemWideVisibility
</b>
            </p>
            <p><b> enableSystemWideVisibility </b>
            </p>
            <p>Deze acties ondersteunen de mogelijkheid om filters, weergaven en groepen in het hele systeem te delen.</p><p>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/nl/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E"> filters, meningen, of groeperingen van de Merk beschikbaar aan alle gebruikers </a> maken.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView/View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> layoutType </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> disableSystemWideVisibility
</b>
            </p>
            <p><b> enableSystemWideVisibility </b>
            </p>
            <p>Deze acties ondersteunen de mogelijkheid om filters, weergaven en groepen in het hele systeem te delen.</p><p>Voor meer informatie, zie <a href="https://experienceleague.adobe.com/nl/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E"> filters, meningen, of groeperingen van de Merk beschikbaar aan alle gebruikers </a> maken.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Gebruiker (GEBRUIKER)

Een object User vertegenwoordigt een persoon met een account in Workfront die zich kan aanmelden en met het systeem kan communiceren.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
           <li>
            <p><b> tarieven </b>
            </p>
            <p>Dit is toegevoegd en vertegenwoordigt de objecten Rate die aan deze gebruiker zijn gekoppeld.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Een object UserNote is een melding.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Zoekopdrachten</td>
      <td>
        <ul>
          <li>
            <p><b> myAllObjectTypesUnreadNotifications </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Werken (WERKEN)

Een voorwerp van het Werk is een gemeenschappelijke interface die zowel Taak als OpTask erft, en gemeenschappelijke code tussen twee deelt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> workPerDate </b>
            </p>
            <p>Dit veld is toegevoegd en bevat het aantal minuten werk per dag dat u moet doen. De notatie heeft de notatie <code>YYYY-MM-DD: (number of minutes)</code> en er wordt rekening gehouden met de tijdzone.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
