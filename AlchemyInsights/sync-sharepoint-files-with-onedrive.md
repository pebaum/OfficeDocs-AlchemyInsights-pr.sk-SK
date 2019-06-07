---
title: Synchronizácia súborov SharePointu pomocou nového synchronizačného klienta pre OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: b20692042917935eda213aa0e27b2a739a50e3d9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716276"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="38271-102">Synchronizácia súborov SharePointu pomocou nového synchronizačného klienta pre OneDrive</span><span class="sxs-lookup"><span data-stu-id="38271-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<p><span data-ttu-id="38271-103">
  <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Príkaz Otvoriť v prieskumníku otvorí lokálnu inštanciu Windows Prieskumníka, ktorá zobrazí štruktúru priečinkov na serveri hosťujúcom lokalitu SharePoint. Preto odporúčame <a href="https://support.office.com/sk-SK/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88">synchronizovať súbory SharePointu pomocou nového synchronizačného klienta OneDrive</a> s funkciou <a href="https://support.office.com/sk-SK/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e">súborov na požiadanie</a>, pretože poskytuje lokálny prístup k súborom a ponúka najlepší výkon.</span></span><span class="sxs-lookup"><span data-stu-id="38271-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site. This being said , we recommend <a href="https://support.office.com/en-us/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88">syncing SharePoint files with the new OneDrive sync client</a> which provides <a href="https://support.office.com/en-us/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e">Files On-Demand</a> because it provides local access to your files and offers the best performance</span></span></span></p> <p><span data-ttu-id="38271-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Ak ste sa miesto nového synchronizačného klienta rozhodli použiť zobrazenie v prieskumníku, postupujte podľa krokov a najvhodnejších postupov v článkoch nižšie.</span></span><span class="sxs-lookup"><span data-stu-id="38271-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span></span></p> <ul> <li><span data-ttu-id="38271-105">
  <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">
  <a href="https://support.office.com/sk-SK/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4">Riešenie problémov v SharePointe Online pomocou príkazu Otvoriť v prieskumníku</a></span></span><span class="sxs-lookup"><span data-stu-id="38271-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</a></span></span></span></li> <li><span data-ttu-id="38271-106">
  <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">
  <a href="https://support.office.com/sk-SK/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2">Kopírovanie alebo premiestňovanie súborov v knižnici pomocou príkazu Otvoriť v prieskumníku</a></span></span><span class="sxs-lookup"><span data-stu-id="38271-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2">Copy or move library files by using Open with Explorer</a></span></span></span></li> </ul> <p><span data-ttu-id="38271-107"><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Poznámka:</span></u></strong><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> Tlačidlo Otvoriť v prieskumníku sa nezobrazuje v novej knižnici. Kliknite na rozbaľovaciu ponuku <strong>Zobraziť</strong> v pravom hornom rohu (názov rozbaľovacej ponuky závisí od aktuálneho zobrazenia) a potom kliknite na položku <strong>Zobraziť</strong> v Prieskumníku.</span></span><span class="sxs-lookup"><span data-stu-id="38271-107"><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Note:</span></u></strong><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> The Open with Explorer button doesn't appear in the new library experience. Click the <strong>View</strong> drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click <strong>View</strong> in File Explorer.</span></span></span></p> <p><span data-ttu-id="38271-108"><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Poznámka: </span></u></strong><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> Príkaz Otvoriť v prieskumníku v SharePointe používa <strong>ovládacie prvky ActiveX</strong>, takže je podporovaný iba v prehliadači Internet Explorer 10 alebo 11. Príkaz Otvoriť v prieskumníku nefunguje vo Windowse v prehliadačoch Microsoft Edge, Google Chrome a Mozilla Firefox a ani na platforme Mac. Z tohto dôvodu môže byť možnosť &ldquo;Zobrazenie v Prieskumníku&rdquo; neaktívna.</span></span><span class="sxs-lookup"><span data-stu-id="38271-108"><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Note:</span></u></strong><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> SharePoint Open with Explorer uses <strong>ActiveX controls</strong>, so it's only supported in Internet Explorer 10 or 11. Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform. Due to this reason, the &ldquo;Explorer View&rdquo; option may be grayed out.</span></span></span></p> <ul> <li><span data-ttu-id="38271-109">
  <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">
  <a href="https://support.office.com/sk-SK/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca">Príčiny nedostupnosti ale neaktívnosti tlačidiel na páse s nástrojmi v SharePointe.</a></span></span><span class="sxs-lookup"><span data-stu-id="38271-109"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca">Why SharePoint ribbon buttons are unavailable or grayed out.</a></span></span></span></li> </ul> <p>&nbsp;</p>

  
