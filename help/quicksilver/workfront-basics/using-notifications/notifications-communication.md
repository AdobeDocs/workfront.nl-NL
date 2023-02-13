---
content-type: reference
navigation-topic: notifications
title: '"Meldingen: Communicatie'
description: In de volgende berichten wordt u gewaarschuwd voor communicatie, zoals een updateopmerking, die plaatsvindt op een tijdelijk onderdeel waarmee u te maken hebt. Zie Uw eigen gebeurtenismeldingen activeren of deactiveren voor informatie over het configureren van de meldingen die u ontvangt.
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%

---

# Meldingen: Communicatie

In de volgende berichten wordt u gewaarschuwd voor communicatie, zoals een updateopmerking, die plaatsvindt op een tijdelijk onderdeel waarmee u te maken hebt. Voor informatie over het vormen van welke berichten u ontvangt, zie [Uw eigen gebeurtenismeldingen activeren of deactiveren](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Deze meldingen geven een melding van alle opmerkingen die op een bepaald item zijn geplaatst. Daarom moet u alle meldingen selecteren of deselecteren en tegelijk verzenden in een e-mailbericht met een dagelijkse samenvatting. Als u alleen op de hoogte wilt worden gesteld van bepaalde opmerkingen wanneer deze plaatsvinden, kunt u de afzonderlijke meldingen opgeven die u wilt verzenden.

Zie ook [Gebeurtenismeldingen](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>Iemand neemt me op een geleide update</strong> </p> <p>Een geleide update is wanneer een gebruiker specifiek een andere gebruiker in een update omvat, zoals die in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] updates</a>.</p> <p>In dit geval ontvangt de gebruiker die is opgenomen in de gestuurde update een e-mailmelding over de update.</p> <p>Het e-mailbericht wordt alleen verzonden als de gebruiker toegangsrechten heeft voor het object.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL wanted you to know]</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is: <em>[!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Objectnaam waar de update is uitgevoerd<br>Naam bovenliggend object<br>Objectreferentienummer<br>Namen van alle gebruikers en teams die zijn opgenomen in de gestuurde update<br>Datum en tijd waarop de update is uitgevoerd<br>Tekst van gestuurde update<br><strong>[!UICONTROL Comment]</strong> knop<br>*Totaal aantal ontvangen opmerkingen<br>*Aantal ontvangen opmerkingen voor elk object<br>*<strong>[!UICONTROL See All Notifications]</strong> knop<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand antwoordt op mijn verzoek</strong> </p> <p>Nadat een gebruiker een werkverzoek indient en een andere gebruiker op dat werkverzoek antwoordt, ontvangt de gebruiker die het verzoek indiende een e-mailbericht.</p> <p>Er wordt geen e-mailmelding verzonden als:</p> 
    <ul> 
     <li> <p>De gebruiker die antwoordt is de zelfde gebruiker die het verzoek indiende</p> </li> 
     <li> <p>De gebruiker heeft geen toegang om de notitie te zien</p> </li> 
    </ul><strong>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Comment on] &lt;request name=""&gt; op &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></strong> Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> Naam aanvraag<br>Projectnaam<br>Referentienummer<br>Naam van de gebruiker die op uw verzoek heeft geantwoord<br>Datum en tijd waarop de opmerking is gemaakt<br>Tekst van de opmerkingen op uw verzoek<br>*Totaal aantal ontvangen opmerkingen<br>*Aantal ontvangen opmerkingen voor elke aanvraag<br>*<strong>[!UICONTROL See All Notifications]</strong> knop<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Op mijn verzoek is een opmerking geplaatst</strong> </p> <p>De primaire contactpersoon voor een uitgave ontvangt een e-mailbericht wanneer een opmerking op een [!UICONTROL Help Desk] verzoek, tenzij de gebruiker die de opmerking heeft geplaatst ook de primaire contactpersoon voor de kwestie is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Comment on] &lt;request name=""&gt; op &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Naam aanvraag<br>Projectnaam<br>Referentienummer<br>Naam van de gebruiker die op uw verzoek heeft geantwoord<br>Datum en tijd waarop de opmerking is gemaakt<br>Tekst van de opmerkingen op uw verzoek<br>*Totaal aantal ontvangen opmerkingen<br>*Aantal ontvangen opmerkingen voor elke aanvraag<br>*Projectnaam<br>*<strong>[!UICONTROL See All Notifications]</strong> knop<br>*Datum van de dagelijkse samenvatting<br></td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Er wordt een opmerking toegevoegd aan mijn document</strong> </p> <p>De eigenaar van een document in [!DNL Adobe Workfront] ontvangt een e-mailbericht wanneer een opmerking in het document wordt geplaatst, tenzij de gebruiker die de opmerking heeft geplaatst ook de eigenaar van het document is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current]. </p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Comment on] &lt;request name=""&gt; op &lt;project name=""&gt; (ref# &lt;request reference="" number=""&gt;)</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>Documentnaam<br>Project-, taak- of uitgeversnaam<br>Referentienummer<br>Naam van de gebruiker die op uw verzoek heeft geantwoord<br>Datum en tijd waarop de opmerking is gemaakt<br>Tekst van de opmerkingen die in het document zijn gemaakt</td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand reageert op een thread waar ik in zit</strong> </p> <p>De deelnemers in de draad en de gebruikers die in een direct bericht inbegrepen zijn ontvangen een e-mailbericht wanneer een gebruiker een commentaar in de draad aanbrengt.</p> <p>Gebruikers moeten beschikken over [!UICONTROL View] toegang om een bericht te ontvangen.</p> <p>De volgende gebruikers ontvangen geen melding:</p> 
    <ul> 
     <li>Teams die zijn opgenomen in een direct bericht</li> 
     <li>De eigenaar van de notitie</li> 
     <li>De primaire contactpersoon</li> 
    </ul> <p><strong>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL RE: Comment on] &lt;object name=""&gt;&lt;object type=""&gt; op &lt;project name=""&gt;(ref# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> Objectnaam<br>Naam bovenliggend object<br>Naam van de gebruiker die op de draad commentaren<br>Tekst van de op de verbinding gemaakte opmerking<br>Datum en tijd waarop de opmerking is gemaakt<br>*Totaal aantal ontvangen opmerkingen<br>*Aantal ontvangen opmerkingen voor elk object<br>*Projectnaam<br>*<strong>[!UICONTROL See All Notifications]</strong> knop<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand reageert op een van mijn werkitems</strong> </p> <p>De ontvanger van het werkitem ontvangt een e-mailbericht wanneer een gebruiker een update aan een werkitem toevoegt, tenzij de gebruiker die de update toevoegt ook de ontvanger is. </p> <p>Als er een opmerking op een aanvraag wordt geplaatst, stuurt u een e-mail naar de primaire contactpersoon voor de uitgave.</p> <p>De primaire contactpersoon voor een kwestie ontvangt een e-mailbericht wanneer een commentaar op een verzoek wordt gepost, tenzij de gebruiker die de opmerking heeft geplaatst ook de primaire contactpersoon voor de kwestie is.</p> <p>Gebruikers die rechtstreeks in de opmerking zijn opgenomen, ontvangen ook een e-mailbericht.</p> <p>Een kennisgeving wordt alleen verzonden als de projectstatus [!UICONTROL Current].</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>[!UICONTROL Comment on] &lt;work item="" name=""&gt; op &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Itemnaam zakelijk<br>Projectnaam<br>Referentienummer zakelijk item<br>Naam van de gebruiker die opmerkingen heeft gemaakt over het werkitem<br>Tekst van de opmerking die op het werkitem is geplaatst<br>Datum en tijd waarop de opmerking is gemaakt<br>*Totaal aantal ontvangen opmerkingen<br>*Aantal ontvangen opmerkingen voor elk object<br>*Projectnaam<br>*<strong>[!UICONTROL See All Notifications]</strong> knop<br>*Datum van de dagelijkse samenvatting </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Iemand neemt mijn team op een geleide update</strong> </p> <p>Een geleide update is wanneer een gebruiker specifiek een andere gebruiker in een update omvat, zoals die in <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Andere tags toepassen op updates</a>.</p> <p>In dit geval ontvangt elk lid van het team dat is opgenomen in de gestuurde update een e-mailmelding over de update.</p> <p>Het e-mailbericht wordt alleen verzonden naar gebruikers die toegangsrechten hebben tot het object.</p> <p>Als de gebruiker die de gestuurde update verzendt lid is van het team dat wordt opgenomen, ontvangt de gebruiker die de update verzendt geen e-mailbericht.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: [!UICONTROL Comment on] &lt;object name=""&gt; op &lt;parent object="" name=""&gt; (ref# &lt;object reference="" number=""&gt;)</p> <p> Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>Objectnaam<br>Naam bovenliggend object<br>Objectreferentienummer<br>Naam van de gebruiker die de gestuurde update heeft uitgevoerd<br>Naam van alle teams en gebruikers die zijn opgenomen in de gestuurde update<br>Datum en tijd waarop de gestuurde update is uitgevoerd<br>Tekst van de omgeleide update<br><strong>[!UICONTROL Comment]</strong> knop<br>*Totaal aantal ontvangen opmerkingen<br>*Aantal ontvangen opmerkingen voor elk object<br>*Projectnaam<br>*<strong>[!UICONTROL See All Notifications]</strong> knop<br>*Datum van de dagelijkse samenvatting </p> </td> 
   <td><strong>Dagelijks</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Wanneer de opmerking bij de gebruiker wordt toegevoegd</strong> </p> <p>U kunt een opmerking maken over een gebruiker in het dialoogvenster [!UICONTROL Updates] van het gebruikersobject. U kunt ook een opmerking plaatsen bij een gebruiker wanneer u de instellingen van de gebruiker bewerkt. De gebruiker waartegen de opmerking wordt geplaatst, ontvangt een e-mail om deze op de hoogte te stellen van deze opmerking. </p> <p>U moet minstens gemachtigd zijn [!UICONTROL View] de gebruiker om een update in te voeren op de [!UICONTROL Updates] van de gebruiker. U moet [!UICONTROL Edit] machtigingen voor de gebruiker om de instellingen van de gebruiker te bewerken. </p> <p>Ga voor meer informatie over het maken van opmerkingen over gebruikers op het tabblad Updates naar <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Werk bijwerken</a>.</p> <p>Voor meer informatie over het invoeren van een opmerking voor een gebruiker wanneer u de instellingen van de gebruiker bewerkt, raadpleegt u <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Mijn instellingen configureren</a>.</p> <p>Het onderwerp van de e-mail met onmiddellijke kennisgeving is: <em>&lt;user name=""&gt; [!UICONTROL wanted you to know]</em></p> <p>Het onderwerp van de dagelijkse overzichtsmelding is:<em> [!UICONTROL Digest of Communication] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> Uw gebruikersnaam<br>Naam van de gebruiker die de opmerking heeft toegevoegd<br>Tekst van de opmerking<br>Datum en tijd waarop de opmerking is gemaakt<br>*Totaal aantal ontvangen opmerkingen<br>*Aantal ontvangen opmerkingen voor elk object<br>*<strong>[!UICONTROL See All Notifications]</strong> knop<br>*Datum van de dagelijkse samenvatting </td> 
   <td> <p><strong>Meteen</strong> </p> <p><strong>en dagelijks</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
