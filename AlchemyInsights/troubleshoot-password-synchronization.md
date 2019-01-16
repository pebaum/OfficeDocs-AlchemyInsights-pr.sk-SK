---
title: Riešiť synchronizáciu hesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311423"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="5a992-102">Riešiť synchronizáciu hesla</span><span class="sxs-lookup"><span data-stu-id="5a992-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="5a992-103">Riešenie problémov, kde žiadne heslá sú synchronizované Azure AD pripojiť verziu 1.1.614.0 alebo novšiu verziu:</span><span class="sxs-lookup"><span data-stu-id="5a992-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="5a992-104">Otvorte novú reláciu prostredia Windows PowerShell na Azure AD pripojiť server pomocou možnosti **Spustiť ako správca** .</span><span class="sxs-lookup"><span data-stu-id="5a992-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="5a992-105">Spustiť **Set-ExecutionPolicy RemoteSigned** alebo **Set-ExecutionPolicy neobmedzený**.</span><span class="sxs-lookup"><span data-stu-id="5a992-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="5a992-106">Spustiť sprievodcu Azure AD pripojiť.</span><span class="sxs-lookup"><span data-stu-id="5a992-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="5a992-107">Prejdite na \*\* ďalšie úlohy \*\* stránky, vyberte \*\* riešenie \*\*, a kliknite na tlačidlo **ďalej**.</span><span class="sxs-lookup"><span data-stu-id="5a992-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="5a992-108">Na stránke Riešenie problémov kliknite na ponuku **spustenie na spustenie riešenia problémov** v prostredí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5a992-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="5a992-109">V hlavnom menu, vyberte **Riešenie problémov synchronizácie heslo**.</span><span class="sxs-lookup"><span data-stu-id="5a992-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="5a992-110">V podmenu vyberte **synchronizáciu hesla nefunguje vôbec**.</span><span class="sxs-lookup"><span data-stu-id="5a992-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="5a992-111">**Porozumieť výsledky riešenia úlohy**</span><span class="sxs-lookup"><span data-stu-id="5a992-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="5a992-112">Riešenie problémov úloha vykoná tieto kontroly:</span><span class="sxs-lookup"><span data-stu-id="5a992-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="5a992-113">Overuje, že heslo synchronizácia zapnutá pre nájomcu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5a992-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="5a992-114">Overuje, že Azure AD pripojiť server nie je v oddychových režime.</span><span class="sxs-lookup"><span data-stu-id="5a992-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="5a992-115">Pre každý existujúci lokálneho Active Directory konektor (čo zodpovedá existujúcu aktívnu Adresárová štruktúra):</span><span class="sxs-lookup"><span data-stu-id="5a992-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="5a992-116">Overuje, či je zapnutá funkcia synchronizácie heslo.</span><span class="sxs-lookup"><span data-stu-id="5a992-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="5a992-117">Vyhľadáva heslo synchronizácie tep udalostí v denníku udalostí aplikácie Windows.</span><span class="sxs-lookup"><span data-stu-id="5a992-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="5a992-118">Pre každú doménu služby Active Directory do lokálnej služby Active Directory konektor:</span><span class="sxs-lookup"><span data-stu-id="5a992-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="5a992-119">Overuje, že doména je dosiahnuteľný z server Azure AD pripojiť.</span><span class="sxs-lookup"><span data-stu-id="5a992-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="5a992-120">Overuje, že Active Directory Domain Services (AD DS) účty používané konektor služby Active Directory lokálne má správne meno používateľa, heslo a povolenia potrebné pre synchronizáciu hesla.</span><span class="sxs-lookup"><span data-stu-id="5a992-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="5a992-121">Viac pomoc riešenie problémov synchronizácie heslo nájdete v časti [Riešenie problémov heslo synchronizácia s Azure AD pripojenie synchronizácie](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="5a992-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  
