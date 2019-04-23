---
title: Vyriešiť otázky doručovanie pošty do e-mailu verejných priečinkov
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910627"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="fd754-102">Vyriešiť otázky doručovanie pošty do e-mailu verejných priečinkov</span><span class="sxs-lookup"><span data-stu-id="fd754-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="fd754-103">Ak externých odosielateľov nemôže odoslať správy na poštové verejné priečinky a odosielateľov Zobraziť chybové hlásenie: **Nepodarilo sa nájsť (550 5.4.1)**, skontrolujte email domény pre verejný priečinok je nakonfigurovaný ako doménu interného prenosu namiesto autoritatívnu doménu:</span><span class="sxs-lookup"><span data-stu-id="fd754-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="fd754-104">Otvorte [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="fd754-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="fd754-105">Prejsť na **tok pošty** \> **akceptovaných domén**, vyberte akceptovanej domény, a potom kliknite na tlačidlo **Upraviť**.</span><span class="sxs-lookup"><span data-stu-id="fd754-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="fd754-106">Vo vlastnostiach stránky otvorí, ak typ domény nastavená na **Authoritative**, zmeňte hodnotu na **interný prenos** a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="fd754-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="fd754-107">Ak externých odosielateľov chyba **nemáte povolenie (550 5.7.13)**, spustite nasledujúci príkaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a zobrazia sa povolenia pre anonymných používateľov vo verejnom priečinku:</span><span class="sxs-lookup"><span data-stu-id="fd754-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="fd754-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Napríklad `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="fd754-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="fd754-109">Ak chcete povoliť externým používateľom odosielať e-mailom na tento verejný priečinok, pridať CreateItems prístup priamo k užívateľovi Anonym.</span><span class="sxs-lookup"><span data-stu-id="fd754-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="fd754-110">Napríklad `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="fd754-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>