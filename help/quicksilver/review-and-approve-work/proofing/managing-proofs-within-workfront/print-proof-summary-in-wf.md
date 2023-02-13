---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Een proefdrukoverzicht afdrukken in Adobe Workfront
description: U kunt een proefdrukoverzicht afdrukken, opslaan als een PDF of exporteren als een XLS-bestand of PDF-bestand dat is geoptimaliseerd voor Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Een proefdrukoverzicht afdrukken in Adobe Workfront

U kunt een proefdrukoverzicht afdrukken, opslaan als een PDF of exporteren als een XLS-bestand of PDF-bestand dat is geoptimaliseerd voor Adobe Reader.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werken of plannen</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Een proefdrukoverzicht afdrukken of opslaan als een PDF-bestand

U kunt een proefdrukoverzicht rechtstreeks vanuit de documentlijst afdrukken.

>[!NOTE]
>
>U kunt niet meerdere proefsamenvattingen tegelijkertijd vanuit de documentlijst afdrukken.

1. Houd de muisaanwijzer boven de rij met het document in de documentlijst die de proefdruk bevat, en klik vervolgens op **Samenvatting afdrukken**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   of

   Klik tijdens het bekijken van de proefdruk in de kijker van het proef **Afdrukken** pictogram ![](assets/print-icon-in-pv.png) in de linkerwerkbalk. (Als de linkerwerkbalk niet zichtbaar is, klikt u op het pictogram Menu ![](assets/menu-icon-in-pv.png) in de linkerbovenhoek van de proefdrukviewer.)

1. Gebruik een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tonen</td> 
      <td> <p>Geef op wat u wilt afdrukken:</p> 
       <ul> 
        <li>De <strong>Huidige versie</strong> of <strong>Alle versies</strong> van het bewijs</li> 
        <li>Alleen de <strong>Pagina's met opmerkingen</strong> of <strong>Alle pagina's</strong></li> 
        <li>Alleen de <strong>Paginaminiaturen</strong> (een kleine weergave van elke pagina) of <strong>Volledige pagina's</strong> (volledige weergave van het bewijs)<br></li> 
        <p>Opmerking: Als u pinnummers wilt weergeven op markeringen in de afgedrukte uitvoer, moet u Volledige pagina's selecteren, niet Paginaminiaturen. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opmerkingen sorteren op</td> 
      <td> <p>(Alleen beschikbaar als u bovenstaande paginaminiaturen hebt geselecteerd) Geef de volgorde op waarin de opmerkingen van de proefdruk moeten worden afgedrukt:</p> 
       <ul> 
        <li><strong>Oudst</strong>: Van eerste opmerking naar laatste</li> 
        <li><strong>Laatste</strong>: Van laatste opmerking naar eerste</li> 
        <li><strong>Pagina</strong>: Op pagina, van de eerste pagina tot de laatste of van de laatste pagina tot de eerste</li> 
        <li><strong>Maker</strong>: Door de namen van de gebruikers die ze hebben toegevoegd, van A-Z of van Z-A</li> 
       </ul> <p>Deze opties zijn niet van invloed op de uitvoer die u als XLS- of PDF-bestand exporteert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opmerkingen filteren op</td> 
      <td> <p>U kunt elke gewenste combinatie van deze opties gebruiken om alleen bepaalde opmerkingen op te nemen in de uitvoer die u afdrukt of exporteert als een XLS- of PDF-bestand:</p> 
       <ul> 
        <li>Geselecteerde auteurs (standaardwaarde)</li> 
        <li>Acties die u selecteert</li> 
        <li><strong>Onopgelost</strong> status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workflow</td> 
      <td> <p>(Alleen beschikbaar als de proefdruk een geautomatiseerde workflow heeft) Klik op <strong>Diagram tonen</strong> in de gedrukte versie een schema op te nemen waarin de stadia van de proefnemingen en de beslissingen in elk stadium worden aangegeven. In het diagram dat wordt weergegeven, vertegenwoordigen de kleuren beslissingen die in een werkgebied worden genomen:</p> <p><strong>Groen</strong>: Goedgekeurd</p> <p><strong>Blauw</strong>: In afwachting van een beslissing</p> <p><strong>Rood</strong>: Wijzigingen vereist besluit</p> <p><strong>Grijs</strong>: Nog niet begonnen</p> <p><strong>Geel</strong>: Goedgekeurd met wijzigingen</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Afdrukken**.
1. Als u het overzicht wilt afdrukken, klikt u in het rechterdeelvenster van het venster dat wordt weergegeven op de knop **Doel** en klik vervolgens op **Meer weergeven**. Klik op de printer die u wilt gebruiken in de lijst die wordt weergegeven en klik vervolgens op **Afdrukken**.

   of

   Als u het overzicht wilt opslaan als een PDF-bestand, klikt u op de knop **Doel** menu, klikt u op **Opslaan als PDF** en klik vervolgens op **Opslaan**.

## Een proefdrukoverzicht exporteren als een XLS of PDF

U kunt een proefdrukoverzicht voor statische inhoud exporteren als een XLS-bestand of als een PDF-bestand. Het bewijs van uitvoer omvat alleen de inhoud van het bewijs.

1. Houd de muisaanwijzer boven de rij met het document in de documentlijst die de proefdruk bevat, en klik vervolgens op **Samenvatting afdrukken**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Klik op het pictogram XLS of PDF in de rechterbovenhoek van de pagina.

   ![](assets/xls-pdf-icons-350x136.png)

Wanneer het geëxporteerde bestand gereed is, ontvangt u een e-mail waarin u het bestand kunt downloaden.

Als u het overzicht hebt geëxporteerd als een PDF-bestand, worden opmerkingen over de proefdruk weergegeven in de PDF-lezer. Als aan een opmerking meerdere markeringen zijn gekoppeld, wordt de opmerking meerdere keren weergegeven in de lijst met opmerkingen (één keer voor elke markering).
