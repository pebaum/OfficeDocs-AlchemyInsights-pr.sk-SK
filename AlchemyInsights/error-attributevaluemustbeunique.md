---
title: Chyba AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311279"
---
# <a name="error-attributevaluemustbeunique"></a><span data-ttu-id="0260c-102">Chyba: AttributeValueMustBeUnique</span><span class="sxs-lookup"><span data-stu-id="0260c-102">Error: AttributeValueMustBeUnique</span></span>

<span data-ttu-id="0260c-p101">Najčastejším dôvodom pre AttributeValueMustBeUnique chyba je dvoch objektov s rôznymi SourceAnchor (immutableId) majú rovnakú hodnotu pre ProxyAddresses alebo UserPrincipalName atribúty. Opraviť AttributeValueMustBeUnique chyba:</span><span class="sxs-lookup"><span data-stu-id="0260c-p101">The most common reason for the AttributeValueMustBeUnique error is two objects with different SourceAnchor (immutableId) have the same value for the ProxyAddresses and/or UserPrincipalName attributes. To fix the AttributeValueMustBeUnique error:</span></span>
  
1. <span data-ttu-id="0260c-p102">Identifikáciu duplicitných proxyAddresses, userPrincipalName alebo iné hodnoty atribútu, ktorý spôsobuje chybu. Tiež určiť, ktoré objekty dvoch (alebo viacerých) sú zapojené do konfliktu. Správy generované Azure AD pripojiť zdravie pre synchronizáciu môže pomôcť identifikovať dva objekty.</span><span class="sxs-lookup"><span data-stu-id="0260c-p102">Identify the duplicated proxyAddresses, userPrincipalName or other attribute value that's causing the error. Also identify which two (or more) objects are involved in the conflict. The report generated by Azure AD Connect Health for sync can help you identify the two objects.</span></span>
    
2. <span data-ttu-id="0260c-108">Určiť predmet, ktorý by mal mať duplicitné hodnoty aj naďalej a predmet, ktorý by nemal.</span><span class="sxs-lookup"><span data-stu-id="0260c-108">Identify which object should continue to have the duplicated value and which object should not.</span></span>
    
3. <span data-ttu-id="0260c-p103">Odstráňte duplicitné hodnoty objektu, že by nemali mať túto hodnotu. Všimnite si, že by mal urobiť zmeny v adresári kde sa objekt pochádza z. V niektorých prípadoch budete musieť odstrániť objekty v konflikte.</span><span class="sxs-lookup"><span data-stu-id="0260c-p103">Remove the duplicated value from the object that should NOT have that value. Note that you should make the change in the directory where the object is sourced from. In some cases, you may need to delete one of the objects in conflict.</span></span>
    
4. <span data-ttu-id="0260c-112">Ak ste vykonali zmeny v objekte na reklamu, nech Azure AD pripojiť synchronizovať zmeny pre chyby opravené.</span><span class="sxs-lookup"><span data-stu-id="0260c-112">If you made the change in the on premises AD, let Azure AD Connect sync the change for the error to get fixed.</span></span>
    
