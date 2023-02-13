---
title: Gebruikers administratieve toegang verlenen tot bepaalde gebieden
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om gebruikers van een de vergunningsadministratieve toegang van het Plan tot bepaalde gebieden van het systeem te verlenen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# Gebruikers administratieve toegang verlenen tot bepaalde gebieden

<!--Linked in several places, do not rename or change URL.-->

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om gebruikers van een de vergunningsadministratieve toegang van het Plan tot bepaalde gebieden van het systeem te verlenen.

>[!NOTE]
>
>Dit is anders dan het geven van volledige administratieve toegang tot Workfront aan een gebruiker, zoals wordt uitgelegd in [Volledige administratieve toegang verlenen aan een gebruiker](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md). &#x200B;

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gebruikers van het subsidieplan hebben administratieve toegang tot bepaalde gebieden van Workfront

>[!IMPORTANT]
>
>Wij adviseren sterk dat u de ingebouwde toegangsniveaus onveranderd laat zodat u naar hen kunt verwijzen nadat u opstelling uw gebruikers. Als u een toegangsniveau wilt aanpassen, kopieert u het standaardtoegangsniveau en wijzigt u de kopie. (U kunt dit voor elk toegangsniveau behalve de Beheerder van het Systeem en Externe Gebruiker doen.)

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Toegangsniveaus**.
1. Klik op de naam van het toegangsniveau dat u wilt gebruiken om gebruikers administratieve toegang te verlenen tot bepaalde gebieden van Workfront.
1. In de **Beheertoegang toestaan voor** , selectievakjes om de nodige administratieve toegang te verlenen.

   Met deze opties kunt u de volgende mogelijkheden bieden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Goedkeuringsprocessen</td> 
      <td><p>Goedkeuringsprocessen voor gebruik in het hele systeem en voor specifieke groepen maken en beheren.</p><p>Zonder deze toegang kunnen gebruikers alleen ad-hocgoedkeuringsprocessen maken voor items die ze kunnen beheren.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bedrijven</td> 
      <td><p>Nieuwe bedrijven toevoegen en bestaande bedrijven in Workfront bewerken</p>
      <p>Zonder deze toegang kunnen gebruikers alleen bestaande bedrijven bekijken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste formulieren</td> 
      <td><p>Aangepaste formulieren in hun groep maken en bewerken (de velden toevoegen, bewerken en verwijderen).</p><p>Zonder deze toegang kunnen gebruikers bestaande formulieren alleen koppelen aan objecten waartoe ze toegang hebben om bij te dragen of te beheren.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wisselkoersen</td> 
      <td> <p>Voeg nieuwe valuta toe in Workfront.</p> <p>Zonder deze toegang kan de gebruiker alleen een bestaande valuta toevoegen aan een project dat hij of zij maakt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td><p>Alle uitgaven weergeven voor objecten in Workfront.</p><p>Hierdoor kan de gebruiker geen nieuwe kostentypen maken.</p><p>Zonder deze toegang kan de gebruiker alleen het volgende weergeven:</p>
       <ul>
        <li>Uitgaven voor projecten, taken of kwesties die zij beheren</li>
        <li>Hun eigen kosten</li>
        <li>De kosten van hun ondergeschikten</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Functies</td> 
      <td> <p>Met deze toegang mag de gebruiker het volgende doen:</p> 
       <ul> 
        <li>Bestaande taakrollen weergeven en bewerken</li> 
        <li>Nieuwe taakrollen toevoegen</li> 
        <li>Rolfacturering en kostentarieven bewerken</li> 
       </ul> <p><b>BELANGRIJK</b>: Als u een gebruiker van de Planner administratieve toegang tot baanrollen verleent, wordt de de toegang die van Gegevens van de Financiële plaatsen de Facturering van de Rol &amp; Tarieven van de Kosten uitgeeft voor de gebruiker automatisch toegelaten. Later, als u administratieve toegang tot baanrollen voor de gebruiker van de Planner onbruikbaar maakt, zijn de baanrollen nog zichtbaar aan de gebruiker omdat Edit de Facturering van de Rol &amp; het plaatsen van de Tarieven nog wordt toegelaten. Als dit gebeurt en u de toegang van de gebruiker tot de rollen van de meningsbaan moet verwijderen, moet u de het Edit van de Rol van de gebruiker het Factureren &amp; van de Tarieven van Kosten plaatsen van de Toestemming onbruikbaar maken. Zie voor instructies <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Toegang tot financiële gegevens verlenen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mijlpalen in mijn fractie</td> 
      <td>Bekijk alle milestone-paden in het systeem onder het menu Paden van mijlpaal in Setup. De gebruikers kunnen om het even welke milestone wegen ook uitgeven of schrappen die tot om het even welk van hun groepen behoren. De gebruikers kunnen niet de milestone wegen beheren (uitgeven of schrappen) die niet aan om het even welk van hun groepen worden toegewezen.<br><p>Zonder deze toegang, kunnen de gebruikers bestaande milestone wegen slechts bekijken en hen toepassen op projecten zij toegang hebben te beheren.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td>Herinneringsberichten maken en beheren in Workfront.<br>Zonder deze toegang zijn gebruikers beperkt tot het ontvangen en weergeven van meldingen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timesheets en uren</td> 
      <td> <p>Hiermee kunnen gebruikers alle uren en tijdbladen in Workfront bekijken.</p> <p>Wanneer deze optie is uitgeschakeld, kunnen gebruikers slechts uren weergeven op:</p> 
       <ul> 
        <li>Projecten, taken of problemen die ze beheren</li> 
        <li>Hun eigen tijdschema</li> 
        <li>Een tijdspad van iemand die een melding ontvangt</li> 
        <li>Een door hen goed te keuren tijdschema</li> 
       </ul> <p><b>OPMERKING</b>:  <p>Of deze optie nu in- of uitgeschakeld is, groepsbeheerders kunnen timesheet-profielen maken voor de groepen en subgroepen die zij beheren en deze toewijzen aan groepsleden waarvan zij de gebruikersprofielen kunnen bewerken.</p> <p>Het toelaten van deze optie zou teveel toegang voor sommige groepsbeheerders kunnen verlenen omdat zij timesheets kunnen bekijken die door timesheet profielen (en de uren) voor alle gebruikers in het systeem worden geproduceerd, niet alleen voor die in de groepen die zij beheren. U kunt deze optie voor groepsbeheerders onbruikbaar maken die niet veel toegang nodig hebben.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Als u klaar bent, klikt u op **Opslaan**.
1. Wijs het nieuwe toegangsniveau aan een gebruiker toe, zoals die in wordt beschreven [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >U kunt gebruikers administratieve toegang tot gebruikers toestaan. Voor meer informatie over het geven van gebruikers administratieve toegang tot gebruikers zodat kunnen zij gebruikersrekeningen beheren, zie [Toegang verlenen aan gebruikers](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
