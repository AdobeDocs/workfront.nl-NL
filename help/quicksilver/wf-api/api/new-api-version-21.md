---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 21
description: Adobe Workfront heeft API-versie 21 uitgebracht op 23 oktober 2025. API-versie 21 bevat de volgende wijzigingen ten opzichte van versie 20.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 7166a6b51a45b744a33df697c2bc8080427908a8
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Nieuwe functies in API-versie 21

>[!IMPORTANT]
>
>Deze wijziging in de API-versie heeft een eindwijziging die invloed kan hebben op uw bestaande API-aanroepen. Dit is te wijten aan het feit dat API-versie 21 gebruik maakt van Event Subscriptions versie 2.
>
> Voor velden met meerdere selecties verzendt versie 2 van Event-abonnementen altijd als een array. Versie 1 heeft een array verzonden als er meer dan één waarde is geselecteerd. Als er slechts één waarde is geselecteerd, wordt een tekenreeks verzonden.

Adobe Workfront heeft API-versie 21 uitgebracht op 23 oktober 2025. API-versie 21 bevat de volgende wijzigingen ten opzichte van versie 20.

## Toegevoegde bronnen

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>ID</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>ID</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

## Verwijderde bronnen

### AssignmentBillingRole (ASBLRL)

Het object AssignmentBillingRole en alle bijbehorende velden zijn verwijderd.

## Gewijzigde bronnen

### AccessLevelPermissions (ALVPER)

Een AccessLevelPermissions-object vertegenwoordigt een specifieke machtiging om een Workfront-object te openen, maken of wijzigen. Deze toestemmingen kunnen dan met een Niveau van de Toegang worden geassocieerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> coreAction </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b> forbiddenActions </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> secundairActions </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Als een gebruiker in Workfront geen toegang heeft tot een object dat hij of zij nodig heeft, kan hij of zij toegang tot dat object aanvragen. Het AccessRequest-object vertegenwoordigt deze aanvraag.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> actie </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Een voorwerp AccessRule vertegenwoordigt een regel die in de niveaus van de douanetoegang wordt geplaatst die bepaalt hoe de gebruikers projecten kunnen delen zij tot stand brengen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> coreAction </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b> forbiddenActions </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> secundairActions </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AankondigingBijlage (ANMAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> fileExtension </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b> actualWorkRequiredDouble </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> teamAssignment </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Toewijzing (ASSGN)

Een voorwerp van de Toewijzing vertegenwoordigt de verbinding tussen een het werkpunt en de gebruiker, het team, of de groep die wordt toegewezen om aan het te werken.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> assignBillingRoles </b>
            </p>
            <p>Verwijderd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Categorie (CTGY)

Een object Categorie is een aangepast formulier.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> catObjCode </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b> objTypes </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Klant (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Gebruik van een Java-applet voor tijdlijnberekeningen uitschakelen)
            </p>
            <p>Toegevoegd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Document (DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> getTemporaryCloudURL </b>
            </p>
            <p>Toegevoegd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder

Het object DocumentFolder heeft de markering `RESTORABLE` toegevoegd.

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
            <p><b> getTerejectionCommenttimeCloudURL </b>
            </p>
            <p>De validator toegevoegd <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### OpTask (OPTASK)

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
            <p><b> actualWorkRequiredDouble </b>
            </p>
            <p>Toegevoegd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Parameter (PARAM)

Een object Parameter is een aangepast veld.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> dataType </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (Lexische RTF-tekst)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b> displayType </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Enkele regel omdraaien)</p>
              </li></ul>
         <li>
            <p><b> isActive </b>
            </p>
            <p>Toegevoegd</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standaardvelden</td>
      <td>
        <ul>
         <li>
            <p><b> isActive </b>
            </p>
            <p>Toegevoegd</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PORT)

Een Portfolio-object is een verzameling projecten die concurreren om dezelfde bronnen, meestal geld of mensen om ze te voltooien.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> overrideCurrency </b>
            </p>
            <p>Toegevoegd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Programma (PRGM)

Een programmaobject is een subset van projecten binnen een portfolio, waarin vergelijkbare projecten kunnen worden gegroepeerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> munt </b>
            </p>
            <p>Toegevoegd</p>
              </li>
            </ul>
         </li>
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
            <p><b> actualWorkRequiredDouble </b>
            </p>
            <p>Toegevoegd</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Een voorwerp QueueDef vertegenwoordigt een Rij, die een project is dat aan het gebied van de Desk van de Hulp is gepubliceerd om gebruikers toe te staan om kwesties aan het voor te leggen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> requestorCoreAction </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b> requestForForbiddenActions </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Contactgegevens bewerken)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> helpDeskProjects </b>
            </p>
            <p>Toegevoegd</p>
            </li>
            </ul>
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
            <p><b> localBillingPerHour </b>
            </p>
            <p>Verwijderd</p>
              </li>
          <li>
            <p><b> localCostPerHour </b>
            </p>
            <p>Verwijderd</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Rol (ROLE)

Een object Role (taakrol) vertegenwoordigt een functionele capaciteit of een vaardigheid die een gebruiker zou kunnen opvullen, zoals Designer of Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> met voeten treedt Valuta </b>
            </p>
            <p>Verwijderd</p>
              </li>
          <li>
            <p><b> de Kosten Tarief van de Overschrijving </b>
            </p>
            <p>Verwijderd</p>
              </li>
          <li>
            <p><b> met voeten treden het Facturerings Tarief </b>
            </p>
            <p>Verwijderd</p>
              </li>
      </td>
    </tr>
  </tbody>
</table>

### ScheduledReport (SCHREP)

Een voorwerp ScheduledReport vertegenwoordigt een rapport dat is gevormd om voor levering te gepland.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> formaat </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Een ScoreCardQuestion-object vertegenwoordigt een vraag die aan een Scorecard is toegevoegd. Deze vragen worden gewoonlijk bepaald door de manager van Portfolio, en hun antwoorden staan de manager toe om te begrijpen hoe goed een project zich op de doelstellingen van de portefeuille richt.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> displayType </b>
            </p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Enkele regel omdraaien)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

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
            <p><b> actualWorkRequiredDouble </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> teamAssignment </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Team

Het Team-object heeft de markeringen `DATA_EXTENDIBLE` en `SHARABLE` toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> categoryID </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td>
        <ul>
          <li>
            <p><b> categorie </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objectCategories </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### TemplateAssignment

Het object TemplateAssignment heeft de markering `ATTRIBUTE_ATTACHABLE` toegevoegd.

### Tijdschema (TSHET)

Een voorwerp Timesheet vertegenwoordigt virtuele timecard dat Gebruikers toestaat om werkelijk gewerkte uren voor Taken, Projecten, en de Types van uren van overheaduren in te gaan.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objCode </b>
            </p>
            <p>Verwijderd</p>
              </li>
         </ul>
      </td>
    </tr>
  </tbody>
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
            <p><b> actualWorkRequiredDouble </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> teamAssignment </b>
            </p>
            <p>Toegevoegd</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


