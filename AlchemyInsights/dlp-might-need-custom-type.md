---
title: DLP potrebovať vlastný typ
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: cd5bac5efe3a16d32f9b695c8cb452a1eaa3a796
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2019
ms.locfileid: "31872488"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="1f4c0-102">DLP potrebovať vlastný typ</span><span class="sxs-lookup"><span data-stu-id="1f4c0-102">DLP might need a custom type</span></span>

<span data-ttu-id="1f4c0-103">S údajov loss prevention (DLP) politiky, môžete identifikovať a ochranu citlivých údajov v organizácii.</span><span class="sxs-lookup"><span data-stu-id="1f4c0-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="1f4c0-104">V niektorých prípadoch budete musieť vytvoriť svoj vlastný **vlastný** typ citlivé informácie chrániť údaje organizácie.</span><span class="sxs-lookup"><span data-stu-id="1f4c0-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="1f4c0-105">Napríklad vašej organizácii môže byť potrebné na identifikáciu a ochranu zamestnancov ID alebo iné dáta v nejakej forme špecifické pre vaše org. Ak áno, nájdete v nasledujúcich článkoch ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="1f4c0-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="1f4c0-106">**Prispôsobiť typ vstavaný citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="1f4c0-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="1f4c0-107">Ak typ vstavaný citlivých informácií by vyhovoval vašim potrebám s niekoľkými Tweak, môžete [prispôsobiť typ vstavaný citlivých informácií](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1f4c0-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="1f4c0-108">Napríklad, môžete pridať alebo odstrániť kľúčové slová, alebo pridať či odstrániť podporné dôkazy napríklad dátum alebo adresu.</span><span class="sxs-lookup"><span data-stu-id="1f4c0-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="1f4c0-109">**Vytvorenie vlastných citlivých informácií typu**</span><span class="sxs-lookup"><span data-stu-id="1f4c0-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="1f4c0-110">Ale ak potrebujete na identifikáciu a ochranu citlivých informácií typu úplne, môžete [vytvoriť vlastné citlivé informácie typ](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) v UI & zabezpečenia súladu Center.</span><span class="sxs-lookup"><span data-stu-id="1f4c0-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="1f4c0-111">**Vytvorenie vlastných citlivých informácií typu v & zabezpečenia súladu centrum PowerShell**</span><span class="sxs-lookup"><span data-stu-id="1f4c0-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="1f4c0-112">Nakoniec, ak UI neposkytuje všetky možnosti, ktoré potrebujete, môžete [vytvoriť vlastné citlivé informácie typu v & zabezpečenia súladu centrum PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="1f4c0-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="1f4c0-113">Tým začína súbor XML, môžete použiť k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="1f4c0-113">By starting with an XML file, you can use every option available.</span></span>

    