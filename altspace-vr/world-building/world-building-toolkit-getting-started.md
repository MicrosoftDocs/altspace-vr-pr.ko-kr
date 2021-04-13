---
title: 세계 개발 도구 키트 소개
description: 전 세계의 도구 키트와 함께 Unity 장면 템플릿을 사용 하 여 AltspaceVR 환경을 설정 하 고 업로드 하는 방법에 대해 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 도구 키트
ms.openlocfilehash: cf4660f46d93ca5c5f23de3f567ff04b12519617
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212627"
---
# <a name="introducing-the-world-building-toolkit"></a><span data-ttu-id="d796c-104">세계 개발 도구 키트 소개</span><span class="sxs-lookup"><span data-stu-id="d796c-104">Introducing the World Building Toolkit</span></span>

> [!NOTE]
> <span data-ttu-id="d796c-105">세계 개발 도구 키트는 microsoft에서 제공 하는 [Anthony Madden](https://twitter.com/chigamesstudio)에 의해 실행 되는 커뮤니티 프로젝트입니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-105">The World Building Toolkit is a community project run by our awesome friend, [Anthony Madden](https://twitter.com/chigamesstudio), with support from us.</span></span> <span data-ttu-id="d796c-106">관심이 있는 경우 [공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 에 참여 하 고 #world-빌딩 채널을 방문 하세요.</span><span class="sxs-lookup"><span data-stu-id="d796c-106">If you're interested, please join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel.</span></span> <span data-ttu-id="d796c-107">현재 Mac 평가판 베타를 제공 하 고 있습니다. [자세한 정보](https://altvr.com/altspacevr-mac)</span><span class="sxs-lookup"><span data-stu-id="d796c-107">We currently have a Mac Trial Beta right now, [more details](https://altvr.com/altspacevr-mac)</span></span>

<span data-ttu-id="d796c-108">업 로더를 사용 하 여 전 세계의 템플릿으로 Unity 장면을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-108">The Uploader allows you to use a Unity scene as a Template for your Worlds.</span></span> <span data-ttu-id="d796c-109">Minecraft에서 파티를 즐겨 사용 하거나 즐겨 사용 하는 haunted를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-109">You can bring in a haunted house for Halloween or your favorite creation from Minecraft.</span></span> <span data-ttu-id="d796c-110">Unity로 가져올 수 있는 경우 이러한 방식으로 Altspace으로 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-110">If you can import it into Unity, you can probably get it into Altspace this way.</span></span> <span data-ttu-id="d796c-111">다음은 몇 가지 [예](https://account.altvr.com/worlds/1046572460192825569)입니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-111">Here are a few [example Worlds](https://account.altvr.com/worlds/1046572460192825569).</span></span>

![예제 세계](images/unity-uploader-img-01.png)

## <a name="setup"></a><span data-ttu-id="d796c-113">설치 프로그램</span><span class="sxs-lookup"><span data-stu-id="d796c-113">Setup</span></span>

1. <span data-ttu-id="d796c-114">[공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 에 참여 하 고 #world을 방문 하세요. 친구는 친구 들이 혼자 빌드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-114">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel - Friends don't let friends build Worlds alone.</span></span>
2. <span data-ttu-id="d796c-115">기본 사항에 대 한 [시작 하기 가이드](world-building-getting-started.md) 를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="d796c-115">Read our [World-Building Getting Started Guide](world-building-getting-started.md) for the basics</span></span>
3. <span data-ttu-id="d796c-116">[Unity 허브를 설치](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) 하 고 **unity 2019.4.2 f1** 을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-116">[Install Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) and install **Unity 2019.4.2f1**.</span></span> <span data-ttu-id="d796c-117">이 버전을 정확 하 게 일치 하지 않으면 업 로더가 작동 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-117">The Uploader won't work unless you match this version exactly.</span></span> <span data-ttu-id="d796c-118">무료 Unity 계정이 없으면 무료 Unity 계정이 필요 하 고, 재미를 위해이 작업을 수행 하므로 **개인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-118">You'll need a free Unity account if you don't have one and choose **Personal** since you're doing this for fun!</span></span> <span data-ttu-id="d796c-119">설치 하는 동안 **Android 빌드** 옵션을 선택 하 고 자동 업데이트를 사용 하지 않도록 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-119">During the install, make sure you check the **Android Builds** option and disable auto-update.</span></span>
4. [<span data-ttu-id="d796c-120">최신 Unity 업 로더 다운로드</span><span class="sxs-lookup"><span data-stu-id="d796c-120">Download the latest Unity Uploader</span></span>](https://aka.ms/AsvrCommunityUploader)
5. <span data-ttu-id="d796c-121">웹 사이트에서 [템플릿을 만듭니다](https://account.altvr.com/space_templates/new) .</span><span class="sxs-lookup"><span data-stu-id="d796c-121">[Create a Template](https://account.altvr.com/space_templates/new) on our website.</span></span> <span data-ttu-id="d796c-122">**템플릿을 헬로 월드** 으로 이름을로 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-122">Name it **Hello World Template**.</span></span>
6. <span data-ttu-id="d796c-123">[세계를 만들고](https://account.altvr.com/worlds/my) **헬로 월드** 이름을로 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-123">[Create a World](https://account.altvr.com/worlds/my) and name it **Hello World**.</span></span> <span data-ttu-id="d796c-124">템플릿으로 **헬로 월드 템플릿을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-124">Select **Hello World Template** as the Template.</span></span>

![만든 세계 화면](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a><span data-ttu-id="d796c-126">장면 업로드</span><span class="sxs-lookup"><span data-stu-id="d796c-126">Upload your scene</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. <span data-ttu-id="d796c-127">Unity 허브를 열고 새 Unity 2019.4.2 f1 프로젝트를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-127">Open Unity Hub and create a new Unity 2019.4.2f1 project.</span></span>
2. <span data-ttu-id="d796c-128">프로젝트를 연 상태에서 다운로드 한 파일을 두 번 클릭 하 여 업 로더를 가져옵니다 (Unity 패키지).</span><span class="sxs-lookup"><span data-stu-id="d796c-128">With your project open, import the Uploader by double-clicking the file you downloaded (it's a Unity package).</span></span> <span data-ttu-id="d796c-129">이제 **AltspaceVR** 라는 새 탭이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-129">You should now see a new tab called **AltspaceVR**.</span></span> <span data-ttu-id="d796c-130">Altspace와 함께 사용 하려는 모든 Unity 프로젝트에 대 한 패키지를 가져와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-130">You'll need to import the package for every Unity project you want to use with Altspace</span></span>
3. <span data-ttu-id="d796c-131">**메뉴 > AltspaceVR > 빌드 설정** 열기</span><span class="sxs-lookup"><span data-stu-id="d796c-131">Open **Menu > AltspaceVR > Build Settings**</span></span>
4. <span data-ttu-id="d796c-132">Altspace 계정 자격 증명으로 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-132">Sign in with your Altspace account credentials</span></span>
5. <span data-ttu-id="d796c-133">**템플릿 로드** 를 선택한 다음 **헬로 월드 템플릿** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-133">Select **Load Templates** and then select **Hello World Template**</span></span>
6. <span data-ttu-id="d796c-134">장면에 큐브를 추가 하 고 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-134">Add a cube to your scene and save.</span></span>
7. <span data-ttu-id="d796c-135">**Windows 용 빌드** 를 선택 하 고 **Android 용 빌드** 를 선택 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-135">Check **Build for Windows?** and uncheck **Build for Android?**</span></span>
8. <span data-ttu-id="d796c-136">**업로드** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-136">Select **Upload**.</span></span> <span data-ttu-id="d796c-137">약 1 분 후 **업로드가** 완료 된 것을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-137">In about a minute, you should see **Upload** complete.</span></span>
9. <span data-ttu-id="d796c-138">Altspace를 시작 하 고 **내 세계 > 메뉴 >** 를 입력 하 여 **헬로 월드** 를 조인 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-138">Join **Hello World** by launching Altspace and entering from **Menu > Worlds > My Worlds**</span></span>
10. <span data-ttu-id="d796c-139">**메뉴 > 설정 > 중간 > 공간 다시** 설정에서 전 세계를 다시 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-139">Reset the World from **Menu > Settings > Moderate > Reset Space**</span></span>
11. <span data-ttu-id="d796c-140">큐브가 표시 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-140">You should see the cube.</span></span> <span data-ttu-id="d796c-141">위의 비디오에서 빨리이 작업을 수행 하는 경우 10 초 내에 변경 내용을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-141">If you do it fast like in the video above, you can see changes within as little as 10 seconds.</span></span>

## <a name="whats-supported"></a><span data-ttu-id="d796c-142">지원되는 내용</span><span class="sxs-lookup"><span data-stu-id="d796c-142">What's supported</span></span>

* <span data-ttu-id="d796c-143">예: 모델, 충돌, 애니메이션, 파티클 효과, 오디오, skyboxes 등</span><span class="sxs-lookup"><span data-stu-id="d796c-143">Yes: models, collision, animations, particle effects, audio, skyboxes, and so on</span></span>
* <span data-ttu-id="d796c-144">아니요: 스크립트</span><span class="sxs-lookup"><span data-stu-id="d796c-144">No: scripts.</span></span> <span data-ttu-id="d796c-145">보안을 위해 스크립트가 포함 된 업로드가 거부 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-145">For security purposes, uploads containing scripts will be rejected</span></span>
* <span data-ttu-id="d796c-146">예: 동적 전 세계 조명 등의 화려한 사물</span><span class="sxs-lookup"><span data-stu-id="d796c-146">Maybe: fancy stuff like dynamic global illumination</span></span>
* <span data-ttu-id="d796c-147">다른 플랫폼에 대 한 장면을 개별적으로 또는 함께 업로드</span><span class="sxs-lookup"><span data-stu-id="d796c-147">Upload scenes for different platforms separately or together</span></span>
* <span data-ttu-id="d796c-148">업 [로더를 사용](https://account.altvr.com/worlds/featured)하 여 많은 기능을 빌드 했습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-148">See [Featured Worlds](https://account.altvr.com/worlds/featured), many were built using the Uploader</span></span>

## <a name="tips"></a><span data-ttu-id="d796c-149">팁</span><span class="sxs-lookup"><span data-stu-id="d796c-149">Tips</span></span>

* <span data-ttu-id="d796c-150">[공식 AltspaceVR Discord](https://discordapp.com/invite/altspacevr)에 참여 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-150">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr).</span></span>
* <span data-ttu-id="d796c-151">왼쪽의 템플릿 페이지에서 플랫폼별 최신 업로드를 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-151">On the Template page on the left side, we show you the latest uploads by platform.</span></span> <span data-ttu-id="d796c-152">성공적으로 완료 되 면 **1-2 분 전에** 표시 됩니다. Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span><span class="sxs-lookup"><span data-stu-id="d796c-152">If it was successful, you'd see **1-2 mins ago**.Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span></span>

![업로드가 강조 표시 된 템플릿 패널 열기](images/unity-uploader-img-03.png)

* <span data-ttu-id="d796c-154">업데이트 시에는 전 세계에 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-154">You can be in-World when you update.</span></span> <span data-ttu-id="d796c-155">업 로더가 **업로드가 완료** 되 면 변경 내용을 볼 수 있도록 전 세계를 다시 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-155">The moment the Uploader says **Upload Complete** you can reset the World to see the changes.</span></span>
* <span data-ttu-id="d796c-156">간단한 장면을 사용 하 여 PC 전용으로 빌드하면 Altspace가 변경 되는 데 1 분 미만이 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-156">Building for PC-only with a simple scene should take less than 1 minute to see a change in Altspace</span></span>
* <span data-ttu-id="d796c-157">혼란을 피하기 위해 전 세계를 개인 또는 목록으로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-157">Set your World to be Private and Unlisted to avoid distractions.</span></span>
* <span data-ttu-id="d796c-158">사용자가 기본적으로 생성 하는 위치를 확인할 수 있도록 원본에 큐브를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-158">Place a cube at the origin so you can see where people will spawn by default.</span></span> <span data-ttu-id="d796c-159">업로드할 때 큐브를 숨깁니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-159">Hide the cube when uploading.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d796c-160">문제 해결</span><span class="sxs-lookup"><span data-stu-id="d796c-160">Troubleshooting</span></span>

<span data-ttu-id="d796c-161">**거의 모든 항목으로 텔레포트 할 수 없습니다** . 이로 텔레포트 하려면 개체에 충돌을 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-161">**I'm falling or can't teleport onto anything** You need to add collision to objects to teleport onto them.</span></span>

<span data-ttu-id="d796c-162">**변경 내용 없음**</span><span class="sxs-lookup"><span data-stu-id="d796c-162">**Nothing changed**</span></span>
    * <span data-ttu-id="d796c-163">장면을 Unity에 저장 했습니까?</span><span class="sxs-lookup"><span data-stu-id="d796c-163">Did you save the scene in Unity?</span></span>
    * <span data-ttu-id="d796c-164">테스트 중인 플랫폼을 선택 하셨습니까?</span><span class="sxs-lookup"><span data-stu-id="d796c-164">Did you choose the platform you're testing on?</span></span>
    * <span data-ttu-id="d796c-165">올바른 세계에 있나요?</span><span class="sxs-lookup"><span data-stu-id="d796c-165">Are you in the right World?</span></span> <span data-ttu-id="d796c-166">업 로더 및 세계 양식에서 적합 한 템플릿을 선택 했습니까?</span><span class="sxs-lookup"><span data-stu-id="d796c-166">Did you choose the right Template in the Uploader AND in the World form?</span></span>
    * <span data-ttu-id="d796c-167">템플릿 페이지 통계를 확인 했나요?</span><span class="sxs-lookup"><span data-stu-id="d796c-167">Did you check the Template page stats?</span></span>

<span data-ttu-id="d796c-168">**업로드 실패 또는 시간 초과**</span><span class="sxs-lookup"><span data-stu-id="d796c-168">**Upload fails or times out**</span></span>
    * <span data-ttu-id="d796c-169">가장 일반적인 업로드 오류에 잘못 된 Unity 버전이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-169">Most common upload error is having the wrong Unity version.</span></span> <span data-ttu-id="d796c-170">필요한 버전과 정확 하 게 일치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-170">It must match the required version exactly.</span></span>
    * <span data-ttu-id="d796c-171">업로드가 너무 클 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-171">Your upload might be too large.</span></span> <span data-ttu-id="d796c-172">PC 장면을 100 < 유지 하세요.</span><span class="sxs-lookup"><span data-stu-id="d796c-172">Try to keep PC scenes < 100 MB.</span></span> <span data-ttu-id="d796c-173">Small 및 build를 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-173">Start small and build up.</span></span> <span data-ttu-id="d796c-174">최적화, 최적화, 최적화.</span><span class="sxs-lookup"><span data-stu-id="d796c-174">Optimize, optimize, optimize.</span></span>
    * <span data-ttu-id="d796c-175">간단한 큐브로 새 프로젝트를 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="d796c-175">Try with a fresh project with a simple cube.</span></span>
    * <span data-ttu-id="d796c-176">빌드 중에 강제 종료 하지 마세요. 장면을 손상 시킬 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-176">Don't force quit during a build--it can corrupt your scene.</span></span> <span data-ttu-id="d796c-177">다시 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-177">Try reuploading.</span></span>

<span data-ttu-id="d796c-178">**속도가 느립니다.**</span><span class="sxs-lookup"><span data-stu-id="d796c-178">**It's a slow process**</span></span>
    * <span data-ttu-id="d796c-179">나중에 Android를 반복 하는 동안에만 PC 용을 빌드하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-179">We recommend building for PC only while iterating and for Android later.</span></span>
    * <span data-ttu-id="d796c-180">사용 하지 않는 파일을 제거해 보세요.</span><span class="sxs-lookup"><span data-stu-id="d796c-180">Try removing unused files.</span></span> <span data-ttu-id="d796c-181">어떤 이유로 Unity가 overzealous를 가져오는 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-181">For whatever reason Unity gets overzealous sometimes.</span></span>

<span data-ttu-id="d796c-182">**내 Altspace 자격 증명을 사용 하 여 로그인 할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="d796c-182">**I can't sign in with my Altspace credentials**</span></span>
    * <span data-ttu-id="d796c-183">전자 메일은 대/소문자를 구분 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-183">Emails are case-sensitive.</span></span>
    * <span data-ttu-id="d796c-184">새 프로젝트를 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="d796c-184">Try with a new project.</span></span>
    * <span data-ttu-id="d796c-185">Altspace 계정이 정상 상태 인지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="d796c-185">Make sure your Altspace account is in good standing.</span></span>

## <a name="see-also"></a><span data-ttu-id="d796c-186">참조</span><span class="sxs-lookup"><span data-stu-id="d796c-186">See also</span></span>

* [<span data-ttu-id="d796c-187">Unity 학습</span><span class="sxs-lookup"><span data-stu-id="d796c-187">Unity Learn</span></span>](https://unity3d.com/learn)
* [<span data-ttu-id="d796c-188">Unity 포럼</span><span class="sxs-lookup"><span data-stu-id="d796c-188">Unity Forums</span></span>](https://forum.unity.com)
