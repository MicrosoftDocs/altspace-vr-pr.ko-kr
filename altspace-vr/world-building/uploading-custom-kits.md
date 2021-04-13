---
title: 사용자 지정 키트 업로드
description: AltspaceVR에서 사용자 지정 키트를 설정, 생성 및 업로드 하는 방법 및 문제 해결 도움말을 확인 하는 방법을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 키트, 업로드, 문제 해결
ms.openlocfilehash: e5a1b9c2ef5339db0cb821cb6f7d21a930416451
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213505"
---
# <a name="uploading-custom-kits"></a><span data-ttu-id="63fc7-104">사용자 지정 키트 업로드</span><span class="sxs-lookup"><span data-stu-id="63fc7-104">Uploading custom kits</span></span>

<span data-ttu-id="63fc7-105">세계 편집기에는 전 세계에서 생성할 수 있는 아티팩트가 포함 된 키트가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-105">The World Editor has Kits containing Artifacts that you can spawn into your World.</span></span> <span data-ttu-id="63fc7-106">예를 들어 [Campfire Kit](https://account.altvr.com/kits/993516233267609824) 에는 다양 한 유형의 트리가 있습니다. 각 트리 유형은 아티팩트입니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-106">For example, the [Campfire Kit](https://account.altvr.com/kits/993516233267609824) has many types of trees--each type of tree is an Artifact.</span></span> <span data-ttu-id="63fc7-107">사용자 고유의 키트를 만들려면 Unity AssetBundles을 만들고 각 아티팩트에 대 한 Unity Prefab 포함 된 .zip 파일을 업로드 하 고 웹 사이트에 각 아티팩트를 등록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-107">To create your own Kit, you have to create Unity AssetBundles and upload a .zip file containing a Unity Prefab for each Artifact and register each Artifact on our website.</span></span> <span data-ttu-id="63fc7-108">다행히 커뮤니티 중심 Unity 업 로더는 대부분의 워크플로를 자동화 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-108">Fortunately, the community-driven Unity Uploader automates most of the workflow.</span></span> <span data-ttu-id="63fc7-109">업로드 되 면 사용자의 사용자 키트에서 개체를 생성할 수 있으며, 다른 사용자가 자동으로 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-109">Once uploaded, you can spawn objects from your own Kits in your Worlds and other users can automatically see them.</span></span> <span data-ttu-id="63fc7-110">나중에 친구 또는 전체 커뮤니티를 포함 하 여 키트를 공유할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-110">Later, you can share your Kit with your friends or even with the entire Community by being featured.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63fc7-111">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="63fc7-111">Prerequisites</span></span>

1. [<span data-ttu-id="63fc7-112">Unity 허브 및 Unity 설치</span><span class="sxs-lookup"><span data-stu-id="63fc7-112">Install Unity Hub and Unity</span></span>](world-building-toolkit-getting-started.md)
2. <span data-ttu-id="63fc7-113">최신 버전의 [Unity 업 로더](https://altvr.com/download-latest-unity-uploader/) 다운로드</span><span class="sxs-lookup"><span data-stu-id="63fc7-113">Download the latest version of the [Unity Uploader](https://altvr.com/download-latest-unity-uploader/)</span></span>

## <a name="setup"></a><span data-ttu-id="63fc7-114">설치 프로그램</span><span class="sxs-lookup"><span data-stu-id="63fc7-114">Setup</span></span> 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. <span data-ttu-id="63fc7-115">[> 키트](https://account.altvr.com/kits) 의 웹 사이트에서 키트 만들기</span><span class="sxs-lookup"><span data-stu-id="63fc7-115">Create a Kit on our website at [Worlds > Kits](https://account.altvr.com/kits)</span></span>
2. <span data-ttu-id="63fc7-116">브라우저의 주소 표시줄에 있는 키트 ID를 클립보드로 복사 합니다 .이 단계는 업 로더 버전 0.9 이상에서 더 쉽게 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-116">Copy the Kit ID from your browser's address bar to your clipboard (this step will be easier in Uploader versions 0.9+)</span></span>
3. <span data-ttu-id="63fc7-117">새 Unity 프로젝트 만들기</span><span class="sxs-lookup"><span data-stu-id="63fc7-117">Create a new Unity Project</span></span>
4. <span data-ttu-id="63fc7-118">패키지를 두 번 클릭 하 여 Unity 업 로더 가져오기</span><span class="sxs-lookup"><span data-stu-id="63fc7-118">Import the Unity Uploader by double-clicking the package</span></span>

![가져온 unity 업 로더 패키지](images/custom-kits-img-01.png)

5. <span data-ttu-id="63fc7-120">Altspace 전자 메일 및 암호를 사용 하 여 업 로더에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-120">Sign in to the Uploader with your Altspace email and password</span></span>

![Unity의 AltspaceVR 로그인 인터페이스](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a><span data-ttu-id="63fc7-122">키트 생성 및 업로드</span><span class="sxs-lookup"><span data-stu-id="63fc7-122">Generate and upload your kit</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. <span data-ttu-id="63fc7-123">키트 **폴더 이름** 에 키트 id를 사용 하 여 접두사 및 테마 (예: **1137484494681408069_pirates**)로 입력 하 고 키트 **자산 이름** 에 키트 id를 접두사로 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-123">Fill in **Kit Folder Name** with your Kit ID as the prefix and a theme (for example, **1137484494681408069_pirates**) and fill in **Kit Asset Name** with your Kit ID as the prefix.</span></span> <span data-ttu-id="63fc7-124">모든 자산에는이 접두사가 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-124">All the assets will need to have this prefix.</span></span>

![키트 폴더 이름을 사용 하는 Unity의 AltspaceVR 인터페이스](images/custom-kits-img-03.png)

2. <span data-ttu-id="63fc7-126">각 아티팩트 또는 아티팩트 집합:</span><span class="sxs-lookup"><span data-stu-id="63fc7-126">For each Artifact or set of Artifacts:</span></span>
* <span data-ttu-id="63fc7-127">원본 Prefab를 계층 탭으로 끌어 옵니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-127">Drag your source Prefab(s) into the Hierarchy tab</span></span>
* <span data-ttu-id="63fc7-128">집합에 포함 하려는 항목을 선택 합니다. 예를 들어</span><span class="sxs-lookup"><span data-stu-id="63fc7-128">Select the ones you want to include in a set, say five types of barrels</span></span>
* <span data-ttu-id="63fc7-129">**배럴** 을 사용 하 여 **키트 자산 이름** 업데이트</span><span class="sxs-lookup"><span data-stu-id="63fc7-129">Update the **Kit Asset Name** with **barrel**</span></span>
* <span data-ttu-id="63fc7-130">**GameObject를 키트 Prefab로 변환을 선택 합니다** .</span><span class="sxs-lookup"><span data-stu-id="63fc7-130">Select **Convert GameObject(s) to Kit Prefab**</span></span>
* <span data-ttu-id="63fc7-131">새 Prefabs 및 스크린샷이 자산/Prefabs 폴더에 만들어졌는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-131">Verify that new Prefabs and Screenshots were created in the Assets/Prefabs folder</span></span>

![아티팩트가 선택 된 Unity의 AltspaceVR 인터페이스](images/custom-kits-img-04.png)

> [!NOTE]
> <span data-ttu-id="63fc7-133">생성 된 Prefab를 수정 하려면 계층으로 다시 끌고 변경한 다음 검사기 탭에서 **적용** 을 클릭 하 여 Prefab를 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-133">If you want to make any modifications to a generated Prefab, drag it back into the Hierarchy, make changes, and then click **Apply** in the Inspector tab to update the Prefab.</span></span> 

3. <span data-ttu-id="63fc7-134">준비가 되 면 업 로더 탭 아래로 스크롤하여 자산 번들로 zip 파일을 생성할 준비를 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-134">When you're ready, scroll down the Uploader tab and let's prepare to generate a zip file with the Asset Bundle</span></span>
4. <span data-ttu-id="63fc7-135">더 빠른 반복을 위해 **Android 용 빌드 키트** 를 선택 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-135">For faster iteration, uncheck the **Build Kit for Android?**.</span></span> <span data-ttu-id="63fc7-136">나중에, 반복이 완료 되거나 키트를 공유/기능 하려면 나중에 Android 용 버전을 빌드 및 업로드 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-136">Remember to build and upload a version for Android later when you're done iterating or want to share/feature your Kit.</span></span> 
5. <span data-ttu-id="63fc7-137">**Load Kit Prefab 디렉터리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-137">Select **Load Kit Prefab Directories**</span></span>
6. <span data-ttu-id="63fc7-138">키트 폴더 이름과 일치 하는 항목 옆에 있는 **빌드** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-138">Choose **Build** next to the one matching your Kit Folder Name.</span></span> <span data-ttu-id="63fc7-139">동일한 Unity 프로젝트에서 여러 키트를 생성 하는 것이 일반적입니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-139">It's common to produce multiple Kits from the same Unity project.</span></span> <span data-ttu-id="63fc7-140">이는 키트 크기에 따라 다소 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-140">This may take a while depending on the size of your Kit.</span></span> <span data-ttu-id="63fc7-141">완료 되 면 zip 파일을 포함 하는 폴더가 자동으로 열립니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-141">When it's done, the folder containing your zip file will open automatically.</span></span> 
7. <span data-ttu-id="63fc7-142">웹 사이트로 이동 하 여 이전에 만든 키트를 편집 하 고 생성 한 zip 파일을 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-142">Go to the website, edit the Kit you created earlier, and upload the zip file you produced.</span></span> <span data-ttu-id="63fc7-143">이 업로드는 파일 크기에 따라 다소 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-143">This upload may take a while depending on the file size.</span></span>
    * <span data-ttu-id="63fc7-144">성공 하는 경우 파일 크기를 "업로드" 하 고 PC 및 Android에 대해, 그리고 마지막으로 업데이트 한 시간에 왼쪽에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-144">If successful, you’ll see on the left side under “Uploads” the file sizes and for PC and Android and when they were last updated</span></span>
    * <span data-ttu-id="63fc7-145">실패 한 경우 스크립트가 없는지 확인 하 고 스크립트를 지원 하지 않습니다. 보안을 위해 해당 내용을 확인 하 고 다시 시도 하세요.</span><span class="sxs-lookup"><span data-stu-id="63fc7-145">If unsuccessful, make sure you don't have any scripts, we don't support scripts, we check for those for security and try again.</span></span>

<span data-ttu-id="63fc7-146">축하합니다!</span><span class="sxs-lookup"><span data-stu-id="63fc7-146">Congratulations!</span></span> <span data-ttu-id="63fc7-147">자신의 키트를 사용 하 여 빌드할 준비가 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-147">You're ready to build Worlds with your own Kit!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="63fc7-148">문제 해결</span><span class="sxs-lookup"><span data-stu-id="63fc7-148">Troubleshooting</span></span> 

<span data-ttu-id="63fc7-149">**제한이 있나요?**</span><span class="sxs-lookup"><span data-stu-id="63fc7-149">**Are there limits?**</span></span>
<span data-ttu-id="63fc7-150">아직 하드 제한이 없지만 사용자는 하나의 아티팩트를 사용 하는 경우에도 전체 키트의 플랫폼에 대 한 AssetBundle을 다운로드 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-150">There are no hard limits yet but remember that users need to download the AssetBundle for their platform for the entire Kit even if only one Artifact is used.</span></span> <span data-ttu-id="63fc7-151">플랫폼별 다운로드를 5mb 이하로 유지 하세요.</span><span class="sxs-lookup"><span data-stu-id="63fc7-151">Try to keep the download per-platform to 5 MB or less.</span></span> <span data-ttu-id="63fc7-152">이 작업을 수행 하는 한 가지 방법은 항목을 작은 키트로 분할 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-152">One way to do that is to split up things into smaller Kits.</span></span> <span data-ttu-id="63fc7-153">예를 들어 200 props은 반으로 분할 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-153">For example, 200 props should split in half.</span></span> 

<span data-ttu-id="63fc7-154">**"눈에 분할"이 표시 되나요?**</span><span class="sxs-lookup"><span data-stu-id="63fc7-154">**Seeing “split eye”?**</span></span>
<span data-ttu-id="63fc7-155">최신 업 로더를 다시 가져와 올바른 렌더링 설정 가져오기</span><span class="sxs-lookup"><span data-stu-id="63fc7-155">Reimport the latest Uploader to get the right rendering settings</span></span>

<span data-ttu-id="63fc7-156">**업데이트/변경 내용이 반영 되지 않나요?**</span><span class="sxs-lookup"><span data-stu-id="63fc7-156">**Updates/changes not reflected?**</span></span>
    * <span data-ttu-id="63fc7-157">키트 페이지에서 업데이트 된 시간 확인</span><span class="sxs-lookup"><span data-stu-id="63fc7-157">Check the updated time on the Kit page</span></span>
    * <span data-ttu-id="63fc7-158">세계를 다시 시작 해도 작동 하지 않습니다.--클라이언트를 다시 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-158">Reentering the World will not work-- restart client.</span></span> <span data-ttu-id="63fc7-159">하지만 업데이트 하는 데 몇 분 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-159">Even then it may take a few minutes to update</span></span>
    * <span data-ttu-id="63fc7-160">폴더 이름 또는 prefab 이름에 공백이 없는지 확인 합니다 **(예: ' party_favors ' 및 ' 파티 우위 '** ).</span><span class="sxs-lookup"><span data-stu-id="63fc7-160">Make sure there are no spaces in your folder names or prefab names **for example, 'party_favors' vs 'party favors'**</span></span>

<span data-ttu-id="63fc7-161">**스크립트가 있다고 생각 하지만** AssetBundle 브라우저에는 경우에 따라 파일이 자동으로 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-161">**It keeps saying I have a script but I don't** The AssetBundle Browser automatically includes files sometimes.</span></span> <span data-ttu-id="63fc7-162">가져오는 모델을 분리 해 보세요.</span><span class="sxs-lookup"><span data-stu-id="63fc7-162">Try to isolate the model you're bringing in.</span></span> <span data-ttu-id="63fc7-163">예를 들어, 다른 Prefab의 일부인 경우에는 끌어 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-163">For example, don't drag it in when it's part of another Prefab already</span></span>

<span data-ttu-id="63fc7-164">**파티클 시스템 및 애니메이션은 어떻습니까?**</span><span class="sxs-lookup"><span data-stu-id="63fc7-164">**What about Particle Systems and Animations?**</span></span>
<span data-ttu-id="63fc7-165">이러한 경우에는 메시를 렌더링 하 고 충돌을 비활성화 하 여 원본에 배치 된 1x1x1 큐브 아래에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-165">For these, next them under a 1x1x1 Cube positioned at the origin with Mesh Rendering and Collision disabled.</span></span> <span data-ttu-id="63fc7-166">파티클 시스템은 루프를 사용 하도록 설정 해야 하며, **크기 조정을** **계층** 으로 설정 하 여 altspace에서 적절히 크기를 조정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-166">Particle Systems should have looping enabled and **Scaling** should be set to **Hierarchy** so that we can scale them in Altspace properly.</span></span> <span data-ttu-id="63fc7-167">모든 애니메이션에 대 한 prefabs를 생성 한 후에는 각 애니메이션에 대 한 **충돌** 개체에서 충돌을 비활성화 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-167">After you generate the prefabs for all the animations, disable the collisions on the **collision** objects for each.</span></span>

<span data-ttu-id="63fc7-168">**아티팩트가 어두움** 모델의 재질 셰이더를 **모바일/꼭 짓 점 전용 방향 광원** 으로 설정 했습니까?</span><span class="sxs-lookup"><span data-stu-id="63fc7-168">**The Artifacts are dark** Did you set the model's material shader to **Mobile/Vertex lit-only directional lights**?</span></span>

<span data-ttu-id="63fc7-169">**아티팩트가 올바른 방법이 아닙니다** . **모델** 및 **collider** 를 회전 하 고 Prefab를 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-169">**The Artifact isn't facing the right way** Rotate the **model** and **collider** and update the Prefab.</span></span> <span data-ttu-id="63fc7-170">부모를 회전 해도 아무것도 수행 되지 않습니다. 무시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-170">Rotating the parent won't do anything--that's ignored.</span></span> <span data-ttu-id="63fc7-171">**회전 재정의** 필드를 사용 하 여이 작업을 쉽게 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="63fc7-171">You can use the **Rotation Override** field to do this easily.</span></span>

<span data-ttu-id="63fc7-172">**이러한 아티팩트를 SDK의 **Createfromlibrary** 함수와 함께 사용할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="63fc7-172">**Can these Artifacts be used with the SDK's **CreateFromLibrary** function?**</span></span>
<span data-ttu-id="63fc7-173">예</span><span class="sxs-lookup"><span data-stu-id="63fc7-173">Yes</span></span>