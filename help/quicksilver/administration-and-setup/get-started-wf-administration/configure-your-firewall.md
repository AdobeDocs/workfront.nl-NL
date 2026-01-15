---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: De Lijst van gewenste personen van uw firewall configureren
description: Als uw firewall of postserver wordt gevormd om toegang tot slechts bepaalde verkopers toe te staan, moet u bepaalde IP adressen aan zijn lijst van gewenste personen toevoegen. Hierdoor wordt de communicatie tussen uw omgeving en de Adobe Workfront-servers geopend en kunnen uw gebruikers berichten verzenden vanuit Workfront en SSO gebruiken met Active Directory of LDAP.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 3c680b39685e650dd442adbb49e4091d558d1410
workflow-type: tm+mt
source-wordcount: '1603'
ht-degree: 0%

---

# De lijst van gewenste personen van uw firewall configureren

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
>
>Om uw lijst van gewenste personen te vormen als uw organisatie aan Adobe Admin Console is bezet, zie [&#x200B; Domeinen worden toegestaan voor de Apps en de Diensten van Adobe &#x200B;](https://helpx.adobe.com/nl/enterprise/kb/network-endpoints.html).
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [&#x200B; Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfsplatform) &#x200B;](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>De manier een organisatie zijn lijst van gewenste personen vormt is uniek aan elke organisatie. Werk samen met uw IT-team om de procedure van uw organisatie te identificeren en deze toevoegingen te implementeren.

Als uw firewall of postserver wordt gevormd om toegang tot slechts bepaalde verkopers toe te staan, moet u bepaalde IP adressen aan zijn lijst van gewenste personen toevoegen. Hierdoor wordt de communicatie tussen uw omgeving en de Adobe Workfront-servers geopend en zijn de volgende processen mogelijk:

* Berichten verzenden vanuit de Workfront-toepassing

  >[!NOTE]
  >
  >Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

* Documentwebkoppelingen gebruiken bij het configureren van aangepaste documentintegratie
* Workfront Event-abonnementen gebruiken

  Voor meer informatie, zie [&#x200B; Abonnement API van de Gebeurtenis &#x200B;](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

U moet ook bepaalde poorten openen om e-mailberichten te coderen wanneer ze worden geleverd.

## Workfront-lijsten van gewenste personen die u kunt gebruiken

Als uw organisatie het plan van de Onderneming heeft, kunt u twee lijsten van gewenste personen van Workfront ook vormen:

* **lijst van gewenste personen E-mail**: Laat u controleren waar de gebruikers gegevens kunnen e-mailen die in Workfront worden opgeslagen. Voor meer informatie, zie [&#x200B; uw e-maillijst van gewenste personen &#x200B;](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md) vormen.
* **IP lijst van gewenste personen**: Beperkt toegang tot Workfront tot 75 IP adressen of IP adreswaaiers die u specificeert, die een extra laag van veiligheid voor de toepassing van Workfront verstrekken. Voor meer informatie, zie [&#x200B; toegang tot Adobe Workfront door IP adres &#x200B;](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md) beperken.

## Zoek uw Workfront-cluster

De IP adressen die u aan uw lijst van gewenste personen op uw firewall moet toevoegen hangen van de cluster af waar uw milieu van de Productie loopt.

De cluster van uw organisatie zoeken:

{{step-1-to-setup}}

1. In de linkernavigatie, klik **Systeem**, dan uitgezochte **Info van de Klant**.
1. Bepaal de plaats van het **gebied van de Opstelling van de Cluster** bij de hoger-juiste hoek van de pagina. De cluster van uw organisatie wordt hier vermeld.

   CL01 verwijst naar Cluster 1, CL02 is Cluster 2, enzovoort.

Voor meer informatie, zie de sectie [&#x200B; de cluster van uw organisatie en het plan van Workfront van &#x200B;](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) in het overzicht van de artikel [&#x200B; Firewall &#x200B;](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## IP adressen om aan de lijst van gewenste personen toe te voegen

>[!IMPORTANT]
>
>Sommige integratie van Workfront werkt niet wanneer de lijst van gewenste personen wordt toegelaten omdat zij niet met een statisch IP adres kunnen worden gevormd. Als u de volgende integratie wilt gebruiken, moet u de lijst van gewenste personen uitschakelen.
>
>* Workfront for Outlook

* [&#x200B; IP adressen om voor Clusters 1, 2, 3, 5, 7, 8 en 9 toe te staan &#x200B;](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [&#x200B; IP adressen om voor Cluster 4 &#x200B;](#ip-addresses-to-allow-for-cluster-4) toe te staan
* [&#x200B; IP adressen om voor Cluster 6 &#x200B;](#ip-addresses-to-allow-for-cluster-6) toe te staan
* [IP adressen om voor Cluster 10 toe te staan](#ip-addresses-to-allow-for-cluster-10)
* [&#x200B; IP adressen om voor een Aandrijving van de Test &#x200B;](#IP%20Addre2) toe te staan
* [&#x200B; IP adressen om toe te staan wanneer het uitvoeren van gebeurtenisabonnementen &#x200B;](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [&#x200B; IP adressen om voor de toegang tot van de Fusie van Workfront &#x200B;](#ip-addresses-to-add-for-accessing-workfront-fusion) toe te voegen
* [&#x200B; IP adressen om voor het gebruiken van Workfront voor Jira toe te voegen &#x200B;](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URL&#39;s die moeten worden toegevoegd voor alle clusters Workfront](#urls-to-add-for-all-clusters-workfront)

### IP-adressen voor clusters 1, 2, 3, 5, 7, 8 en 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Als uw milieu van de Productie op Cluster 1, 2, 3, 5, 7, 8, of 9 is moet u de volgende IP adressen toestaan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Voor SSO, documentwebhaken of andere functionaliteit</td> 
   <td> 
    <ul> 
     <li>35 160 0 242</li> 
     <li>34 213 36 118</li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52 36 154,34</li> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">E-mail ontvangen van de Workfront-toepassing</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181,84</li> 
     <li>35 161 82 137</li> 
     <li>52.14.70.114</li> 
     <li>52 15 230 220</li> 
     <li>54 71 252,65</li>
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>23 251 237 109</li> 
     <li>23 251 237 106</li> 
     <li>206 55 149 212</li>
     <li>206 55 149 214</li>
     <li>206 55 149 215</li>
     <li>206 55 149 213</li>
     <li>206 55 149 211</li>
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP adressen om voor Cluster 4 toe te staan {#ip-addresses-to-allow-for-cluster-4}

Als uw Productieomgeving zich op Cluster 4 bevindt, voegt u de volgende IP-adressen voor SSO toe, voegt u de integratie van de documentwebhaak en ontvangt u e-mail van de Workfront-toepassing:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69 169 230,232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32
* 23.251.239.98
* 23.251.239.99
* 24.110.76.224
* 24.110.76.223

### IP adressen om voor Cluster 6 toe te staan {#ip-addresses-to-allow-for-cluster-6}

Als uw milieu van de Productie op Cluster 6 is, voeg de volgende IP adressen toe.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">E-mail ontvangen van de Workfront-toepassing</td> 
   <td> 
    <ul> 
     <li>34 94 227,64</li> 
     <li>34 94 227,65</li> 
     <li>34 94 227,66</li> 
     <li>34 94 227,67</li> 
     <li>34 66 82 64</li> 
     <li>34 66 82 65</li> 
     <li>34 66 82 66</li> 
     <li>34 66 82 67</li> 
    <li>206 55 149 212</li>
   <li>206 55 149 214</li>
   <li>206 55 149 215</li>
   <li>206 55 149 213</li>
   <li>206 55 149 211</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">De e-mailservice gebruiken</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181,84</li> 
     <li>35 161 82 137</li> 
     <li>52.14.70.114</li> 
     <li>52 15 230 220</li> 
     <li>54 71 252,65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">De mailservice van Mailgun gebruiken</td> 
   <td> 
    <ul> 
     <li>143 55 228,56 </li> 
     <li>209 61 151 229</li> 
     <li>69 72 43,7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP adressen om voor Cluster 10 toe te staan

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

### IP adressen om voor Cluster 11 toe te staan

Voeg de volgende IP-adressen toe om e-mail te ontvangen van de Workfront-toepassing in cluster 11:

* 24.110.76.224
* 24.110.76.223

### IP adressen om voor een Aandrijving van de Test toe te staan

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">E-mail ontvangen van de Workfront-toepassing wanneer u een teststation gebruikt</td> 
   <td> 
    <ul> 
     <li>69 42 126 188 </li> 
     <li>66 119 37 185</li> 
     <li>66 119 37 186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Voor integratie van SSO's en documentwebhaak bij gebruik van een teststation</td> 
   <td> 
    <ul> 
     <li> <p>69 42 126 188:</p> <p>Dit adres moet ook aan uw lijst van gewenste personen worden toegevoegd zodat uw gebruikers e-mails van Workfront kunnen ontvangen.</p> </li> 
     <li>66 119 37 186</li> 
     <li>66 119 37 167</li> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP adressen toestaan wanneer het uitvoeren van gebeurtenisabonnementen  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Voor alle milieu&#39;s, voeg de volgende IP adressen toe om ladingen van de gebeurtenisabonnementen van Workfront te ontvangen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Voor klanten in Europa</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>52 208 159 124</li> 
     <li>54 220 93 204</li> 
     <li>Op 52.17.130.2011</li> 
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Voor klanten op andere locaties dan Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52 36 154,34</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52 39 217 230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-adressen die moeten worden toegevoegd voor toegang tot Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Voeg de volgende IP adressen aan uw lijst van gewenste personen toe om Workfront Fusion toe te laten om tot uw systeem toegang te hebben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li> 
     <li>10.20.126.137</li>
     <li>34 223 32,4</li>
     <li>52 39 176 220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] op de Microsoft Azure-cluster</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Ook, als uw organisatie uitgaande netwerk het filtreren gebruikt, voeg het volgende domein aan uw lijst van gewenste personen toe om uw systeem toe te laten om tot Workfront Fusion toegang te hebben. Deze URL&#39;s worden gebruikt voor webhaken in Fusion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] op de Microsoft Azure-cluster</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Het uitgaande netwerk filtreren is ongewoon. Controleer met uw netwerkbeheerder om te zien of moet u uw lijst van gewenste personen bijwerken om voor het aan te passen.

### IP adressen om voor het gebruiken van Workfront voor Jira toe te voegen {#ip-addresses-to-add-for-using-workfront-for-jira}

Voeg de volgende IP adressen aan uw lijst van gewenste personen toe om Workfront voor de integratie van Jira te gebruiken.

Het domein jira.workfront.com moet ook toegankelijk zijn vanaf uw bedrijfsservers. Dit domein is vereist omdat het als middleware tussen Workfront en Jira fungeert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Voor klanten in Europa</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>52 208 159 124</li> 
     <li>54 220 93 204</li> 
     <li>Op 52.17.130.2011</li> 
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
     <li>35 162 128,73</li> 
     <li>52.42.25,64</li> 
     <li>34 213 36 118</li> 
     <li>35 160 0 242 </li> 
     <li> <p>3 209 27 146</p> </li> 
     <li> <p>18 205 251,4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Voor klanten op andere locaties dan Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52 36 154,34</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52 39 217 230</li> 
     <li>35 162 128,73</li> 
     <li>52.42.25,64</li> 
     <li>34 213 36 118</li> 
     <li>35 160 0 242 </li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Toe te voegen domeinen voor toegang tot Workfront

Als uw organisatie uitgaande netwerk het filtreren gebruikt, voeg de volgende domeinen aan uw lijst van gewenste personen toe om uw systeem toe te laten om tot Workfront toegang te hebben.

>[!NOTE]
>
>Het uitgaande netwerk filtreren is ongewoon. Controleer met uw netwerkbeheerder om te zien of moet u uw lijst van gewenste personen bijwerken om voor het aan te passen.

* `<your domain>` .my.workfront.com
* `<your domain>` .preview.workfront.com
* `<your domain>` .sb01.workfront.com
* `<your domain>` .sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* snippet.maze.co
* *.aptrinsic.com
* *.static.workfront.com


  Dit is een statisch domein dat alle volgende domeinen uitcompileert. U kunt desgewenst de afzonderlijke domeinen toevoegen:

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

Als uw organisatie op de Adobe Verenigde Ervaring is, gebruikt het de volgende domeinen. Deze domeinen worden behandeld onder `*.adobe.com` , maar kunnen desgewenst worden toegevoegd.

* &lt;your domain>.my.workfront.adobe.com
* &lt;your domain>.preview.workfront.adobe.com
* &lt;your domain>.sb01.workfront.adobe.com
* &lt;your domain>.sb02.workfront.adobe.com


Voeg bij Workfront Fusion de volgende domeinen toe:

* Voor organisatie niet op de Adobe Verenigde Ervaring:
   * app.workfrontfusion.com (VS AWS)
   * app-eu.workfrontfusion.com (EU AWS)
   * app-az.workfrontfusion.com (US Azure)

* Voor organisatie op de Adobe Unified Experience
(Deze domeinen worden behandeld onder `*.adobe.com` , maar kunnen desgewenst worden toegevoegd.)

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## URL&#39;s die moeten worden toegevoegd voor alle clusters Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Help-inhoud weergeven in uw Workfront-omgeving</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Als u Workfront Proof toegang wilt geven tot Workfront in elke cluster, voegt u deze toe aan alle omgevingen</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Vereist om proefdrukken in Workfront te bekijken</li> 
     <li>*.proofhq.com - Vereist om proefdrukken in Workfront Proof te bekijken</li> 
     <li>*.proofhq.eu - Vereist om proefdrukken in Workfront Proof te bekijken</li> 
    </ul> <p><b> NOTA </b>:  <p>Wij steunen het toevoegen van IP adressen aan uw lijst van gewenste personen voor Workfront Proof niet. Ze waren dynamisch nadat Workfront naar AWS was verhuisd. In plaats daarvan raden we u aan alleen Workfront Proof-domeinen toe te staan.</p> <p>Als er een probleem is met het toevoegen van deze domeinen aan uw lijst van gewenste personen en u hebt in plaats daarvan een IP-adres nodig, neemt u contact op met de klantenondersteuning van Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## IP-adressen en URL&#39;s die moeten worden toegevoegd voor toegang tot Workfront Proof

U moet de volgende IP adressen aan uw lijst van gewenste personen toevoegen om diverse functies te gebruiken.

* [&#x200B; voor callbacks en Webcapture proefdrukken &#x200B;](#for-callbacks-and-webcapture-proofs)
* [Voor uitgaande e-mail](#for-outgoing-email)

### Voor callbacks en webcapture-proefdrukken {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (clusters 1, 2, 3, 5 en 7)</td> 
   <td> 
    <ul> 
    <li>35 84 172 250</li>
     <li>34 213 36 118</li> 
     <li>35 160 0 242</li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
     <li>35 165 152 202</li> 
     <li>54 184 151 122</li> 
     <li>35.84.40.190</li> 
     <li>54 218 48 56</li> 
     <li>34 211 224,9</li> 
     <li>52 36 154,34</li> 
     <li>34 232 138,38</li> 
     <li>54 237 6 156</li> 
     <li>54 237 12 32</li> 
     <li>44 241 82 96</li> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>52 207 47 153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
    <li>34 255 252 190</li>
     <li>34 246 27 40</li> 
     <li>52 208 123 166</li> 
     <li>3 121 129</li> 
     <li>3 122 11 35</li> 
     <li>34 241 103,51</li> 
     <li>Op 46.51.203.2011</li> 
     <li>54 247 174 227</li> 
     <li>52 208 159 124</li> 
     <li>Op 52.17.130.2011</li> 
     <li>34 252 250 191</li> 
     <li>52 30 133 50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> <p><b> NOTA </b>: DNS de serveropties worden niet meer gesteund.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Voor uitgaande e-mail {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (clusters 1, 2, 3, 5 en 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23 251 237 106</li> 
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (cluster 4)</td> 
   <td> 
    <ul> 
     <li>23 251 239,98</li> 
     <li>69 169 230 231</li> 
     <li>69 169 230 232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Poorten om te openen voor de beste Workfront Proof-prestaties

Open de volgende poorten als u problemen ondervindt met het laden van proefdrukken of als u niet werkt in Workfront Proof:

* 5671
* 5672
* 15671

## Poorten die moeten worden geopend voor gecodeerde e-mail

E-mails van de Workfront-toepassing worden versleuteld met de poorten 465 en 587. Als uw mailserver geen ondersteuning biedt voor gecodeerde e-mail, worden e-mails zonder codering verzonden met poort 25.

## E-mailmeldingen van Workfront-ondersteuning

Als u geen e-mails ontvangt van Workfront Support, moet u de Salesforce IP-adressen en -domeinen toevoegen die u nodig hebt. Raadpleeg het Help-artikel van Salesforce over Salesforce IP-adressen en -domeinen die u wilt toestaan voor meer informatie.
