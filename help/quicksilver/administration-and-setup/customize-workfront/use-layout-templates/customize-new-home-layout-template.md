---
title: Nieuwe startpagina aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Met een lay-outsjabloon kunt u configureren wat gebruikers zien wanneer ze nieuwe startpagina openen.
author: Nolan
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: 845f0c04923f6e35dcb004ba807c79577385462b
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Nieuwe startpagina aanpassen met een lay-outsjabloon

Met een lay-outsjabloon kunt u configureren wat gebruikers zien wanneer ze nieuwe startpagina openen.

U kunt configureren:

* Welke widgets standaard in de werkruimte worden weergegeven en de lay-out ervan op de pagina
* Welke achtergrond is geselecteerd
* Specifieke widgetinstellingen, waaronder de filters en groepen die beschikbaar zijn voor de widgets Mijn projecten, Mijn taken en Mijn problemen, en de standaardwaarden

>[!IMPORTANT]
>
>De sjablonen voor de beheerderslay-out die op deze pagina worden beschreven, hebben voorrang op de aanpassingsopties van individuele gebruikers.
>
>Wanneer wijzigingen in een lay-outsjabloon worden opgeslagen, wordt de nieuwe startpagina van gebruikers in die lay-outsjabloon aangepast aan de lay-outsjabloon en worden hun bestaande widgetselecties onder aan de pagina geplaatst. Widgets die door de beheerder zijn geselecteerd, kunnen door een gebruiker worden verplaatst en van grootte worden gewijzigd, maar kunnen niet worden verwijderd.

Ga voor meer informatie over de nieuwe introductiepagina naar [Aan de slag met Nieuwe startpagina](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

Voor informatie over het maken van lay-outsjablonen raadpleegt u [Lay-outsjablonen maken en beheren](../use-layout-templates/create-and-manage-layout-templates.md).

Voor informatie over lay-outsjablonen voor groepen raadpleegt u [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outsjabloon aan gebruikers raadpleegt u [Gebruikers toewijzen aan een lay-outsjabloon](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Nieuwe startpagina aanpassen met een lay-outsjabloon

1. Beginnen met het werken aan een lay-outsjabloon, zoals beschreven in [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klik op de pijl omlaag ![](assets/dropdown-arrow.png) krachtens **Aanpassen wat gebruikers zien** en klik vervolgens op **Werkruimte Home**.

1. Klik in de tabbladen die aan de rechterkant worden weergegeven op **Ontwerp en lay-out** om widgets en de achtergrond te kiezen en te rangschikken, of **Widget-instellingen** om instellingen voor afzonderlijke widgets, zoals beschikbare filters en groepen, te beheren.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ontwerp en lay-out</td> 
      <td>
      <p>Selecteer welke widgets in de werkruimten van de gebruikers aanwezig zullen zijn, hun positie, en kies een achtergrond. Hoewel gebruikers de geselecteerde widgets niet kunnen verwijderen, kunnen ze deze wel verplaatsen, de grootte ervan wijzigen en extra widgets toevoegen.</p>
      <p>Dit tabblad functioneert in feite als een kleine nieuwe werkruimte Home. Het kan daarom worden aangepast volgens de stappen die worden beschreven in <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Widgets toevoegen, bewerken of verwijderen in nieuwe startpagina</a>. Selecteer widgets en rangschik de werkruimte zoals u deze voor gebruikers wilt weergeven.</p>
      <p>Voer de volgende stappen uit om de achtergrond te wijzigen <b>Achtergrondaanpassing</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Aan de slag met Nieuwe startpagina</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Widget-instellingen</td> 
      <td>
      <p>Wijzig de instellingen voor afzonderlijke widgets. Momenteel worden slechts drie widgets ondersteund:</p>
      <ul>
        <li>Mijn projecten</li>
        <li>Mijn taken</li>
        <li>Mijn problemen</li>
      </ul>
      <p>Nadat u de widget hebt geselecteerd die u wilt bewerken, worden de beschikbare opties rechts weergegeven. Deze opties zijn momenteel <b>Filters</b> en <b>Groepen</b>. U kunt:</p>
      <ul>
        <li><b>Selecteer welke filters of groepen beschikbaar zijn voor gebruikers:</b><p>Schakel het vakje naast alle opties in de lijst in die gebruikers mogen gebruiken. Niet-geselecteerde opties worden niet weergegeven voor gebruikers.</li></p>
        <li><b>Stel een standaardfilter of -groep in voor de widget:</b><p>Houd de muis boven een optie en er verschijnt een knop waarmee u die optie als de standaardinstelling voor gebruikers kunt instellen. De huidige standaardinstelling heeft rechts een blauwe standaardbadge.</li></p>
        <li><b>Voeg een bestaand filter of een bestaande groep toe aan de lijst met beschikbare opties:</b><p>Klik op de knop met het plusteken onder aan elke lijst om een optie aan die lijst toe te voegen. Alleen bestaande filters of groepen kunnen op deze manier worden toegevoegd.</li></p>
      </ul>
      </td> 
     </tr>
    </tbody> 
   </table>

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u klaar bent met aanpassen, klikt u op **Opslaan** in de linkerbenedenhoek.

