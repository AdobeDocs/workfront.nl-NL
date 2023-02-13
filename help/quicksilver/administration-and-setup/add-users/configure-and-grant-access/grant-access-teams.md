---
title: Toegang verlenen aan teams
description: Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot teams in Workfront te definiëren
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Toegang verlenen aan teams

Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot teams in Workfront te definiëren, zoals wordt uitgelegd in [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## De toegang van gebruikers tot het bewerken van gebruikers configureren met behulp van een aangepast toegangsniveau

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** rechts van Teams selecteert u vervolgens de mogelijkheden die u onder **Uw instellingen nauwkeurig afstellen**.

   * **Weergave**: Als u configureert hoe gebruikers met een licentie teams kunnen weergeven, wijzigt u een van de volgende opties:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Aan mijn groepen gekoppelde teams weergeven</td>
         <td>
          <p><b>Ingeschakeld</b>: Wanneer de gebruikers teams op een type-vooruit gebied van het Team zoeken, kunnen de gebruikers de teams zien verbonden aan hun groepen al dan niet zij teamleden zijn. </p>
          <p><b>Uitgeschakeld</b>: Wanneer de gebruikers teams op een type-vooruit gebied van het Team zoeken, kunnen de gebruikers de teams zien verbonden aan hun groepen slechts waar zij teamleden zijn</p><p>Deze optie is standaard ingeschakeld.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Alle teams weergeven</td>
         <td><p>Wanneer deze optie wordt toegelaten en de gebruikers teams op een type-vooruit gebied van het Team zoeken, kunnen de gebruikers om het even welk team zien en selecteren.</p><p>Deze optie is standaard ingeschakeld. </p></td>
        </tr>
       </tbody>
      </table>

   * **Bewerken**: Als u configureert hoe gebruikers met een licentie voor abonnementen en werklicenties teams kunnen beheren, wijzigt u een van de volgende opties:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Maken</td>
         <td><p>Hiermee kunnen gebruikers met een licentie voor abonnementen of werken teams maken.</p><p>Deze optie is standaard ingeschakeld.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Verwijderen</td>
         <td><p> Hiermee kunnen gebruikers met een licentie voor abonnementen de teams verwijderen die ze kunnen bewerken (niet beschikbaar voor gebruikers met een werkvergunning).</p><p>Deze optie is standaard ingeschakeld.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Teams bewerken in groepen die ik beheer (alleen groepbeheerders)</td>
         <td><p>Hiermee staat u toe dat gebruikers van een abonnement die zijn aangewezen als groepsbeheerders, teams bewerken die zijn gekoppeld aan de groepen die zij beheren.</p><p>Deze optie is standaard ingeschakeld.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Teams bewerken die ik wil</td>
         <td><p>Hiermee staat u gebruikers toe een licentie of werklicentie te gebruiken om teams te bewerken waarin zij lid zijn.</p><p>Deze optie is standaard uitgeschakeld.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Aan mijn groepen gekoppelde teams weergeven</td>
         <td>
         <p><b>Ingeschakeld</b> Wanneer de gebruikers teams op een type-vooruit gebied van het Team zoeken, kunnen de gebruikers de teams zien verbonden aan hun groepen al dan niet zij teamleden zijn. </p>
         <p><b>Uitgeschakeld</b>: Wanneer de gebruikers teams op een type-vooruit gebied van het Team zoeken, kunnen de gebruikers de teams zien verbonden aan hun groepen slechts waar zij teamleden zijn</p><p>Deze optie is standaard ingeschakeld.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Alle teams weergeven</td>
         <td><p>Wanneer deze optie wordt toegelaten en de gebruikers teams op een type-vooruit gebied van het Team zoeken, kunnen de gebruikers om het even welk team zien en selecteren.</p><p>Deze optie is standaard ingeschakeld. </p></td>
        </tr>
       </tbody>
      </table>

1. Klik op de X om het dialoogvenster **Uw instellingen nauwkeurig afstellen** doos.
1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Als u klaar bent, klikt u op **Opslaan**.

>[!NOTE]
>
>* Het volgende is waar, ongeacht de montages van het toegangsniveau:
   >
   >   * Teameigenaars kunnen hun teams altijd weergeven en bewerken
   >   * De gebruikers hebben altijd toegang om de teams te bekijken zij op zijn
>
* De configuratie van om het even welke optie beschikbaar voor zowel Mening als geeft (zoals &quot;teams van de Mening verbonden aan mijn groepen&quot;) wordt behouden als u besluit om Mening in plaats van uit te geven of uit te geven in plaats van Mening op een toegangsniveau te selecteren.
>


## Toegang tot teams per licentietype

Voor informatie over wat de gebruikers in elk toegangsniveau met kwesties kunnen doen, zie de sectie [Teams](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
