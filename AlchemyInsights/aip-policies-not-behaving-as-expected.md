---
title: 'AIP: Politiky sa nesprávajú podľa očakávania'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506573"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="fe601-102">AIP: Politiky sa nesprávajú podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="fe601-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="fe601-103">Azure informácie ochrana: Politiky sa nesprávajú podľa očakávania, nájdete v nasledujúcich častiach odporúčané pokyny pre rôzne problémy s politikou:</span><span class="sxs-lookup"><span data-stu-id="fe601-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="fe601-104">Ak máte problémy s vizuálnymi označeniami, prečítajte si článok [Pri použití vizuálnych označení](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="fe601-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="fe601-105">Ak máte problémy s automatickým označovaním, prečítajte si tému [Konfigurácia podmienok pre automatickú a odporúčanú klasifikáciu služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a o [tom, čo citlivé typy informácií hľadajú.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="fe601-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="fe601-106">Ak máte problémy s natívnou ochranou/pfile, prečítajte si [konfiguráciu rozhrania API súboru](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="fe601-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="fe601-107">Skontrolujte, či používate politiky rozsahu, ktoré nie sú správne nakonfigurované: [Ako nakonfigurovať politiku Azure ochranu informácií pre konkrétnych používateľov pomocou politiky rozsahu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="fe601-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="fe601-108">Ak automatické označovanie nefunguje pre program Outlook pri pripájaní označeného dokumentu, overte, či vlastnosť DRMEncryptProperty nie je definovaná podľa popisu: [Nastavenie databázy Registry správy prístupových práv k informáciám pre zabezpečenie](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="fe601-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="fe601-109">Ak problémy pretrvávajú, zhromažďovať Denníky klienta Azure information protection a pripojiť exportované denníky k tejto letenke.</span><span class="sxs-lookup"><span data-stu-id="fe601-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="fe601-110">Otvorte dokument balíka Office alebo vytvorte nový e-mail v programe Outlook.</span><span class="sxs-lookup"><span data-stu-id="fe601-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="fe601-111">Kliknite na **položku Pomôcť a spätnú**väzbu o ochrane  >  **a citlivosti**.</span><span class="sxs-lookup"><span data-stu-id="fe601-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="fe601-112">Kliknite na **položku Exportovať denníky**.</span><span class="sxs-lookup"><span data-stu-id="fe601-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="fe601-113">Uložte denníky podľa vášho výberu miesta a pripojte ich k tejto žiadosti o službu.</span><span class="sxs-lookup"><span data-stu-id="fe601-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="fe601-114">Ďalšie zdroje:</span><span class="sxs-lookup"><span data-stu-id="fe601-114">Additional resources:</span></span>

- [<span data-ttu-id="fe601-115">Ako nakonfigurovať označenie pre vizuálne značenie Azure informácie ochrany</span><span class="sxs-lookup"><span data-stu-id="fe601-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="fe601-116">Preskúmanie dokumentácie azure information protection</span><span class="sxs-lookup"><span data-stu-id="fe601-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="fe601-117">Používanie menoviek citlivosti v aplikáciách balíka Office</span><span class="sxs-lookup"><span data-stu-id="fe601-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)
