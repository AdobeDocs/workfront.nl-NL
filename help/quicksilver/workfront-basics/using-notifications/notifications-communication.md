---
content-type: reference
navigation-topic: notifications
title: 'Meldingen: Communicatie'
description: In de volgende berichten wordt u gewaarschuwd voor communicatie, zoals een updateopmerking, die plaatsvindt op een tijdelijk onderdeel waarmee u te maken hebt. Zie Uw eigen e-mailmeldingen wijzigen voor informatie over het configureren van de berichten die u ontvangt.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 0%

---

# Meldingen: Communicatie

In de volgende berichten wordt u gewaarschuwd voor communicatie, zoals een updateopmerking, die plaatsvindt op een tijdelijk onderdeel waarmee u te maken hebt. Voor informatie over het vormen van welke berichten u ontvangt, zie [ uw eigen e-mailberichten wijzigen ](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Deze meldingen geven een melding van alle opmerkingen die op een bepaald item zijn geplaatst. Daarom moet u alle meldingen selecteren of deselecteren en tegelijk verzenden in een e-mailbericht met een dagelijkse samenvatting. Als u alleen op de hoogte wilt worden gesteld van bepaalde opmerkingen wanneer deze plaatsvinden, kunt u de afzonderlijke meldingen opgeven die u wilt verzenden.

Zie ook [ de berichten van de Gebeurtenis ](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong> Iemand omvat me op een geleide update </strong> </p> <p>Een geleide update is wanneer een gebruiker specifiek een andere gebruiker in een update omvat, zoals die in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] updates </a> wordt beschreven.</p> <p>In dit geval ontvangt de gebruiker die is opgenomen in de gestuurde update een e-mailmelding over de update.</p> <p>Het e-mailbericht wordt alleen verzonden als de gebruiker toegangsrechten heeft voor het object.</p> <p>Het onderwerp van de e-mail met onmiddellijke meldingen is: <em>&lt;Naam van de gebruiker die u in de update heeft opgenomen&gt; [!UICONTROL wanted you to know]</em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is: <em>[!UICONTROL Digest of Communication] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> De Naam van objecten waar de update <br> Namen van het Aantal van de Verwijzing van 1&rbrace; Voorwerp van de Naam van het Voorwerp <br> van alle gebruikers en teams inbegrepen in de geleide update <br> Datum en Tijd werd gemaakt <br> Tekst van geleide update <br><strong>[!UICONTROL Comment]</strong> knoop <br>*Totaal aantal ontvangen commentaren <br>*Aantal commentaren voor elk voorwerp <br>* <strong>[!UICONTROL See All Notifications]</strong> knoop <br>*Datum van de dagelijkse samenvatting<br><br></td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> De antwoorden van iemand op mijn verzoek </strong> </p> <p>Nadat een gebruiker een werkverzoek indient en een andere gebruiker op dat werkverzoek antwoordt, ontvangt de gebruiker die het verzoek indiende een e-mailbericht.</p> <p>Er wordt geen e-mailmelding verzonden als:</p> 
    <ul> 
     <li> <p>De gebruiker die antwoordt is de zelfde gebruiker die het verzoek indiende</p> </li> 
     <li> <p>De gebruiker heeft geen toegang om de notitie te zien</p> </li> 
    </ul><strong> Het onderwerp van de directe bericht e-mail is: <em>[!UICONTROL Comment on] &lt;Naam van het Verzoek&gt; op &lt;Naam van Project&gt; (ref# &lt;Nummer van de Referentie van het Verzoek&gt;) </em> </strong> Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Communication] &lt;Datum van dagelijkse samenvatting&gt; </em></td> 
   <td> De Naam van het verzoek <br> Naam van het Project <br> Aantal van het Referentie <br> van de gebruiker die op uw Verzoek <br> Datum en Tijd antwoordde toen de commentaar <br> werd gemaakt Tekst van commentaar op uw Verzoek <br>*Totaal aantal ontvangen commentaren <br>*Aantal commentaren die voor elk verzoek <br>* <strong>[!UICONTROL See All Notifications]</strong> worden ontvangen knoop <br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> een commentaar van A wordt gepost op mijn verzoek </strong> </p> <p>De primaire contactpersoon voor een uitgave ontvangt een e-mailbericht wanneer een opmerking wordt geplaatst op een [!UICONTROL Help Desk] -aanvraag, tenzij de gebruiker die de opmerking heeft geplaatst ook de primaire contactpersoon voor de uitgave is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Comment on] &lt;Naam verzoek&gt; op &lt;Naam van project&gt; (ref# &lt;Referentienummer verzoek&gt;) </em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> De Naam van het verzoek <br> Naam van het Project <br> Aantal van het Referentie <br> van de gebruiker die op uw Verzoek <br> Datum en Tijd antwoordde toen de opmerking <br> Tekst van commentaar werd gemaakt op uw Verzoek <br>*Totaal aantal ontvangen commentaren <br>*Aantal commentaren voor elk verzoek <br> * De Naam van het Project <br> * <strong>[!UICONTROL See All Notifications]</strong> knoop <br>*Datum van de dagelijkse samenvatting<br></td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de commentaar van A wordt toegevoegd op mijn document </strong> </p> <p>De eigenaar van een document in [!DNL Adobe Workfront] ontvangt een e-mailbericht wanneer een opmerking in het document wordt geplaatst, tenzij de gebruiker die de opmerking heeft geplaatst ook de eigenaar van het document is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Er wordt alleen een melding verzonden als de projectstatus [!UICONTROL Current] is. </p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Comment on] &lt;Naam verzoek&gt; op &lt;Naam van project&gt; (ref# &lt;Referentienummer verzoek&gt;) </em></p> <p> Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt; </em></p> </td> 
   <td>De Naam van het document <br> Project, Taak, of de Naam van de Uitgave <br> Naam van het Verwijzing <br> Naam van de gebruiker die aan uw 3&rbrace; Datum en Tijd van het Verzoek antwoordde toen de opmerking <br> Tekst van commentaar werd gemaakt op het document<br></td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de commentaren van iemand op een draad ik binnen ben </strong> </p> <p>De deelnemers in de draad en de gebruikers die in een direct bericht inbegrepen zijn ontvangen een e-mailbericht wanneer een gebruiker een commentaar in de draad aanbrengt.</p> <p>Gebruikers moeten [!UICONTROL View] toegang hebben om een melding te ontvangen.</p> <p>De volgende gebruikers ontvangen geen melding:</p> 
    <ul> 
     <li>Teams die zijn opgenomen in een direct bericht</li> 
     <li>De eigenaar van de notitie</li> 
     <li>De primaire contactpersoon</li> 
    </ul> <p><strong> Het onderwerp van de onmiddellijke bericht e-mail is: <em>[!UICONTROL RE: Comment on] &lt;Objectnaam&gt;&lt;Objecttype&gt; op &lt;Projectnaam&gt; (ref# &lt;Objectreferentienummer&gt; </em>) </strong> </p> <p><strong> Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt; </em> </strong> </p> </td> 
   <td> De Naam van het voorwerp <br> Naam van het Voorwerp van de ouder &lbrace;<br> Naam van de gebruiker die op de draad <br> Tekst van commentaar becommentarieerde op de draad <br> Datum en Tijd maakte toen de opmerking <br>*Totaal aantal ontvangen commentaren <br>*Aantal commentaren voor elk voorwerp <br>*De Naam van het Project <br>* <strong>[!UICONTROL See All Notifications]</strong> knoop <br>*Datum van dagelijkse samenvatting werd ontvangen </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de commentaren van iemand op één van mijn werkpunten </strong> </p> <p>De ontvanger van het werkitem ontvangt een e-mailbericht wanneer een gebruiker een update aan een werkitem toevoegt, tenzij de gebruiker die de update toevoegt ook de ontvanger is. </p> <p>Als er een opmerking op een aanvraag wordt geplaatst, stuurt u een e-mail naar de primaire contactpersoon voor de uitgave.</p> <p>De primaire contactpersoon voor een kwestie ontvangt een e-mailbericht wanneer een commentaar op een verzoek wordt gepost, tenzij de gebruiker die de opmerking heeft geplaatst ook de primaire contactpersoon voor de kwestie is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Het onderwerp van de directe-berichtenmail is: <em>[!UICONTROL Comment on] &lt;Work Item Name&gt; op &lt;Project Name (ref# &lt;Work Item Reference Number&gt;) </em></p> <p> Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> De Naam van het Punt van het werk {<br> Naam van het Punt van het 1} Werk van de Naam van het Punt van het Werk <br> Tekst van de commentaren die op het Punt van het Werk <br> worden gemaakt Datum en Tijd toen de commentaar <br>*Totaal aantal ontvangen commentaren <br>*Aantal commentaren voor elk voorwerp <br>*De Naam van het Project <br>* <strong>[!UICONTROL See All Notifications]</strong> knoop <br>*Datum van dagelijkse samenvatting werd ontvangen<br><br> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Iemand omvat mijn team op een geleide update </strong> </p> <p>Een geleide update is wanneer een gebruiker specifiek een andere gebruiker in een update omvat, zoals die in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref"> wordt beschreven Tags anderen op updates </a>.</p> <p>In dit geval ontvangt elk lid van het team dat is opgenomen in de gestuurde update een e-mailmelding over de update.</p> <p>Het e-mailbericht wordt alleen verzonden naar gebruikers die toegangsrechten hebben tot het object.</p> <p>Als de gebruiker die de gestuurde update verzendt lid is van het team dat wordt opgenomen, ontvangt de gebruiker die de update verzendt geen e-mailbericht.</p> <p>Het onderwerp van de e-mail met expresmeldingen is: [!UICONTROL Comment on] &lt;Object name&gt; op &lt;Parent Object Name&gt; (ref# &lt;Object Reference Number&gt;)</p> <p> Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>De Naam van het voorwerp <br> Aantal van de Verwijzing van het Voorwerp &lbrace;<br> Naam van de gebruiker die de geleide update <br> Naam van alle teams en gebruikers inbegrepen in de geleide update <br> Datum en Tijd maakte toen de geleide update <br> Tekst van de geleide update <br><strong>[!UICONTROL Comment]</strong> knoop <br>*Totaal aantal ontvangen commentaren <br>*Aantal ontvangen commentaren voor elk voorwerp <br>*De Naam van het Project <br>* <strong>[!UICONTROL See All Notifications]</strong> <br> button <br>*Datum van dagelijkse samenvatting </p> </td> 
   <td><strong> Dagelijks </strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> wanneer de commentaar op gebruiker </strong> wordt toegevoegd </p> <p>U kunt een opmerking maken voor een gebruiker op het tabblad [!UICONTROL Updates] van het gebruikersobject. U kunt ook een opmerking plaatsen bij een gebruiker wanneer u de instellingen van de gebruiker bewerkt. De gebruiker waartegen de opmerking is geplaatst, ontvangt een e-mail om deze op de hoogte te stellen van deze opmerking. </p> <p>U moet machtigingen hebben voor ten minste [!UICONTROL View] de gebruiker om een update in te voeren op het tabblad [!UICONTROL Updates] van de gebruiker. U moet [!UICONTROL Edit] machtigingen hebben voor de gebruiker om de instellingen van de gebruiker te kunnen bewerken. </p> <p>Voor meer informatie over het maken van commentaren op gebruikers in het lusje van Updates, zie <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref"> het werk van de Update </a>.</p> <p>Voor meer informatie over het ingaan van een commentaar op een gebruiker wanneer u de montages van de gebruiker uitgeeft, zie <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref"> Mijn Montages </a> vormen.</p> <p>Het onderwerp van de e-mail met onmiddellijke meldingen is: <em> &lt;Gebruikersnaam&gt; [!UICONTROL wanted you to know]</em></p> <p>Het onderwerp van het dagelijkse samenvattingsbericht is:<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> Uw Naam van de Gebruiker <br> Naam van de gebruiker die de commentaar <br> Tekst van de commentaar <br> Datum en Tijd toevoegde de commentaar <br>*Totaal aantal ontvangen commentaren <br>*Aantal ontvangen commentaren voor elk voorwerp <br>* <strong>[!UICONTROL See All Notifications]</strong> knoop <br>*Datum van dagelijkse samenvatting </td> 
   <td> <p><strong> Onmiddellijk </strong> </p> <p><strong> en Dagelijks </strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
