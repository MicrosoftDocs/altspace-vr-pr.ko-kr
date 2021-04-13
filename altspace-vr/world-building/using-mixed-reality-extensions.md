---
title: Mixed Reality 확장 사용
description: 혼합 현실 확장을 사용 하 고 문제를 해결 하 여 AltspaceVR 환경을 확장 하 고 조정 하는 방법을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 혼합 현실, 확장, 문제 해결
ms.openlocfilehash: 498e71c48f7c67abc40ce4f4667c9eeac4c4e73b
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212643"
---
# <a name="using-a-mixed-reality-extension"></a><span data-ttu-id="ec067-104">Mixed Reality 확장 사용</span><span class="sxs-lookup"><span data-stu-id="ec067-104">Using a Mixed Reality Extension</span></span>

<span data-ttu-id="ec067-105">[혼합 현실 확장](https://developer.altvr.com/) (mres)은 원하는 [stargate에서 작업 stargate](https://account.altvr.com/mres/1152987031857529562)에 사용할 수 있는 [앱입니다.](https://account.altvr.com/mres/1173667287173955931)</span><span class="sxs-lookup"><span data-stu-id="ec067-105">[Mixed Reality Extensions](https://developer.altvr.com/) (MREs) are apps you can use in your Worlds from [helmets](https://account.altvr.com/mres/1173667287173955931) to a working [Stargate](https://account.altvr.com/mres/1152987031857529562).</span></span> <span data-ttu-id="ec067-106">이는 프로그래밍 경험이 있는 커뮤니티 멤버가 Altspace을 확장 하 고 단방향 세계 빌더를 사용 하 여 더 많은 대화형 작업을 수행할 수 있는 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-106">This is how community members with programming experience can extend Altspace and one-way World Builders can make their Worlds more interactive.</span></span> <span data-ttu-id="ec067-107">MREs는 전 세계 누구나 사용할 수 있는 반면, 전 세계의 프로그램은 전 세계에 있는 사람을 찾아보고 생성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-107">While MREs can be used by anyone in a World, only people in the World Building Program can browse and spawn MREs in their Worlds.</span></span> 

1. <span data-ttu-id="ec067-108">[웹 사이트](https://account.altvr.com/mres)의 mre 섹션을 탐색 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-108">Browse the MRE section of our [website](https://account.altvr.com/mres).</span></span> <span data-ttu-id="ec067-109">기본적으로 고유한 MREs를 표시 하므로 **Altspace** 를 선택 하 여 공식 mres **를 확인 하 고 커뮤니티** 에서 mres를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-109">By default you'll see your own MREs so select on **Altspace** to see official MREs and **Featured** to see MREs from the community.</span></span> <span data-ttu-id="ec067-110">전 세계에서 사용 하기 전에 모든 MRE를 숙지 하세요.</span><span class="sxs-lookup"><span data-stu-id="ec067-110">Get familiar with any MRE before you use it in your World.</span></span> 
2. <span data-ttu-id="ec067-111">[Memets](https://account.altvr.com/mres/1173667287173955931) mre로 이동 하 여 **클립보드로 복사를** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-111">Navigate to the [Helmets](https://account.altvr.com/mres/1173667287173955931) MRE and select **Copy to Clipboard**.</span></span> 
3. <span data-ttu-id="ec067-112">전 세계를 입력 하 고, 기본 편집기 **> SDK 앱** 을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-112">Enter your World and open the World Editor to **Basics > SDK App**.</span></span> <span data-ttu-id="ec067-113">대상 URI 필드에에 대 한 URL을 붙여 넣고 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-113">Paste in the URL for Helmets into the Target URI field and select **Confirm**.</span></span> <span data-ttu-id="ec067-114">MRE 개체가 나타나고 클라우드에서 실행 되는 MRE에 연결 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-114">The MRE Object should appear and attempt to connect to the MRE that's running in the cloud.</span></span> <span data-ttu-id="ec067-115">이제를 클릭할 수 있는 몇 가지 방법을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-115">You should now see some helmets you can click on.</span></span>
4. <span data-ttu-id="ec067-116">다른 세계 개체와 마찬가지로 MRE를 이동/회전/크기 조정 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-116">Move/rotate/scale the MRE just as you would any other World Object.</span></span>

<span data-ttu-id="ec067-117">축하합니다!</span><span class="sxs-lookup"><span data-stu-id="ec067-117">Congratulations!</span></span> <span data-ttu-id="ec067-118">지금 MREs를 사용 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-118">You're using MREs now--you're so cool!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ec067-119">문제 해결</span><span class="sxs-lookup"><span data-stu-id="ec067-119">Troubleshooting</span></span>

<span data-ttu-id="ec067-120">**MRE가 찡그린를 표시 합니다.**</span><span class="sxs-lookup"><span data-stu-id="ec067-120">**MRE is showing a frowning emoji**</span></span> 
    * <span data-ttu-id="ec067-121">URL이 올바른지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-121">Verify that the URL is correct</span></span>
    * <span data-ttu-id="ec067-122">개체에서 **재생 옵션을** 설정/해제 하 고 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-122">Toggle **Is Playing** option on the Object and choose **confirm**</span></span>
    * <span data-ttu-id="ec067-123">다시 시작</span><span class="sxs-lookup"><span data-stu-id="ec067-123">Try reentering</span></span>

<span data-ttu-id="ec067-124">**Mre가 지연** MRE가 호스트 되는 위치에 따라 몇 가지 네트워크 대기 시간이 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-124">**MRE is lagging** Depending on where an MRE is hosted you may experience some network latency</span></span>

<span data-ttu-id="ec067-125">**Url을 붙여 넣어야 하는 이유는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="ec067-125">**Why do we have to paste URLs?**</span></span>
<span data-ttu-id="ec067-126">나중에 키트에서 아티팩트를 수행 하는 것 처럼 MREs를 관리 하 고 생성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-126">In the future, you can manage and spawn MREs like you do Artifacts from Kits.</span></span> <span data-ttu-id="ec067-127">그때까지 계속 해 서 Url을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec067-127">Until then, we'll continue using URLs</span></span>