---
title: 전역 역할 부여
description: 역할 및 기능 시스템에 대해 알아보고 AltspaceVR 환경에서 사용자 역할을 제공 하는 방법에 대 한 단계별 지침을 확인 하세요.
ms.date: 03/11/2021
ms.topic: article
keywords: 역할
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212790"
---
# <a name="granting-world-roles"></a><span data-ttu-id="3f12f-104">전역 역할 부여</span><span class="sxs-lookup"><span data-stu-id="3f12f-104">Granting world roles</span></span>

<span data-ttu-id="3f12f-105">Altspace에는 역할 및 기능 시스템이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="3f12f-106">각 사용자는 여러 역할을 가질 수 있으며 해당 역할은 어디에 있는지에 따라 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="3f12f-107">각 역할은 하나 이상의 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="3f12f-108">예를 들어 사용자 고유의 이벤트에 있는 경우 **발표자** 및 **중재자** 역할을 자동으로 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-108">For example, when you're in your own event, you automatically receive the **presenter** and **moderator** roles.</span></span> <span data-ttu-id="3f12f-109">이러한 두 가지 역할을 사용 하 여, 준비를 하 고, 색종이를 출시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span> 

1. <span data-ttu-id="3f12f-110">전 세계를 편집 하 고 아래로 스크롤하여 **VR** 섹션 (전 세계 [관리 방법](managing-worlds.md))으로 스크롤합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-110">Edit your World and scroll down to the **In VR** section ([How to manage Worlds](managing-worlds.md))</span></span>

![세계의 VR 섹션에서 역할 변경](images/granting-roles.png)

2. <span data-ttu-id="3f12f-112">이 세계의 특정 사용자 에게만 특정 역할을 부여 하려면 **역할** 필드를 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-112">Edit the **Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="3f12f-113">예를 들어 **발표자**  +  **중재자** **를 제공** 하 고 calen을 제공 하려는 경우 다음을 추가 하 고 **저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-113">For example, if you want to give me **presenter** + **moderator** and give Calen **moderator**, you would add the following and select **Save**.</span></span> <span data-ttu-id="3f12f-114">형식은 각 줄에서 **{role}, {username 또는 email}** 입니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-114">The format is **{role},{username or email}** on each line.</span></span> <span data-ttu-id="3f12f-115">사용자 이름은 대/소문자를 구분 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-115">Username is case-insensitive.</span></span> 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. <span data-ttu-id="3f12f-116">**편집** 을 다시 선택 하면 역할 필드 위에 다음이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-116">If you select **Edit** again, you should see the following above the Roles field.</span></span> <span data-ttu-id="3f12f-117">데이터베이스에서 업데이트 된 것을 알 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-117">That's how you know updated in the database.</span></span>

```
Presenters: jimmy
Moderators: jimmy,calen
```

* <span data-ttu-id="3f12f-118">이 변경 내용이 Altspace에 적용 되려면 전 세계를 다시 설정 하 여 모든 사용자가 다시 참가 하도록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-118">In order for the change to take effect in Altspace, you should reset the world, forcing everyone to rejoin.</span></span> <span data-ttu-id="3f12f-119">아래에는 역할의 전체 목록이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-119">There's a full list of roles below.</span></span>

4. <span data-ttu-id="3f12f-120">전 세계에 참가 하는 모든 역할에 역할을 부여 하려면 **컨텍스트 역할** 필드를 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-120">Edit the **Contextual Roles** field if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="3f12f-121">예를 들어 사용자가 폰를 사용 하 여 서로를 대상으로 하는 동안 서로를 들 여 받을 수 있도록 하려면 다음을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-121">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="3f12f-122">**업데이트** 를 선택한 후 전 세계를 다시 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-122">After you select **Update**, reset the World.</span></span> <span data-ttu-id="3f12f-123">이는이 세계에만 영향을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-123">This will only affect this World.</span></span> <span data-ttu-id="3f12f-124">역할을 전체 Universe에 부여 하려면 Universe에서 동일한 필드를 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-124">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> 

## <a name="roles"></a><span data-ttu-id="3f12f-125">역할</span><span class="sxs-lookup"><span data-stu-id="3f12f-125">Roles</span></span> 

* <span data-ttu-id="3f12f-126">스테이지에 있을 수 있는 것과 같은 **발표자** 기능</span><span class="sxs-lookup"><span data-stu-id="3f12f-126">**Presenter** - abilities like being able to be on stage</span></span>
* <span data-ttu-id="3f12f-127">**중재자** -decorum 유지 관리 **와 같은 기능**</span><span class="sxs-lookup"><span data-stu-id="3f12f-127">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="3f12f-128">**Terraformer** -전 세계 편집기를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-128">**Terraformer** - ability to use the World Editor</span></span>
* <span data-ttu-id="3f12f-129">**파일럿** -즉석 모드를 전환 하 고 6DOF 비행 도구를 생성 하는 기능</span><span class="sxs-lookup"><span data-stu-id="3f12f-129">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="3f12f-130">**Megaphone_only** -전 세계 어디에서 든 사용자의 귀를 이야기 하는 기능</span><span class="sxs-lookup"><span data-stu-id="3f12f-130">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="3f12f-131">**Showcase_new_sdk** -MRE sdk 앱을 생성 하는 기능</span><span class="sxs-lookup"><span data-stu-id="3f12f-131">**Showcase_new_sdk** - ability to spawn MRE SDK apps</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="3f12f-132">문제 해결</span><span class="sxs-lookup"><span data-stu-id="3f12f-132">Troubleshooting</span></span>

<span data-ttu-id="3f12f-133">**역할을 삭제할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="3f12f-133">**Can I delete roles?**</span></span>
<span data-ttu-id="3f12f-134">이제는 폼에서 제공 되지 않으므로 help.altvr.com에서 파일 a를 지원 요청 합니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-134">Not from the form right now so file a Support request at help.altvr.com and we'll take care of it for you</span></span>

<span data-ttu-id="3f12f-135">**다른 지역에서 가져올 때 역할이 복사 되나요?**</span><span class="sxs-lookup"><span data-stu-id="3f12f-135">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="3f12f-136">아니요. 역할은 복사 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3f12f-136">No, roles aren't copied</span></span>