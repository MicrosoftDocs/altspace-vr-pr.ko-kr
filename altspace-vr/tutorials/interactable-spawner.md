---
title: Interactables Spawner 사용
description: Interactables spawner을 만들고, 사용 하 고, 사용자 지정 하 여 AltspaceVR 공간에 항목을 저장 하는 방법을 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: spawner, 상호 작용, 사용자 지정
ms.openlocfilehash: 7f4b87591b2e11b2084af4d2bf83748ed51fd193
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213552"
---
# <a name="using-the-interactables-spawner"></a><span data-ttu-id="fe0d4-104">Interactables Spawner 사용</span><span class="sxs-lookup"><span data-stu-id="fe0d4-104">Using the Interactables Spawner</span></span>

<span data-ttu-id="fe0d4-105">Interactables Spawner를 사용 하면 이벤트, 세계 또는 홈 공간에 interactable 항목을 삽입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-105">The Interactables Spawner allows you to place interactable items in your event, world, or home-space.</span></span> <span data-ttu-id="fe0d4-106">이 기능은 현재 [초기 액세스 프로그램](../world-building/early-access.md) 의 일부 이며 주 메뉴를 통해 옵트인 한 경우에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-106">This feature is currently part of our [Early Access Program](../world-building/early-access.md) and won't be available unless you've opted in through your Main Menu.</span></span>

> [!NOTE]
> <span data-ttu-id="fe0d4-107">이 기능을 계속 해 서 실험 하는 동안 너무 많은 상호 중단을 생성 하면 사용자 환경이 나 이벤트의 성능에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-107">While we continue to pilot this feature please be aware that spawning too many interactables may affect the performance of your environment or event.</span></span> 

## <a name="creating-an-interactable"></a><span data-ttu-id="fe0d4-108">Interactable 만들기</span><span class="sxs-lookup"><span data-stu-id="fe0d4-108">Creating an interactable</span></span>

<span data-ttu-id="fe0d4-109">개체를 interactable 개체로 변환 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-109">To turn your object into an interactable object:</span></span>

1. <span data-ttu-id="fe0d4-110">개체를 공간에 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-110">Place the object in your space.</span></span>
2. <span data-ttu-id="fe0d4-111">그런 다음 개체 목록에서 항목을 찾고 옆의 **기어 아이콘** 을 선택 하 여 해당 설정을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-111">Then, find the entry in the object list, and select the **gear icon** next to it to open its settings:</span></span>

![개체 목록이 강조 표시 된 세계 편집기 열기](images/interactables-spawner-img-01.png)

<span data-ttu-id="fe0d4-113">설정 페이지에서 새 확인란 **"object spawner"** 를 찾을 수 있습니다 .이 확인란을 사용 하 여 interactable 개체로 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-113">On the settings page you’ll find a new checkbox **“Object spawner“**, which is used to make it an interactable object.</span></span>

1. <span data-ttu-id="fe0d4-114">확인란을 선택 하 고 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-114">Check the box and select **confirm**.</span></span>
2. <span data-ttu-id="fe0d4-115">편집 모드에 있는 동안에는 공간에서 개체의 생성 위치를 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-115">While in edit mode, you can move around the object’s spawn location in the space.</span></span>
3. <span data-ttu-id="fe0d4-116">항목 상호 작용을 사용 하려면 **편집 모드를 종료** 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-116">**Exit edit mode** to enable item interaction.</span></span>

![AltspaceVR 앱에서 열린 아티팩트 업데이트 창](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a><span data-ttu-id="fe0d4-118">기타 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="fe0d4-118">Other customizations</span></span>

<span data-ttu-id="fe0d4-119">**"Object spawner"** 를 사용 하도록 설정한 후 해당 개체의 속성으로 돌아가서 생성 된 개체가 동작 하는 방식에 적용할 수 있는 추가 설정이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-119">After enabling **“Object spawner”** when you go back into the properties for that object, there will be an extra setting you can apply to how the spawned object behaves.</span></span>

> [!NOTE]
> <span data-ttu-id="fe0d4-120">Interactable 개체 크기 조정: 개체를 처음으로 선택 하기 전에 전 세계에 표시 되는 개체의 크기를 나타내는 "Scale"과 비교 하 여 개체를 선택할 때 개체의 소수 자릿수를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-120">Interactable object scale: This sets the scale of the object when it gets picked up, compared to “Scale” which is the scale of how the object appears in the world prior to picking it up for the first time.</span></span>

<span data-ttu-id="fe0d4-121">키트 작성자는 AltspaceVR가 실행 되는 동안 키트의 변경 내용이 적용 되지 않을 수 있습니다. AltspaceVR를 다시 시작할 때까지 적용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-121">Kit makers may notice that changes to your Kit while AltspaceVR is running won't take effect until you restart AltspaceVR.</span></span>

<span data-ttu-id="fe0d4-122">최근 환경 **다시 로드** 라는 **일반 설정** 탭 아래에 단추를 추가 했습니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-122">Recently we’ve added a button under the **Moderate Settings** tab called **Reload Worlds Kits**.</span></span> <span data-ttu-id="fe0d4-123">이 단추를 클릭 하면 (사용자만) 공간을 다시 로드 하 여 모든 키트를 다시 로드 합니다. 그러면 AltspaceVR에 있는 동안 업데이트 된 키트의 새 버전만 다운로드 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fe0d4-123">Clicking this button causes (just you) to reenter the space, reloading all Kits again, which will download only new versions of the Kits that have been updated while you were in AltspaceVR.</span></span>

![AltspaceVR 앱에서 일반 설정 패널 열기](images/interactables-spawner-img-03.png)