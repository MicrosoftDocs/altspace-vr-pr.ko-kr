---
title: 세계 백업
description: AltspaceVR 세계의 백업 스냅숏을 만들고, 관리 하 고, 문제를 해결 하는 방법에 대해 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 저장
ms.openlocfilehash: fdef692c737bf2f92db315e04556831d60c2f377
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212659"
---
# <a name="backing-up-your-worlds"></a><span data-ttu-id="b1509-104">세계 백업</span><span class="sxs-lookup"><span data-stu-id="b1509-104">Backing up your worlds</span></span>

<span data-ttu-id="b1509-105">백업은 특정 시점에서 전 세계의 모든 개체에 대 한 "스냅숏" 또는 레코드입니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-105">A Backup is a “snapshot” or record of all the objects in a World at a specific point in time.</span></span> <span data-ttu-id="b1509-106">꿈 집을 작성 하 고 있으며, 언젠가는 실수로 실내를 삭제 한 경우를 가정해 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-106">Suppose you’re building your Dream House and one day you accidentally deleted the living room.</span></span> <span data-ttu-id="b1509-107">전 세계의 전 세계 백업을 만든 경우 해당 특정 백업을 복원 하 고, 전 세계를 재설정 하 고, 비상 공격을 방지할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-107">If you had created a Backup of your World the day before, you could restore that particular backup, reset your World, and avoid a panic attack.</span></span> <span data-ttu-id="b1509-108">또는 모든 계절에 대해 cabin의 버전을 보유 하 고 있으며, 백업으로 전환 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-108">Or perhaps you have a version of your cabin-in-the-woods for every season and you like to switch back and forth between them—you can do that with Backups.</span></span> <span data-ttu-id="b1509-109">각 백업은 단일 세계에 고유 하며 변환 (위치, 회전, 크기 조정) 뿐만 아니라 개체에 대 한 기타 설정도 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-109">Each Backup is specific to a single World and contains not only the transforms (position, rotation, scale) but also other settings on the objects.</span></span> <span data-ttu-id="b1509-110">전 세계에 대해 만들 수 있는 백업 수에는 제한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-110">There's no limit to the number of Backups you can create for a World.</span></span>  

## <a name="whats-included-in-a-backup"></a><span data-ttu-id="b1509-111">백업에는 무엇이 포함 되나요?</span><span class="sxs-lookup"><span data-stu-id="b1509-111">What’s included in a Backup?</span></span>

<span data-ttu-id="b1509-112">현재 백업에는 세계 편집기를 사용 하 여 생성할 수 있는 대부분의 항목이 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-112">A Backup currently includes most things you can spawn with the World Editor:</span></span>
* <span data-ttu-id="b1509-113">아티팩트 (키트 개체)</span><span class="sxs-lookup"><span data-stu-id="b1509-113">Artifacts (Kit objects)</span></span>
* <span data-ttu-id="b1509-114">레이블</span><span class="sxs-lookup"><span data-stu-id="b1509-114">Labels</span></span>
* <span data-ttu-id="b1509-115">Teleporters</span><span class="sxs-lookup"><span data-stu-id="b1509-115">Teleporters</span></span>
* <span data-ttu-id="b1509-116">생성 점수</span><span class="sxs-lookup"><span data-stu-id="b1509-116">Spawn Points</span></span>
* <span data-ttu-id="b1509-117">사진</span><span class="sxs-lookup"><span data-stu-id="b1509-117">Photos</span></span>
* <span data-ttu-id="b1509-118">MRE SDK 앱</span><span class="sxs-lookup"><span data-stu-id="b1509-118">MRE SDK Apps</span></span>
* <span data-ttu-id="b1509-119">네이티브 앱 (예: 현실을 Holograms)</span><span class="sxs-lookup"><span data-stu-id="b1509-119">Native Apps (for example, Holograms Against Reality)</span></span>

<span data-ttu-id="b1509-120">다음은 포함 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-120">The following isn’t included:</span></span>

* <span data-ttu-id="b1509-121">레이아웃 재정의</span><span class="sxs-lookup"><span data-stu-id="b1509-121">Layout overrides</span></span>
* <span data-ttu-id="b1509-122">Skyboxes 및 앰비언트 소리</span><span class="sxs-lookup"><span data-stu-id="b1509-122">Skyboxes and ambient sound</span></span>
* <span data-ttu-id="b1509-123">템플릿</span><span class="sxs-lookup"><span data-stu-id="b1509-123">Templates</span></span>
* <span data-ttu-id="b1509-124">지침</span><span class="sxs-lookup"><span data-stu-id="b1509-124">Instructions</span></span>
* <span data-ttu-id="b1509-125">세계 역할 및 컨텍스트 역할</span><span class="sxs-lookup"><span data-stu-id="b1509-125">World roles and contextual roles</span></span>

## <a name="managing-backups"></a><span data-ttu-id="b1509-126">백업 관리</span><span class="sxs-lookup"><span data-stu-id="b1509-126">Managing Backups</span></span>

<span data-ttu-id="b1509-127">세계 편집기/Altspace를 열고 "백업"을 클릭 하 여 백업을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-127">You can create a Backup by opening your World Editor / Altspace and clicking on “Backups”.</span></span> <span data-ttu-id="b1509-128">첫 번째 단추는 "새 백업" 단추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-128">The first button will be the “New Backup” button.</span></span> <span data-ttu-id="b1509-129">백업을 만들 때 짧은 이름을 입력 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-129">When creating a Backup, you’ll be asked to provide a short name.</span></span> <span data-ttu-id="b1509-130">이 옵션은 선택 사항 이지만 빠르게 혼란 스 러 울 수 있으므로 매우 권장 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-130">This is optional but highly recommended because it will get confusing fast.</span></span> <span data-ttu-id="b1509-131">기존 백업은 "만들기" 단추 뒤에 나열 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-131">Existing backups will be listed after the “Create” button.</span></span> <span data-ttu-id="b1509-132">기존 백업을 클릭 하면 복원이 시작 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-132">Clicking on an existing Backup will start a restore.</span></span> <span data-ttu-id="b1509-133">백업을 복원할 때 전 세계는 몇 분 후에 다시 설정 되지만 변경 내용은 반영 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-133">When restoring a Backup, your World will reset after a few moments but you may not see the changes reflected.</span></span> <span data-ttu-id="b1509-134">1 ~ 2 분 정도 기다렸다가 다시 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-134">Wait a minute or two and reset your World again.</span></span> <span data-ttu-id="b1509-135">**현재 VR에서 백업을 편집 하거나 삭제할 수 있는 방법은 없습니다**.</span><span class="sxs-lookup"><span data-stu-id="b1509-135">**There's currently no way to edit or delete a Backup in VR**.</span></span> <span data-ttu-id="b1509-136">지금은 웹 사이트에서 백업을 관리 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-136">You'll need to manage your Backups on our website for now.</span></span> <span data-ttu-id="b1509-137">(VR의 백업 관리가 곧 개선 될 예정입니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-137">(Backup management in VR will be improved soon.</span></span> <span data-ttu-id="b1509-138">그 동안에는 잘 해 주세요.</span><span class="sxs-lookup"><span data-stu-id="b1509-138">In the meantime, bear with us).</span></span>

<span data-ttu-id="b1509-139">웹 사이트에서 백업을 관리 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-139">To manage your Backups on our website:</span></span>

1. <span data-ttu-id="b1509-140">[> 광산](https://account.altvr.com/users/sign_in)으로 이동 하 여 전 세계를 찾고 관리자 컨트롤에서 "백업"을 누릅니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-140">Navigate to [Worlds > Mine](https://account.altvr.com/users/sign_in), find your World, and press “Backups” in the Administrator Controls:</span></span>

![백업 패널이 열려 있는 세계 웹 사이트의 관리자 컨트롤](images/world-backup-img-01.png)

2. <span data-ttu-id="b1509-142">백업을 만들고, 편집 하 고, 삭제 하 고, 포함 된 개체 수를 확인 하 고, 미리 보기 이미지를 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-142">You can create, edit, and delete your Backups, check how many objects are inside, and even upload a preview image:</span></span> 

![만들기, 편집 및 삭제 명령이 강조 표시 된 백업 창](images/world-backup-img-02.png)

<span data-ttu-id="b1509-144">백업 수에는 제한이 없으며 더 많은 백업이 있으면 전 세계의 성능에 영향을 주지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-144">There's no limit to the number of Backups and having more Backups won't impact the performance of your World.</span></span>

## <a name="other-ways-to-back-up-your-worlds"></a><span data-ttu-id="b1509-145">사용자 환경을 백업 하는 다른 방법</span><span class="sxs-lookup"><span data-stu-id="b1509-145">Other ways to back up your Worlds</span></span>

* <span data-ttu-id="b1509-146">다른 환경을 만들고, 고급 옵션을 표시 하 고, 전 세계에서 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-146">Create another World, Show Advanced Options, and Import from World.</span></span> <span data-ttu-id="b1509-147">드롭다운 메뉴에서 새로 백업할 전 세계를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-147">Choose the World you want to back up from the dropdown menu into the new one.</span></span> <span data-ttu-id="b1509-148">가져오기에 대 한 제한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-148">There no limit for imports.</span></span>
* <span data-ttu-id="b1509-149">Unity 업 로더를 사용 하는 경우 버전 제어를 사용 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-149">If you’re using the Unity Uploader, we strongly recommend you use version control.</span></span> <span data-ttu-id="b1509-150">예: [Unity 용 Github](https://unity.github.com).</span><span class="sxs-lookup"><span data-stu-id="b1509-150">For example, [Github for Unity](https://unity.github.com).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="b1509-151">문제 해결</span><span class="sxs-lookup"><span data-stu-id="b1509-151">Troubleshooting</span></span>

<span data-ttu-id="b1509-152">**도움말! 실수로 백업을 복원 하 고 작업** 을 걱정할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-152">**Help! I accidentally restored a Backup and my work is gone** Don’t worry.</span></span> <span data-ttu-id="b1509-153">이전 백업을 복원 하기 전에 새 백업을 자동으로 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-153">We automatically create a new Backup before restoring old one.</span></span> <span data-ttu-id="b1509-154">올바른 타임 스탬프를 사용 하 여 **auto** 로 시작 하는 이름을 가진 항목을 찾아서 복원 합니다 (예: **auto 2019-01-14T08:23:33-08:00**).</span><span class="sxs-lookup"><span data-stu-id="b1509-154">Look for one with a name starting with **Auto** with the right timestamp and restore that one (for example, **Auto 2019-01-14T08:23:33-08:00**).</span></span>  <span data-ttu-id="b1509-155">작동 하지 않는 경우 [지원 요청](https://help.altvr.com/hc/requests/new) 제출</span><span class="sxs-lookup"><span data-stu-id="b1509-155">If that doesn’t work submit a [Support request](https://help.altvr.com/hc/requests/new)</span></span>

<span data-ttu-id="b1509-156">**백업을 복원 했 고 일부 개체가 누락** 되었습니다. 사진이 있는 경우 사진이 삭제 되었습니까?</span><span class="sxs-lookup"><span data-stu-id="b1509-156">**I restored a Backup and some objects are missing** If any were photos, were those photos deleted?</span></span> <span data-ttu-id="b1509-157">개인 정보 보호를 위해 삭제 된 사진은 복원할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-157">We can’t restore deleted photos for privacy reasons.</span></span> <span data-ttu-id="b1509-158">조사할 수 있도록 [지원 요청](https://help.altvr.com/hc/requests/new) 제출</span><span class="sxs-lookup"><span data-stu-id="b1509-158">Submit a [Support request](https://help.altvr.com/hc/requests/new) so we can investigate</span></span>

<span data-ttu-id="b1509-159">**변경 내용이 표시 되지 않습니다** . 백업은 개체의 수에 따라 복원 하는 데 몇 분 정도 걸릴 수 있으므로 비동기식으로 복원 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-159">**I don’t see any changes** Backups are restored asynchronously meaning they can take a few minutes to restore depending on the number of objects.</span></span> <span data-ttu-id="b1509-160">전 세계를 재설정 하 고 몇 분 후에 아무것도 표시 되지 않으면 다시 설정 해 보세요.</span><span class="sxs-lookup"><span data-stu-id="b1509-160">Remember to reset your World and if you don’t see anything after a few minutes try resetting again.</span></span> <span data-ttu-id="b1509-161">나중에 복원 프로세스의 상태에 대 한 더 많은 피드백을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1509-161">In the future, we can provide more feedback on the status of the restoration process</span></span>