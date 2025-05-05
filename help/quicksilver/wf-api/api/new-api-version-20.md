---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 20
description: Adobe Workfront heeft API-versie 20 uitgebracht op 6 april 2022. API-versie 20 bevat de volgende wijzigingen ten opzichte van versie 19.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# Nieuwe functies in API-versie 20

Adobe Workfront heeft API-versie 20 uitgebracht op 4 mei 2025. API-versie 20 bevat de volgende wijzigingen ten opzichte van versie 19.

## Toegevoegde bronnen

Er zijn geen bronnen toegevoegd voor API-versie 20.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 20

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
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b> forbiddenActions </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b> secundairActions </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
             <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
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
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b> forbiddenActions </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b> secundairActions </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
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
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLabourCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>billedRevenue</li>
              <li>begroting</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLabourCost</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>SchedulBenefit</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost</li>
              <li>SchedulExpenseCost</li>
              <li>scheduledLabourCost</li>
              <li>SchedulNonBillableExpenseCost</li>
              <li>scheduledRiskCost</li>
              <li>scheduledValue</li>
              <li>resterendeKosten</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>scheduledCost</li>
          <li>scheduledRevenue</li>
          </ul>
          </li>
          <li><p><b>scheduledDuration</b></p> <p>De markeringen <code>DYNAMIC</code>, <code>LAZY_READ</code> en <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>De markering toegevoegd <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>De mogelijke waarde <code>URH</code> (Uur gebruiker en Rol) toegevoegd </li>
          <li><p><b>RevenusType</b></p> <p>De mogelijke waarden <code>URH</code> (User and Role Hourly), <code>URC</code> (User and Role Hourly w/Cap) en <code>URF</code> (User and Role Hourly Plus Fixed) zijn toegevoegd.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
          <p>De volgende velden zijn toegevoegd:</p>
             <ul>
              <li><b>factureringstarieven</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Toewijzing (ASSGN)

Een voorwerp van de Toewijzing vertegenwoordigt de verbinding tussen een het werkpunt en de gebruiker, het team, of de groep die wordt toegewezen om aan het te werken.

Het toewijzingsobject heeft de markeringen `ATTRIBUTE_ATTACHABLE` en `DOMAIN_EXTENDABLE` toegevoegd.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### Avatar

Een Avatar-object is een gebruikersfoto.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> attachedObjectCode </b>
            </p>
             <p>Toegevoegd</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> attachedObjectCode </b>
            </p>
             <p>Toegevoegd</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Bewerkingen</td>
      <td>
        <ul>
          <li>
            <p><b> KOPIËREN </b>
            </p>
             <p>Toegevoegd</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

### Basislijn (BLIN)

Basislijnen zijn momentopnamen van hoe de prestaties van een project er op een bepaald moment uitzagen. Ze slaan belangrijke informatie over het project op, zoals belangrijke data, voortgang, kosten en inkomstenwaarden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>begroting</li>
              <li>eac</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost</li>
              <li>SchedulNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>scheduledCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>De markering toegevoegd <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BaselineTask (BSTSK)

Basislijnen zijn momentopnamen van hoe de prestaties van een project er op een bepaald moment uitzagen. Ze slaan belangrijke informatie over het project op, zoals belangrijke data, voortgang, kosten en inkomstenwaarden. Wanneer u een basislijn maakt, worden de taakgegevens ook vastgelegd op de basislijntaken van die basislijn.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost</li>
              <li>SchedulNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>scheduledCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>De markering toegevoegd <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Factureringsrecord (BILL)

Een object BillingRecord registreert de inkomsten, uren of kosten die in rekening kunnen worden gebracht. Deze informatie kan worden gebruikt om facturen op te stellen in een extern boekhoudsysteem.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>bedrag</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Toegevoegd</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

### CategorieParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> configuraties </b>
            </p>
             <p>Toegevoegd</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Bedrijf (CMPY)

Een object Company vertegenwoordigt een organisatie die bestaat uit een verzameling personen.

Het object Company heeft de vlag `SHARABLE` toegevoegd.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (enkelvoudig ondertekeningsschema)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissuesMove)</p></li>
            </ul>
          </li>
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
      <td>
           <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>tarief</li>
      </td>
    </tr>
  </tbody>
</table>


### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixedRevenue</li>
              <li>actualLabourCost</li>
              <li>actualLabourCostHours</li>
              <li>actualLabourRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>fixedCost</li>
              <li>scheduledBillableExpenseCost</li>
              <li>SchedulExpenseCost</li>
              <li>SchedulFixedRevenue</li>
              <li>scheduledLabourCost</li>
              <li>SchedulLabourCostHours</li>
              <li>SchedulLabourRevenue</li>
              <li>SchedulNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLabourCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

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
            <p><b> munt </b>
            </p>
             <p>Toegevoegd</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
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
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Toegevoegd</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

Een voorwerp OpTask is algemeen genoemd als Kwestie. Een kwestie is een het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Een probleem kan ook een verzoek van de Helpdesk zijn. Wijzigingsorders, verzoeken en bugs zijn ook problemen.

Het OpTask-object heeft de markering DOMAIN_EXTENDABLE toegevoegd

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualCost</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
              <li>actualCost</li>
          </ul>
          </li>
        </ul>
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
            <p><b> displayType </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (Interne opzoekopdracht)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Intern opzoeken door meerdere selecties)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio (PORT)

Een Portfolio-object is een verzameling projecten die concurreren om dezelfde bronnen, meestal geld of mensen om ze te voltooien.

Het Portfolio-object heeft de markering `DOMAIN_EXTENDABLE` toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>uitgelijnd</li>
              <li>begroting</li>
              <li>valuta</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Programma (PRGM)

Een programmaobject is een subset van projecten binnen een portfolio, waarin vergelijkbare projecten kunnen worden gegroepeerd.

Het programmaobject heeft de markering `DOMAIN_EXTENDABLE` toegevoegd.

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
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLabourCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>billedRevenue</li>
              <li>begroting</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLabourCost</li>
              <li>eac</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>SchedulBenefit</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost</li>
              <li>SchedulExpenseCost</li>
              <li>scheduledLabourCost</li>
              <li>SchedulNonBillableExpenseCost</li>
              <li>scheduledRevenue</li>
              <li>scheduledRiskCost</li>
              <li>scheduledValue</li>
              <li>resterendeKosten</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>scheduledCost</li>
          <li>scheduledRevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>De markering toegevoegd <code>CURRENCY</code></li>
        </ul>
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
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b> requestForForbiddenActions </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Verwijderen uit aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Subprojecten toevoegen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Tarief (SNELHEID)

Een object Rate vertegenwoordigt een factureringssnelheid in Workfront.

Het object Rate heeft de markering `ATTRIBUTE_ATTACHABLE` toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>De volgende velden zijn toegevoegd:
          <ul>
          <li>valuta</li>
          <li>vergrendeld</li>
          <li>type</li>
          <li>value</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rol (ROLE)

Een object Role (taakrol) vertegenwoordigt een functionele capaciteit of een vaardigheid die een gebruiker zou kunnen opvullen, zoals Designer of Product Manager.

Het object Role heeft de markering `DOMAIN_EXTENDABLE` toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>factureringPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
          <p>De volgende velden zijn toegevoegd:
          <ul>
          <li>factureringstarieven</li>
          <li>costRates</li>
          </ul>
          </li>
        </ul>
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
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Een ScoreCardQuestion-object vertegenwoordigt een vraag die aan een Scorecard is toegevoegd. Deze vragen worden gewoonlijk bepaald door de manager van Portfolio, en hun antwoorden staan de manager toe om te begrijpen hoe goed een project zich op de doelstellingen van de portefeuille richt.

<table>
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
             <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li><p><code>INTRNL</code> (Interne opzoekopdracht)</p></li>
              <li><p><code>MULTINTRNL</code> (Intern opzoeken door meerdere selecties)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Taak (TASK)

Een voorwerp van de Taak vertegenwoordigt een het werkpunt dat als stap naar het bereiken van een definitief doel (het voltooien van een Project) moet worden uitgevoerd.

Het object Task heeft de markering `DOMAIN_EXTENDABLE` toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLabourCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost/li&gt;
              <li>SchedulExpenseCost</li>
              <li>scheduledLabourCost</li>
              <li>SchedulNonBillableExpenseCost</li>
              <li>scheduledRevenue</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>scheduledCost</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>De volgende mogelijke waarden zijn toegevoegd:<ul><li><code>URH</code> (Uur gebruiker en rol)</li></ul></li>
          <li><p><b>RevenusType</b></p> <p>De volgende mogelijke waarden zijn toegevoegd:<ul><li><code>URH</code> (Uur gebruiker en rol)</li><li><code>URC</code> (Uur gebruiker en rol met uiteinde)</li><li><code>URF</code> (Gebruiker en Rol Uur plus Vast)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Sjabloon (TMPL)

Een voorwerp van het Malplaatje vertegenwoordigt een patroon voor een project. Projecten kunnen worden gemaakt op basis van sjablonen om tijd te besparen. Een malplaatje bevat een team en taken, die aan om het even welk project zullen worden gekopieerd dat van het malplaatje wordt gecreeerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>begroting</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>SchedulBenefit</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost</li>
              <li>SchedulExpenseCost</li>
              <li>scheduledLabourCost</li>
              <li>SchedulNonBillableExpenseCost</li>
              <li>scheduledRevenue</li>
              <li>scheduledRiskCost</li>
              <li>workRequired</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>scheduledCost</li>
          <li>scheduledRevenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
          <p>De volgende velden zijn toegevoegd:</p>
             <ul>
              <li><b>factureringstarieven</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateTask (TTSK)

Een voorwerp TemplateTask vertegenwoordigt een Taak die deel van een Malplaatje uitmaakt. De Taken van het malplaatje worden Taken in het Project waar het Malplaatje wordt gebruikt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>factureringsbedrag</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost/li&gt;
              <li>SchedulExpenseCost</li>
              <li>scheduledLabourCost</li>
              <li>SchedulNonBillableExpenseCost</li>
              <li>scheduledRevenue</li>
              <li>RevenusType</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>scheduledCost</li>
          <li>scheduledRevenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>De volgende mogelijke waarden zijn toegevoegd:<ul><li><code>URH</code> (Uur gebruiker en rol)</li></ul></li>
          <li><p><b>RevenusType</b></p> <p>De volgende mogelijke waarden zijn toegevoegd:<ul><li><code>URH</code> (Uur gebruiker en rol)</li><li><code>URC</code> (Uur gebruiker en rol met uiteinde)</li><li><code>URF</code> (Gebruiker en Rol Uur plus Vast)</li></ul></li>
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
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objCode </b>
            </p>
             <p>Verwijderd</p>
          </li>
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
            <p><b> updateType </b>
            </p>
             <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gebruiker (GEBRUIKER)

Een object User vertegenwoordigt een persoon met een account in Workfront die zich kan aanmelden en met het systeem kan communiceren.

Het gebruikersobject heeft de velden `ATTRIBUTE_ATTACHABLE` en `DOMAIN_EXTENDABLE` toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>factureringPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
          <p>De volgende velden zijn toegevoegd:</p>
             <ul>
              <li><b>factureringstarieven</b></li>
              <li><b>costRates</b></li>
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
            <p>In de volgende velden is de markering toegevoegd <code>RESTRICTABLE</code> :
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLabourCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>scheduledCost</li>
              <li>SchedulExpenseCost</li>
              <li>scheduledLabourCost</li>
              <li>SchedulNonBillableExpenseCost</li>
              <li>scheduledRevenue</li>
            </ul>
          </li>
          <li>
          <p>Het type van de volgende velden is gewijzigd van <code>double</code> in <code>class java.math.BigDecimal</code> :
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>scheduledCost</li>
          <li>scheduledRevenue</li>
          </ul>
          </li>
          <li><p><b>scheduledDuration</b></p> <p>De markeringen <code>DYNAMIC</code>, <code>LAZY_READ</code> en <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>De markering toegevoegd <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>De mogelijke waarde <code>URH</code> (Uur gebruiker en Rol) toegevoegd </li>
          <li><p><b>RevenusType</b></p> <p>De mogelijke waarden <code>URH</code> (User and Role Hourly), <code>URC</code> (User and Role Hourly w/Cap) en <code>URF</code> (User and Role Hourly Plus Fixed) zijn toegevoegd.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



