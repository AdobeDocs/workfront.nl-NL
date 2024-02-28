---
title: Herinneringsmeldingen instellen
description: Herinneringsmeldingen instellen
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 0%

---

# Herinneringsmeldingen instellen

<!-- Audited: 1/2024 -->

Herinneringsberichten sturen e-mails naar ontvangers op basis van opgegeven criteria. U kunt herinneringsberichten met uw het werkpunten, zoals projecten, taken, kwesties, en timesheets manueel associëren.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard </p>
 <p>of</p> 
<p>Huidig: Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Planner of hoger, met administratieve toegang tot herinneringsmeldingen</p></td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Het e-mailadres voor de herinnering aanpassen

U kunt het onderwerp, de tekst en de HTML aanpassen in het e-mailbericht voor herinneringen.

U kunt ook het standaard-e-mailbericht gebruiken dat bij de herinneringsmelding wordt geleverd. In het standaard-e-mailbericht wordt de naam van het herinneringsbericht gebruikt als het e-mailonderwerp en de objectnaam in de e-mailhoofdtekst, inclusief de gebeurtenis die het bericht heeft geactiveerd.

Als u het e-mailbericht voor een herinnering wilt aanpassen, moet u een e-mailsjabloon maken en dit als bijlage aan het bericht voor een herinnering toevoegen.

Voor informatie over het maken van een e-mailsjabloon raadpleegt u [E-mailsjablonen configureren](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Een herinneringsmelding maken

{{step-1-to-setup}}

1. Klikken **E-mail** > **Meldingen** > **Herinneringsmeldingen**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Klikken **Nieuwe melding voor herinnering**.

1. Klik in de vervolgkeuzelijst op het objecttype dat u wilt koppelen aan de herinneringsmelding.

   Als u bijvoorbeeld een herinneringsbericht aan een tijdspagina wilt koppelen, klikt u op **Tijdschema**.

1. In de **Nieuwe melding voor herinnering** Geef de volgende informatie op in het vak dat wordt weergegeven.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Naam van herinnering</td> 
      <td>Geef een naam op voor de herinneringsmelding.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gekwalificeerde periode</td> 
      <td> <p>Geef het aantal uren, werkdagen, dagen (kalenderdagen), weken of maanden vóór of na de datum in het dialoogvenster <strong>Timing</strong> veld.</p> <p><b>OPMERKING</b>:  
        <ul> 
         <li> <p>Herinneringsmeldingen beginnen 24 uur na de opgegeven datum en zodra aan alle criteria is voldaan.</p> </li> 
         <li> <p>Herinneringsmeldingen voor projecten, taken en uitgaven worden elke avond om middernacht, in de Amerikaanse Mountain Time, geactiveerd. Alle objecten die in aanmerking komen voor een herinneringsmelding vanaf die dag, activeren kort na dat tijdstip een melding aan de aangewezen gebruikers.</p> </li> 
         <li> <p>Herinneringsmeldingen voor tijdbladen worden op de opgegeven tijd verzonden op basis van uw tijdzone en de einddatum, begindatum of laatste updatedatum van het tijdblad.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timing</td> 
      <td> <p>Selecteer de gebeurtenis die het meldingsbericht activeert dat moet worden gepland.</p> <p>Als de herinneringsmelding voor projecten, taken, of kwesties bedoeld is, zijn de beschikbare opties verwant met de Datum van Voltooiing of de Datum van het Begin. In de kennisgeving van de herinnering wordt rekening gehouden met het tijdstempel op de datum van voltooiing en aanvangsdatum van projecten, taken en kwesties.</p>

   <p>Als de herinneringsmelding voor Chronologie bedoeld is, zijn de beschikbare opties verwant met de Datum van het Eind, de Datum van het Begin, of de Laatste Datum van de Update. In de herinneringsmelding voor Timesheets wordt rekening gehouden met de tijdstempel van het tijdbladeinde, het begin en de laatste updatedatum. De tijdpagina begint om middernacht op de dag van de Datum van het Begin (12:00 AM) en beëindigt net vóór middernacht op de Datum van het Eind (11:59 PM).</p>

   <p><b>OPMERKING</b></p>
      <p>Herinneringsmeldingen voor tijdschriften worden slechts om de 24 uur verspreid.</p> <p>Wanneer u binnen een periode van 24 uur meerdere herinneringsmeldingen instelt, stuurt Workfront één e-mailbericht met alle herinneringen die in dat bericht zijn opgenomen.</p>
      <p>Als u bijvoorbeeld drie herinneringsmeldingen configureert om 10 uur vóór, 2 uur vóór en 1 uur vóór een vervaldatum te activeren, worden de drie herinneringen allemaal gecombineerd in dezelfde melding als ze op dezelfde dag voorkomen.</p> <p>Als u echter een herinneringsmelding instelt voor 26 uur vóór en een andere voor 1 uur vóór een vervaldatum, ontvangen gebruikers twee aparte meldingen. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Criteria</td> 
      <td> <p>Selecteer de criteria om de te plannen herinneringsmelding te kwalificeren. Herinneringsmeldingen worden alleen gepland als aan de geselecteerde criteria is voldaan.</p> <p>De volgende opties voor criteria zijn beschikbaar, afhankelijk van het objecttype dat u hebt geselecteerd in Stap 4:</p> 
       <ul> 
        <li><strong>Onvolledig in huidige projecten:</strong> <i>(Beschikbaar voor herinneringen voor taken en uitgaven)</i> De herinneringsmelding wordt alleen verzonden wanneer de objectstatus waaraan de herinneringsmelding is gekoppeld, niet Voltooid is en de projectstatus Huidig is.</li> 
        <li><strong>Alles in huidige projecten:</strong> <i>(Beschikbaar voor herinneringen voor taken en uitgaven)</i> De herinneringsmelding wordt gepland om ongeacht de objecten status en slechts te worden verzonden wanneer de projectstatus waaraan de herinnering bericht wordt geassocieerd Huidig is.</li> 
        <li><strong>Onvolledige projecten:</strong> <i>(Beschikbaar voor herinneringen aan projecten)</i> De herinneringsmelding wordt verzonden wanneer de status van het project om het even wat behalve Voltooid is.</li> 
        <li><strong>Alle projecten:</strong> <i>(Beschikbaar voor herinneringen aan projecten)</i> De herinneringsmelding wordt verzonden ongeacht de projectstatus.</li> 
        <li><strong>Tijdbladen openen:</strong> <i>(Beschikbaar voor herinneringen aan tijdbladen)</i> De melding voor de herinnering wordt verzonden wanneer de status van het tijdschrift Open is.</li> 
        <li><strong>Verzonden tijdbladen:</strong> <i>(Beschikbaar voor herinneringen aan tijdbladen)</i> De herinneringsmelding zal worden verzonden wanneer de timesbladstatus wordt verzonden.</li> 
        <li><strong>Openingstijdschema of minder dan 40 uur per week:</strong> <i>(Beschikbaar voor herinneringen aan tijdbladen)</i> Het herinneringsbericht zal worden verzonden wanneer de timesheet status Open is of wanneer timesheet minder dan 40 geregistreerde uren heeft.</li> 
        <li><strong>E-mailsjabloon:</strong> Selecteer in de vervolgkeuzelijst een e-mailsjabloon die u aan de herinnering wilt toevoegen.<br>Voor informatie over het bouwen van een e-mailsjabloon raadpleegt u <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">E-mailsjablonen configureren</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ontvangers</td> 
      <td>Selecteer de typen gebruikers die u het bericht wilt ontvangen. Maak een keuze uit verschillende objectbelanghebbenden, zoals eigenaar, fiatteur of ontvanger.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.
1. Koppel de herinneringsmelding aan een werkitem, zoals beschreven in [Een herinneringsmelding aan een object koppelen](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Een herinneringsmelding ontvangen

Wanneer aan de voorwaarde is voldaan op het object waaraan de herinneringsmelding is gekoppeld, wordt een e-mailmelding geactiveerd voor de gebruiker die in de herinneringsmelding is gedefinieerd.

Voor meer informatie over het ontvangen van herinneringsberichten, zie [Herinneringsmeldingen](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) sectie in [Adobe Workfront-berichten](../../../workfront-basics/using-notifications/wf-notifications.md).

## Herinneringsmelding testen

Herinneringsmeldingen worden elke avond om middernacht, Mountain Time geactiveerd. Alle objecten die in aanmerking komen voor een herinneringsmelding, activeren kort daarna een melding aan de aangewezen gebruikers.

Als u wilt dat herinneringsberichten handmatig worden geactiveerd, moet eerst aan de voorwaarde voor de herinnering worden voldaan.\
Als een herinnering bijvoorbeeld is ingesteld om een uur na de geplande Voltooiingsdatum van een project te activeren, moet die tijd zijn verstreken tussen het moment waarop de herinnering is ingesteld en nu. Projecten waarvoor de afsluitingsdata waren verstreken voordat de herinnering werd geactiveerd, leiden niet tot een kennisgeving.

Een herinnering handmatig activeren:

{{step-1-to-setup}}

1. Klikken **Systeem** > **Diagnostiek** linksonder in Workfront.

1. Klikken **Herinneringsmeldingen verzenden** en wacht op de bevestiging boven aan het scherm dat ze zijn verzonden.

   De gebruikers die in het herinneringsbericht zijn aangewezen, ontvangen een e-mail.

![](assets/reminder-test.png)