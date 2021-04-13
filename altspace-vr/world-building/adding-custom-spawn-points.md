---
title: 사용자 지정 생성 위치 추가
description: AltspaceVR에 대 한 사용자 지정 생성 점수를 만들고 추가 하 고 문제를 해결 하는 방법에 대해 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: spawnpoint, 문제 해결
ms.openlocfilehash: 0f53bdc229eb21e50edef34981c592556236fc55
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212819"
---
# <a name="adding-custom-spawn-points"></a><span data-ttu-id="db446-104">사용자 지정 생성 위치 추가</span><span class="sxs-lookup"><span data-stu-id="db446-104">Adding custom spawn points</span></span>

<span data-ttu-id="db446-105">전 세계에 들어가는 사람들은 전 세계에 배치 될 때 원점 (0, 0, 0)으로 **생성** 되거나 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="db446-105">People entering your World will **spawn** or appear at the origin, position (0,0,0), when they enter your World.</span></span> <span data-ttu-id="db446-106">그러나 사용자가 성의 입구에서 시작 하도록 하려는 경우에는 하나 이상의 생성 점수를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="db446-106">However, you can add one or more Spawn Points if you want to, say, have people start at the entrance to your castle.</span></span> <span data-ttu-id="db446-107">여러 생성 시점을 지정 하는 경우 누군가가 입력 될 때마다 임의로 선택 되며 원본은 포함 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="db446-107">If you specify multiple Spawn Points, one will be randomly chosen whenever someone enters and the origin won't be included.</span></span> <span data-ttu-id="db446-108">세계 편집기를 사용 하는 모든 세계 또는 이벤트에 대 한 생성 지점을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="db446-108">You can manage Spawn Points to any World or Event where your World Editor is enabled.</span></span> <span data-ttu-id="db446-109">사용자가 생성 하는 위치 (위치)와 방향을 제어 합니다 (회전).</span><span class="sxs-lookup"><span data-stu-id="db446-109">You control where people spawn (position) and what direction they'll be facing (rotation).</span></span> <span data-ttu-id="db446-110">생성 지점은 편집 모드 에서만 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="db446-110">Spawn Points will only be visible in Edit Mode.</span></span> 

1. <span data-ttu-id="db446-111">사용자가 생성 하고자 하는 곳 가까이로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-111">Go near the spot where you want people to spawn.</span></span> <span data-ttu-id="db446-112">**세계 편집기 > 기본 사항을** 열고 **잠금 회전이** 선택 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-112">Open **World Editor > Basics** and make sure **Lock Rotation** is checked.</span></span> <span data-ttu-id="db446-113">생성 **지점** 을 선택 하 여 하나를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="db446-113">Select **Spawn Point** to create one.</span></span> <span data-ttu-id="db446-114">원하는 정확한 위치로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-114">Move it to the exact position you want:</span></span>

![세계 편집기 기본 사항 창 열기](images/spawn-points-img-01.png)

2. <span data-ttu-id="db446-116">생성 지점에 대 한 설정 아이콘을 선택 하 고 **회전 > X** 와 **회전 > Z** 가 모두 **0** 인지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-116">Select on the settings icon for the Spawn Point and make sure **Rotation > X** and **Rotation > Z** are both **0**.</span></span> <span data-ttu-id="db446-117">**8.537777745 e-07** 과 같은 작은 숫자인 경우에도 마찬가지입니다.</span><span class="sxs-lookup"><span data-stu-id="db446-117">If they are small numbers like **8.537777745E-07**, that's fine too.</span></span> <span data-ttu-id="db446-118">부동 소수점 숫자를 처리 하는 방법에 대 한 쿼크입니다.</span><span class="sxs-lookup"><span data-stu-id="db446-118">That's a quirk of how floating point numbers are handled:</span></span>

![전역 편집기 설정에서 생성 시점 업데이트](images/spawn-points-img-02.png)

3. <span data-ttu-id="db446-120">**메뉴 > 설정 > 일반 > 다시 입력 > 공간 다시 입력** 을 통해 사용자를 다시 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-120">Reenter your World via **Menu > Settings > General > Reenter Space > Re-Enter**</span></span>
4. <span data-ttu-id="db446-121">새 생성 시점에서 생성 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-121">You should spawn at your new Spawn Point!</span></span>
5. <span data-ttu-id="db446-122">사용자가 다른 방향을 지정 하려면 생성 점에 대 한 설정을 선택 하 고 **회전 > Y** 만 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-122">If you want people to face a different direction, select the settings for the Spawn Point and set **Rotation > Y** only.</span></span> <span data-ttu-id="db446-123">Y를 180로 설정 하 고 X와 Z를 모두 0으로 설정 합니다 (경고: X 및 Z는 다른 사용자를 만들 수 있음).</span><span class="sxs-lookup"><span data-stu-id="db446-123">Try setting Y to 180 and both X and Z to 0 (Warning: X and Z are advanced may make people sick).</span></span> <span data-ttu-id="db446-124">그런 다음 **확인** 을 선택 하 고 전 세계를 다시 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-124">Then select **Confirm** and reenter the World.</span></span> <span data-ttu-id="db446-125">이는 반대 방향으로 생성 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-125">That should spawn you facing the opposite direction.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="db446-126">문제 해결</span><span class="sxs-lookup"><span data-stu-id="db446-126">Troubleshooting</span></span>

<span data-ttu-id="db446-127">**사람들은 계속 원본에서 생성 되나요?**</span><span class="sxs-lookup"><span data-stu-id="db446-127">**People still spawning at the origin?**</span></span>
    * <span data-ttu-id="db446-128">생성 지점이 땅 또는 표면 위에 약간 위에 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-128">Make sure your Spawn Points are slightly above the ground or surface.</span></span> <span data-ttu-id="db446-129">생성 지점이 다른 개체와 겹치는 경우에는 사용자가 기본 위치인 원본을 생성 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-129">If the Spawn Point is overlapping other objects, people spawn at the default location, the origin.</span></span> <span data-ttu-id="db446-130">이는 개체 내의 생성 지점과 사용자의 높이가 변하는 경우에 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="db446-130">This can happen if the Spawn Point inside an object and the height of person varies.</span></span> 
    * <span data-ttu-id="db446-131">**메뉴 > 설정 > 중간 > 공간 재설정** 을 통해 전 세계를 재설정 해 보세요.</span><span class="sxs-lookup"><span data-stu-id="db446-131">Try resetting your World via **Menu > Settings > Moderate > Reset Space**</span></span>

<span data-ttu-id="db446-132">**여러 생성 지점이 있지만 동일한 위치에서 계속 생성 되나요?**</span><span class="sxs-lookup"><span data-stu-id="db446-132">**Have multiple Spawn Points but still spawning in the same place?**</span></span>
<span data-ttu-id="db446-133">Unlucky 일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="db446-133">You might be unlucky--it's random after all.</span></span> <span data-ttu-id="db446-134">오류가 발생 한 것으로 간주 하기 전에 최소 5 번의 다시 시도를 시도 하세요.</span><span class="sxs-lookup"><span data-stu-id="db446-134">Try a few reentering at least five times before assuming there's an error.</span></span> 

<span data-ttu-id="db446-135">**사람들은 불편 하거나 그 헤드를 기울어진 것입니다** . **잠금 회전** 을 확인 하거나 회전을 위해 X 및 Z 값을 설정 하는 것을 잊은 경우</span><span class="sxs-lookup"><span data-stu-id="db446-135">**People are uncomfortable or their head is tilted** You may have forgotten to check **Lock Rotation** or set the X and Z value for Rotation.</span></span> <span data-ttu-id="db446-136">Exotic 환경을 구축 하지 않는 한 일반적으로 0으로 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="db446-136">Those should usually be set to 0 unless you're building an exotic World.</span></span> 

<span data-ttu-id="db446-137">**사용자가 생성 하는 경우**</span><span class="sxs-lookup"><span data-stu-id="db446-137">**People falling when they spawn?**</span></span>
<span data-ttu-id="db446-138">생성 지점 위치를 개체 위에 너무 높게 설정 하지 마십시오.</span><span class="sxs-lookup"><span data-stu-id="db446-138">Don't set the Spawn Point position too high above an object.</span></span> <span data-ttu-id="db446-139">너무 멀리 있으면 원본에서 respawned 됩니다.</span><span class="sxs-lookup"><span data-stu-id="db446-139">If they fall too far, they'll be respawned at the origin.</span></span>