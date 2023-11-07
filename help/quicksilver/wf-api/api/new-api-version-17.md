---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 17
description: Adobe Workfront heeft API-versie 17 uitgebracht op 6 april 2022. API-versie 17 bevat de volgende wijzigingen ten opzichte van versie 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 0%

---

# Nieuwe functies in API-versie 17

Adobe Workfront heeft API-versie 17 uitgebracht op 12 oktober 2023. API-versie 17 bevat de volgende wijzigingen ten opzichte van versie 16.

## Toegevoegde bronnen

<!--

### Booking (BOOKNG)

-->

### ExternalDocument (EXTDOC)

Een object ExternalDocument is een document of ander digitaal element dat zich in een externe documentopslagprovider bevindt. Deze activa kunnen aan en van Workfront worden gekoppeld.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>beschrijving</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>text</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>pad</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>miniatuurURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>beschrijving</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>text</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>pad</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>miniatuurURL</b></p></li>
          <li><p><b>value</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standaardvelden</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Zoekopdrachten</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Bewerkingen</td>
      <td>
        <ul>
          <li><p><b>ZOEKEN</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td>
        <ul>
          <li><p><b>klant</b></p></li>
          <li><p><b>user</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 17

## Gewijzigde bronnen

De volgende bronnen zijn gewijzigd voor API-versie 17.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Basislijn (BLIN)

Basislijnen zijn momentopnamen van hoe de prestaties van een project er op een bepaald moment uitzagen. Ze slaan belangrijke informatie over het project op, zoals belangrijke data, voortgang, kosten en inkomstenwaarden.

Het object Baseline heeft de markering verwijderd **INLINE_EDITABLE**.

### Factureringsrecord (BILL)

Een object BillingRecord registreert de inkomsten, uren of kosten die in rekening kunnen worden gebracht. Deze informatie kan worden gebruikt om facturen op te stellen in een extern boekhoudsysteem.

Het object BillingRecord heeft de vlag verwijderd **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Bedrijf (CMPY)

Een object Company vertegenwoordigt een organisatie die bestaat uit een verzameling personen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Verwijderd</p>
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
            <p><b>name</b>
            </p>
            <p>De mogelijke waarde "config.defaultToNewHomeDescription" (customer:config.defaultToNewHome)&gt;/p? toegevoegd?<p>Hierdoor kan een organisatie de nieuwe Home-ervaring als standaard voor haar gebruikers instellen.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Een object DocumentVersion vertegenwoordigt een specifieke versie van een bestand (zoals geschreven materiaal, afbeeldingen of andere vormen van informatie).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>De mogelijke waarde Frame.io (FRAMEIO) is toegevoegd</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>De mogelijke waarde "enum.filetype.site" (site) toegevoegd</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRATE)

Een ExchangeRate-object vertegenwoordigt een wisselkoers die in Workfront is ingesteld. ExchangeRate-objecten zijn niet dynamisch.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>De volgende velden zijn toegevoegd:
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>Toegevoegd.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kosten (EXPNS)

De kosten vertegenwoordigen de niet-loonkosten die tijdens de looptijd van een project kunnen worden gemaakt.

Het object Expense heeft de markering verwijderd **INLINE_EDITABLE**.

### Groep (GROEP)

Een object Group vertegenwoordigt een set gebruikers en teams. Groepen vertegenwoordigen vaak de afdelingsstructuur.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Verwijderd</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Uur (UUR)

Een voorwerp van het Uur vertegenwoordigt een uur dat door een gebruiker op timesheet wordt geregistreerd.

Het object Hour heeft de markering verwijderd **INLINE_EDITABLE**.

### Iteratie (ITRN)

Een Iteration-object vertegenwoordigt één Agile Iteration. Herhalingen zijn discrete tijdsperiodes die worden gebruikt om artikelen van het type Agile te plannen en te voltooien.

Het object Iteration heeft de markering verwijderd **INLINE_EDITABLE**.


### JournalEntry (JRNLE)

Het object JournalEntry kan worden ingesteld om informatie over specifieke objectvelden te registreren wanneer deze velden worden gewijzigd. Wanneer een gebied opstelling is om als deel van het voorwerp van de Ingang van het Dagboek worden geregistreerd, zal een overeenkomstig Ingang van het Dagboek worden gecreeerd telkens als dat gebied wordt gewijzigd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>Toegevoegde fiatteur</li>
              <li>Toegevoegde revisor (AAR)</li>
              <li>Verwijderde revisor (ARR)</li>
              <li>Verwijderd fiatteur (ARA)</li>
              <li>Besluit goedgekeurd (ADA)</li>
              <li>Met wijzigingen goedgekeurd besluit (ADC)</li>
              <li>Beslissingsbehoeften (ADN)</li>
              <li>Besluit ingetrokken (ADR)</li>
              <li>Gewijzigde fiatteur (AAC)</li>
              <li>Revisor gewijzigd (ARC)</li>
              <li>Evaluatie voltooid (RDC)</li>
              <li>Herziening ingetrokken (RDR)</li>
              <li>Publiceren (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban Board (KNBNBD)

Een Kanban-bord wordt gebruikt om taken in een behendige omgeving bij te houden.

Het Kanban Board-object heeft de vlag verwijderd **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

Een object LinkedFolder vertegenwoordigt een map die is gekoppeld vanuit een externe documentprovider, zoals Google Drive of Dropbox.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Toegevoegde mogelijke waarde "Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask/Issue (OPTASK)

Een voorwerp OpTask is algemeen genoemd als Kwestie. Een kwestie is een het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Een probleem kan ook een verzoek van de Helpdesk zijn. Wijzigingsorders, verzoeken en bugs zijn ook problemen.

Het object Issue heeft de vlag verwijderd **INLINE_EDITABLE**.

### Project (PROJ)

Projecten zijn werkitems binnen Workfront en vormen een belangrijke bouwsteen voor de manier waarop Workfront mensen helpt om te werken. Een voorwerp van het Project vertegenwoordigt een groep taken met een gemeenschappelijk, specifiek doel.

Het object Project heeft de vlag verwijderd **INLINE_EDITABLE**.

### ProjectUser (PRTU)

Een voorwerp ProjectUser vertegenwoordigt een gebruiker verbonden aan een specifiek project.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Tarief (SNELHEID)

Een object Rate vertegenwoordigt een factureringssnelheid in Workfront.

Het object Rate heeft de markering verwijderd **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>De volgende acties zijn toegevoegd aan de functionaliteit van de kaart van het tarief:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>De <b>setRatesForRole</b> Actie is gewijzigd om de volgende velden toe te voegen:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risico (RISICO)

Een object Risk vertegenwoordigt een mogelijke gebeurtenis die kan voorkomen dat een project op tijd of binnen het budget wordt voltooid. Er worden in de planningsfase risico&#39;s toegevoegd aan projecten om potentiële obstakels te identificeren voordat eventuele werkzaamheden worden goedgekeurd.

Het object Risk heeft de markering verwijderd **INLINE_EDITABLE**.

### Rol/Taakrol (ROLE)

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
            <p><b>defaultInterface</b>
            </p>
            <p>Verwijderd</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Taak (TASK)

Een voorwerp van de Taak vertegenwoordigt een het werkpunt dat als stap naar het bereiken van een definitief doel (het voltooien van een Project) moet worden uitgevoerd.

Het taakobject heeft de markering verwijderd **INLINE_EDITABLE**.

### Team (TEAMOB)

Een voorwerp van het Team is een inzameling van Gebruikers die aan een het werkpunt kunnen worden toegewezen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Verwijderd</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember (TEAMMB)

Een voorwerp TeamMember is een gebruiker verbonden aan een specifiek team.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
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
            <p><b>objCode</b>
            </p>
            <p>Verwijderd</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Bijwerken (UPDATE)

Werkonderdelen in Workfront kunnen worden bijgewerkt om gebruikers op de hoogte te houden van de huidige status. Een object Update vertegenwoordigt een van deze updates. Updates kunnen door gebruikers worden ingevoerd of door het Workfront-systeem worden gemaakt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>De volgende waarden zijn toegevoegd:</p>
            <ul>
              <li>Toegevoegde fiatteur (assetapprovalAddApprover)</li>
              <li>Toegevoegde revisor (assetapprovalAddReviewer)</li>
              <li>Verwijderd fiatteur (assetapprovalRemoveApprover)</li>
              <li>Verwijderde revisor (assetapprovalRemoveReviewer)</li>
              <li>Goedgekeurd besluit (goedkeuringGoedgekeurdBesluit)</li>
              <li>Beslissingsbehoeften werk (assetapprovalDecisionNeedsWork)</li>
              <li>Besluit goedgekeurd met wijzigingen (assetapprovalDecisionApprovedChanges)</li>
              <li>Ingetrokken beschikking (assetapprovalDecisionRevoked)</li>
              <li>Gewijzigde fiatteur (assetapprovalApproverChanged)</li>
              <li>Revisor is gewijzigd (assetapprovalReviewerChanged)</li>
              <li>Revisie voltooid (assetapprovalReviewerDecisionComplete)</li>
              <li>Herziening ingetrokken (assetapprovalReviewerDecisionRevoked)</li>
              <li>Fout bij verzenden van extern document (externalDocumentSendError)</li>
              <li>Gepubliceerde documentversie (documentVersionPublish)</li>
              <li>Workflow voor gekoppelde mappen (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Gebruiker (GEBRUIKER)

Een object User vertegenwoordigt een persoon met een account in Workfront die zich kan aanmelden en met het systeem kan communiceren.

Het object User heeft de markering verwijderd **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>Dit gebied is toegevoegd, en is een aantal tussen 0 en 1 dat het percentage van tijd vertegenwoordigt dat een gebruiker aan projectwerk (niet-overheadwerk) elke dag kan uitgeven. De waarde 1 betekent dat de gebruiker 100% van zijn tijd aan projectwerk kan doorbrengen.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Gebruikersgroepen (USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserNote (USRNOT)

Een object UserNote is een melding.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>De volgende waarden zijn toegevoegd:</p>
            <ul>
              <li>Document vereist uw goedkeuring (AAA)</li>
              <li>Document moet worden gecontroleerd (AAR)</li>
              <li>Document heeft uw goedkeuring niet meer nodig (ARA)</li>
              <li>Document heeft uw revisie niet meer nodig (ARR)</li>
              <li>Voor het document is goedkeuring (ATA) vereist</li>
              <li>Document moet (door gebruiker) worden gecontroleerd (ATR)</li>
              <li>Document is niet langer vereist (goedkeuring door gebruiker)</li>
              <li>Document hoeft niet langer te worden gecontroleerd (door gebruiker)</li>
              <li>Document goedgekeurd (ADA)</li>
              <li>Document goedgekeurd met wijzigingen (ADC)</li>
              <li>Document vereist werk (ADN)</li>
              <li>(Gebruiker) heeft gemarkeerd (document) als goedgekeurd. Uw goedkeuring is niet meer nodig. (AAN)</li>
              <li>(Gebruiker) heeft gemarkeerd (document) als goedgekeurd met wijzigingen. Uw goedkeuring is niet meer nodig. (ACN)</li>
              <li>(Gebruiker) heeft gemarkeerd (document) als het werk dat nodig is. Uw goedkeuring is niet meer nodig. (AWN)</li>
              <li>Uw revisie is nu nodig in plaats van goedkeuring (AAC)</li>
              <li>Het document heeft nu uw goedkeuring nodig in plaats van een revisie (ADN)</li>
              <li>Gereviseerd document (RDC)</li>
              <li>Gereviseerd document (TRC)</li>
              <li>(Gebruiker) heeft (document) gecontroleerd als voltooid. Je beoordeling is niet meer nodig. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
