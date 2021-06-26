---
title: 전역 역할 부여
description: 역할 및 기능 시스템에 대해 알아보고 AltspaceVR 환경에서 사용자 역할을 제공 하는 방법에 대 한 단계별 지침을 확인 하세요.
ms.date: 04/14/2021
ms.topic: article
keywords: 역할
ms.openlocfilehash: 3a1d0f138b29fe545f52d851ff00062f156a860e
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923198"
---
# <a name="granting-world-roles"></a><span data-ttu-id="c8978-104">전역 역할 부여</span><span class="sxs-lookup"><span data-stu-id="c8978-104">Granting world roles</span></span>

<span data-ttu-id="c8978-105">Altspace에는 역할 및 기능 시스템이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="c8978-106">각 사용자는 여러 역할을 가질 수 있으며 해당 역할은 어디에 있는지에 따라 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="c8978-107">각 역할은 하나 이상의 기능을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="c8978-108">예를 들어 사용자 고유의 이벤트에 있는 경우 자동으로 **호스트** 및 **중재자** 역할을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-108">For example, when you're in your own event, you automatically receive the **host** and **moderator** roles.</span></span> <span data-ttu-id="c8978-109">이러한 두 가지 역할을 사용 하 여, 준비를 하 고, 색종이를 출시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span>

1. <span data-ttu-id="c8978-110">전 세계를 편집 하 고 상황에 맞는 **역할** 의 오른쪽 열을 확인 합니다 ([세계를 관리 하는 방법](managing-worlds.md)).</span><span class="sxs-lookup"><span data-stu-id="c8978-110">Edit your World and look over to the right column for **Contextual Roles** ([How to manage Worlds](managing-worlds.md))</span></span>

![세계의 상황별 역할 섹션에서 역할 변경](images/granting-roles.png)

2. <span data-ttu-id="c8978-112">이 세계의 특정 사용자 에게만 특정 역할을 부여 하려면 **상황별 역할** 필드에서 **사용자 추가** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-112">Click **Add User** under the **Contextual Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="c8978-113">예를 들어 **호스트**  +  **중재자** 를 제공 하려는 경우 위에를 추가 하 고 **저장** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-113">For example, if you want to give me **host** + **moderator**, you would add the above and select **Save**.</span></span> <span data-ttu-id="c8978-114">형식은 **username** 이며, username은 대/소문자를 구분 하지 않고, **드롭다운 메뉴에서** 역할을 선택 하 고, 사용자 추가를 여러 번 클릭 하 여 사용자를 더 추가 하 고 **업데이트** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-114">The format is **username**, username is case-insensitive, choose the role from the dropdown menu **Terraformer**, click Add User multiple times to keeping adding more users and then click **Update**.</span></span>

* <span data-ttu-id="c8978-115">이 변경 내용을 Altspace에 적용 하려면 모든 사용자가 다시 참가 하도록 하거나 새 역할을 가진 각 사용자가 전 세계에 다시 참가 하도록 하는 공간을 다시 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-115">In order for the change to take effect in Altspace, you should Reset Space the world forcing everyone to rejoin or have each user with a new role rejoin the world.</span></span>

3. <span data-ttu-id="c8978-116">에서 전 세계에 참가 하는 모든 역할에 역할을 부여 하려는 경우에는 **VR** 섹션에서 **기본 상황별 역할** 필드를 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-116">Edit the **Default Contextual Roles** field, under the **In VR** section, if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="c8978-117">예를 들어 사용자가 폰를 사용 하 여 서로를 대상으로 하는 동안 서로를 들 여 받을 수 있도록 하려면 다음을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-117">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="c8978-118">**업데이트** 를 선택한 후 전 세계 공간을 다시 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-118">After you select **Update**, Reset Space in the World.</span></span> <span data-ttu-id="c8978-119">이는이 세계에만 영향을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-119">This will only affect this World.</span></span> <span data-ttu-id="c8978-120">역할을 전체 Universe에 부여 하려면 Universe에서 동일한 필드를 편집 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-120">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> <span data-ttu-id="c8978-121">이벤트에 대 한 모든 사용자가 이러한 역할을 갖도록 하려면 이벤트 자체의 **기본 Contexual 역할** 에이를 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-121">The same goes for events, if you want everyone in your event to have these roles you'll need to add this to the **Default Contexual Roles** of the event itself.</span></span>

## <a name="roles"></a><span data-ttu-id="c8978-122">역할</span><span class="sxs-lookup"><span data-stu-id="c8978-122">Roles</span></span>

* <span data-ttu-id="c8978-123">**Megaphone_only** -전 세계 어디에서 든 사용자의 귀를 이야기 하는 기능</span><span class="sxs-lookup"><span data-stu-id="c8978-123">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="c8978-124">**중재자** -decorum 유지 관리 **와 같은 기능**</span><span class="sxs-lookup"><span data-stu-id="c8978-124">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="c8978-125">**파일럿** -즉석 모드를 전환 하 고 6DOF 비행 도구를 생성 하는 기능</span><span class="sxs-lookup"><span data-stu-id="c8978-125">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="c8978-126">단계에 있을 수 있는 것과 같은 **호스트** 기능, 폰</span><span class="sxs-lookup"><span data-stu-id="c8978-126">**Host** - abilities like being able to be on stage, have megaphone</span></span>
* <span data-ttu-id="c8978-127">**Terraformer** -([이벤트, 환경, 그룹 및 AltspaceVR의 역할](../getting-started/roles.md))에 대 한 자세한 정보를 제공 하는 세계 편집기를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-127">**Terraformer** - ability to use the World Editor More information about ([Roles in events, worlds, groups, and in AltspaceVR](../getting-started/roles.md))</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c8978-128">문제 해결</span><span class="sxs-lookup"><span data-stu-id="c8978-128">Troubleshooting</span></span>

<span data-ttu-id="c8978-129">**역할을 삭제할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="c8978-129">**Can I delete roles?**</span></span>
<span data-ttu-id="c8978-130">예, 전 세계를 편집 하 고 삭제할 역할 아래에서 **제거** 를 클릭 한 후 **업데이트** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-130">Yes, edit your world, click **Remove** below the role you'd like to delete and click **Update**</span></span>

<span data-ttu-id="c8978-131">**다른 지역에서 가져올 때 역할이 복사 되나요?**</span><span class="sxs-lookup"><span data-stu-id="c8978-131">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="c8978-132">아니요. 역할은 복사 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c8978-132">No, roles aren't copied</span></span>