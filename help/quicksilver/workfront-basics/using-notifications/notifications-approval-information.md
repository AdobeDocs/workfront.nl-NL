---
content-type: reference
navigation-topic: notifications
title: 'Meldingen: goedkeuringsgegevens'
description: In de volgende berichten wordt u gewaarschuwd voor goedkeuringsactiviteiten voor een onderdeel dat u gebruikt. Zie Uw eigen e-mailmeldingen wijzigen voor informatie over het configureren van de berichten die u ontvangt.
author: Courtney
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Meldingen: goedkeuringsgegevens

In de volgende berichten wordt u gewaarschuwd voor goedkeuringsactiviteiten voor een onderdeel dat u gebruikt. Voor informatie over het vormen van welke berichten u ontvangt, zie [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Zie ook [&#x200B; de berichten van de Gebeurtenis &#x200B;](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th> <p>Inclusief velden </p> <p> *Alleen velden voor dagelijkse samenvatting</p> </th> 
   <th>Standaardstatus</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong> Een gedelegeerd verzoek van de de puntgoedkeuring wordt voltooid </strong> </p> <p>Een goedkeuring van de uitgave die u aan een andere gebruiker hebt gedelegeerd werd goedgekeurd of verworpen door die gebruiker.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Issue Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>De Naam van het project van de kwestie <br> Naam van het Referentienummer van het Project <br> van de gebruiker die/de kwestie binnen uw naam <br> goedkeurde van de Goedkeuring <br> de Status van de Uitgave <br> van de gebruiker goedkeurde <br> knoop <br><strong>[!UICONTROL See More Details]</strong> * Aantal van de Verwijzing van het Project <br> * De Naam van het Project <br>*Totaal aantal van gedelegeerde uitgiftegoedkeuringen <br> * Naam van de Naam van de Uitgave <br> <br> &lbrace; <br>*Datum van de dagelijkse samenvatting<br><br></p> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Een gedelegeerd verzoek van de projectgoedkeuring wordt voltooid </strong> </p> <p>Een projectgoedkeuring die u aan een andere gebruiker delegeerde werd goedgekeurd of verworpen door die gebruiker.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Project Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt; </em></p> <p><em> het onderwerp van het dagelijkse samenvattingsbericht is: [!UICONTROL Digest of Approval Information] &lt;Datum van dagelijkse samenvatting&gt; </em> </p> </td> 
   <td> De Naam van het project <br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br> Naam van de gebruiker die/het project namens uw <br>[!UICONTROL Approval Decision]<br>[!UICONTROL Project Status]<br> Naam van de gebruiker goedkeurde die om de goedkeuring <br><strong>[!UICONTROL See More Details]</strong> knoop <br> verzocht * Aantal van de Verwijzing van het Project <br> * Naam van het Project <br> * Naam van de fiatteur<br>[!UICONTROL *Date of the daily digest]<br></td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Een gedelegeerd verzoek van de taakgoedkeuring wordt voltooid </strong> </p> <p>Een taakgoedkeuring die u aan een andere gebruiker delegeerde werd goedgekeurd of verworpen door die gebruiker.</p> <p>Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Task Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt; </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> De Naam van het Project van de taak {<br> Naam van het Referentienummer van 1} Taak &lbrace;<br> van de gebruiker die/de taak binnen uw naam <br> goedkeurde <br> Status van de Taak <br> van de gebruiker goedkeurde die om de goedkeuring <br> verzocht zie Meer Details <br><strong> knoop </strong> * Aantal van de Verwijzing van het Project <br> * Naam van het Project <br>*Totaal aantal gedelegeerde taakgoedkeuringen <br> * Taak Approname <br> <br> ver Name <br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> het verzoek van de documentgoedkeuring van A wordt geannuleerd </strong> </p> <p>De documentfiatteur van het document ontvangt een e-mailbericht wanneer het verzoek om documentgoedkeuring wordt geannuleerd.</p> <p>Het onderwerp van de e-mail met onmiddellijke meldingen is: <em> &lt;Gebruikersnaam&gt; [!UICONTROL canceled the document approval request]</em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> Naam van de gebruiker die het goedkeuringsverzoek <br>[!UICONTROL Document Name] annuleerde </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> I wordt gedelegeerd als fiatteur </strong> </p> <p>Als iemand u toestemming heeft gegeven, ontvangt u een e-mailbericht. </p> <p>Het onderwerp van de directe melding-e-mail is: <em>[!UICONTROL Delegated] &lt;Object Type&gt; [!UICONTROL Approval - Please Review] &lt;Object Name&gt; </em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>De naam van de gebruiker die het voorwerp voor goedkeuring <br> Naam van de gebruiker voorlegde namens wie u de objecten <br> Status van Objecten <br> Datum en Tijd goedkeurde toen de goedkeuring <br> Prioriteit van Objecten <br> de Naam van de Stap van de Goedkeuring <br>[!UICONTROL Planned Completion Date] van de 6&rbrace; knoop van Objecten werd gevraagd<br><strong>[!UICONTROL Make Approval Decision]</strong></p> </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Mijn timesheet wordt goedgekeurd </strong> </p> <p>Wanneer uw tijdspagina is goedgekeurd, ontvangt u een e-mailbericht.</p> <p>Het onderwerp van de e-mail van de directe melding is: <em>[!UICONTROL Timesheet Approved]: &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt; </em></p> <p> <p>Opmerking: u kunt dit bericht niet configureren voor een e-mailbericht met dagelijkse samenvatting.</p> </p> </td> 
   <td> De naam van de gebruiker die uw Tijdopname <br> Datum en Tijd goedkeurde toen de Tijdopnemer <br> Status van Tijdopnemer ([!UICONTROL Approved]) <br> Datum van het Begin en Einddatum van Tijdopmaak <br> Totale uren die in de Tijdopnemer <br> worden geregistreerd Overuren van de Tijdopnemer in de Tijdopnemer &lbrace;worden geregistreerd </td> 
   <td><strong> Onmiddellijk </strong> </td> 
  </tr> 
 </tbody> 
</table>
