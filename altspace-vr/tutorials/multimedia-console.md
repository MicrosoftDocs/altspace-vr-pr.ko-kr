---
title: 멀티미디어 콘솔 사용
description: AltspaceVR 환경의 멀티미디어 콘솔 구성, 게시 및 제어를 시작하는 방법을 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 콘솔, 멀티미디어
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923010"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="ad400-104">멀티미디어 콘솔 사용</span><span class="sxs-lookup"><span data-stu-id="ad400-104">Using the multimedia console</span></span>

<span data-ttu-id="ad400-105">멀티미디어 콘솔은 이벤트 및 세계에서 미디어 공유를 가능하게 하는 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="ad400-106">이를 사용하여 이미지, 프레젠테이션 슬라이드, 라이브 스트림, 비디오, 재생 목록 등과 같은 것을 공유할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="ad400-107">다음은 멀티미디어 콘솔 **v0.5.0+** 를 사용하는 방법에 대한 단계별 지침입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="ad400-108">시작</span><span class="sxs-lookup"><span data-stu-id="ad400-108">Getting started</span></span>

<span data-ttu-id="ad400-109">멀티미디어 콘솔 시작은 두 부분으로 구성된 프로세스입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="ad400-110">먼저 사용자 환경에 배치하는 멀티미디어 콘솔 세션에 대한 구성을 생성하고 게시하는 데 사용할 웹 포털이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="ad400-111">두 번째는 사용자 환경에 실제 멀티미디어 콘솔 앱을 배치하고 사용해야 하는 구성 코드를 설정하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="ad400-112">웹 포털을 통해 멀티미디어 콘솔 구성</span><span class="sxs-lookup"><span data-stu-id="ad400-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="ad400-113">먼저 URL이 필요하기 때문에 콘텐츠가 온라인으로 호스트되는지 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="ad400-114">(사진을 altvr.com 업로드하거나, 비디오 .mp4 파일을 온라인으로 호스트하거나, Dlive 라이브 스트림 링크를 사용할 수 있습니다. https://dlive.tv/yourlivestream)</span><span class="sxs-lookup"><span data-stu-id="ad400-114">(You can upload photos to altvr.com, host a video .mp4 file online or use a Dlive live stream link: https://dlive.tv/yourlivestream)</span></span> 
2. <span data-ttu-id="ad400-115">에서 멀티미디어 콘솔에 대한 웹 포털로 이동합니다. [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="ad400-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="ad400-116">웹 포털에서 멀티미디어 콘솔에 대한 구성을 생성하고 게시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="ad400-117">(다양한 속성에 대한 자세한 내용은 아래를 참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="ad400-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="ad400-118">미디어 목록에 미디어를 입력하고 일반 설정을 구성했으면 앱의 오른쪽 위에 있는 게시 단추를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="ad400-119">게시가 완료되면 배치한 멀티미디어 콘솔에 입력할 수 있는 두 개의 단어 코드가 있는 대화 상자가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="ad400-120">사용자 환경에 멀티미디어 콘솔 배치</span><span class="sxs-lookup"><span data-stu-id="ad400-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="ad400-121">World **Editor > Editor Panel > SDK Apps > 멀티미디어 콘솔** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="ad400-122">(등록되지 않은 **앱에 대한 세계 편집기 > 기본 > SDK 앱으로** 이동하지 마세요.)</span><span class="sxs-lookup"><span data-stu-id="ad400-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="ad400-123">멀티미디어 콘솔을 배치하여 공간과 대상을 가장 잘 배치합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="ad400-124">주황색 편집 모드 단추를 클릭하여 편집 모드에서 나가세요.</span><span class="sxs-lookup"><span data-stu-id="ad400-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="ad400-125">**미디어 플레이어 소유자인가요?** 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="ad400-126">이 멀티미디어 콘솔 세션의 공식 소유자여야 하는 사용자인 경우 확인하고 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="ad400-127">(다른 권한 있는 역할도 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="ad400-128">자세한 목록은 아래를 참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="ad400-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="ad400-129">예를 선택하여 기본 호스트임을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="ad400-130">웹 포털 또는 유효한 JSON에서 코드를 입력하라는 대화 상자가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="ad400-131">대시를 포함하여 웹 포털에서 두 개의 단어 코드를 입력하고 확인을 누릅니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="ad400-132">(JSON은 아래에 설명된 고급 구성입니다.)</span><span class="sxs-lookup"><span data-stu-id="ad400-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="ad400-133">멀티미디어 콘솔은 웹 포털에서 빌드한 구성으로 몇 초 후에 로드됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="ad400-134">멀티미디어 콘솔 제어</span><span class="sxs-lookup"><span data-stu-id="ad400-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="ad400-135">코드를 입력하고 구성 프로세스를 완료하면 미디어 디스플레이 아래에 컨트롤 단추가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="ad400-136">**재생은** 미디어 뷰어를 시작합니다(또는 이전에 중지된 경우 현재 항목에서 다시 시작).</span><span class="sxs-lookup"><span data-stu-id="ad400-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="ad400-137">**중지는** 미디어 뷰어를 중지하고 현재 미디어를 숨깁니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="ad400-138">**Next/Prev는** 다음 또는 이전 미디어로 건너뜁니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="ad400-139">**x/x**   는 미디어 목록에 현재 인덱스를 표시하고 목록의 임의의 지점으로 이동할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="ad400-140">**구성을** 사용하면 웹 포털에서 새 코드를 다시 활성화하여 콘솔에서 새 구성을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="ad400-141">이제 멀티미디어 콘솔을 통해 공유를 시작하도록 설정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="ad400-142">웹 포털 작업</span><span class="sxs-lookup"><span data-stu-id="ad400-142">Working with the web portal</span></span>

<span data-ttu-id="ad400-143">웹 포털은 멀티미디어 콘솔의 다양한 기능을 구성할 수 있는 웹앱입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="ad400-144">이러한 기능은 두 가지 범주로 구분됩니다. 일반 미디어 콘솔 설정 및 미디어 재생 목록</span><span class="sxs-lookup"><span data-stu-id="ad400-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="ad400-145">멀티미디어 콘솔 일반 설정</span><span class="sxs-lookup"><span data-stu-id="ad400-145">Multimedia console general settings</span></span>

<span data-ttu-id="ad400-146">**Playback 설정**</span><span class="sxs-lookup"><span data-stu-id="ad400-146">**Playback Settings**</span></span>

<span data-ttu-id="ad400-147">미디어 목록에 대한 일반 재생 설정</span><span class="sxs-lookup"><span data-stu-id="ad400-147">General playback settings for the media list</span></span>

* <span data-ttu-id="ad400-148">**루프 미디어 목록**- 목록 끝에 도달하면 미디어 목록이 반복되는지 여부를 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="ad400-149">**Start 메서드** - 멀티미디어 콘솔을 시작할 메서드를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="ad400-150">수동 - 미디어를 시작하기 전에 재생 단추를 누를 때까지 대기합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="ad400-151">시작부터 자동 시작 - 목록의 시작 부분에서 미디어 목록 자동 시작</span><span class="sxs-lookup"><span data-stu-id="ad400-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="ad400-152">자동 시작 임의 - 목록의 임의 시작 지점에서 미디어를 자동으로 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="ad400-153">**역할**</span><span class="sxs-lookup"><span data-stu-id="ad400-153">**Roles**</span></span>

<span data-ttu-id="ad400-154">멀티미디어 콘솔을 제어하고 구성하기 위한 역할 할당</span><span class="sxs-lookup"><span data-stu-id="ad400-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="ad400-155">이러한 역할은 다음 집합으로 세분화됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="ad400-156">**소유자만** - 멀티미디어 콘솔 세션의 소유자인 사용자</span><span class="sxs-lookup"><span data-stu-id="ad400-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="ad400-157">**관리자 권한 사용자** - 멀티미디어 콘솔이 원래 구성된 공간에 중재자 또는 호스트 역할이 있는 사용자</span><span class="sxs-lookup"><span data-stu-id="ad400-157">**Elevated Users** - Users that have moderator or host roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="ad400-158">**모든 사용자** - 모든 사용자</span><span class="sxs-lookup"><span data-stu-id="ad400-158">**All Users** - All users</span></span>

<span data-ttu-id="ad400-159">이러한 역할은 이 목록에서 선택한 역할 위에 있는 모든 역할에도 해당 기능을 사용할 수 있는 권한이 부여된다는 점에서 스택됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="ad400-160">예: **관리자 권한 사용자는** AltspaceVR의 중재자 또는 호스트\*\*가 아니더라도 **소유자를** 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator or host\*\* in AltspaceVR.</span></span> <span data-ttu-id="ad400-161">역할 할당에 의해 제어되는 기능은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="ad400-162">**미디어 플레이어를 제어할** 수 있습니다. - 멀티미디어 콘솔의 미디어 재생 단추를 제어할 수 있는 역할을 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="ad400-163">**미디어 플레이어를 구성할** 수 있습니다. - **구성** 단추에 대한 액세스 권한을 부여받아 멀티미디어 콘솔을 구성할 수 있는 역할을 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="ad400-164">미디어 목록에 사진 및 비디오 추가</span><span class="sxs-lookup"><span data-stu-id="ad400-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="ad400-165">미디어는 멀티미디어 콘솔의 핵심입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="ad400-166">이미지 및 비디오 링크는 멀티미디어 콘솔 내에서 미디어 유형으로 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="ad400-167">새 미디어를 추가하려면 **이미지 추가** 또는 **비디오 추가** 아이콘을 선택하여 미디어 정보 및 설정을 입력하는 대화 상자 팝업을 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="ad400-168">다음은 미디어 유형 및 관련 설정에 대한 분석입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="ad400-169">**Image**</span><span class="sxs-lookup"><span data-stu-id="ad400-169">**Image**</span></span>

<span data-ttu-id="ad400-170">이미지는 jpeg, png 및 son on과 같은 표준 이미지 형식이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="ad400-171">공용 링크가 있는 어딘가에 호스트되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="ad400-172">**이름** - (필수) 이미지를 식별할 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="ad400-173">**이미지 URL** - (필수) 이미지의 공용 URL</span><span class="sxs-lookup"><span data-stu-id="ad400-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="ad400-174">**건너뛰기 후** - 이미지를 건너뛰어야 하는 시간(초)</span><span class="sxs-lookup"><span data-stu-id="ad400-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="ad400-175">**비디오**</span><span class="sxs-lookup"><span data-stu-id="ad400-175">**Video**</span></span>

<span data-ttu-id="ad400-176">비디오는 Twitch 및 DLive를 통해 호스팅되는 비디오 또는 라이브 스트림일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="ad400-177">(다른 지원은 적절한 스트림 URL을 얻기 위해 추가 작업과 함께 작동할 수 있지만 멀티미디어 콘솔 내에서 완전히 지원되지는 않습니다.)</span><span class="sxs-lookup"><span data-stu-id="ad400-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="ad400-178">**이름** - (필수) 비디오를 식별할 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="ad400-179">**비디오 URL** - (필수) 비디오가 호스트되거나 라이브 스트림이 제공되는 공용 URL입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="ad400-180">**건너뛰기 후** - 비디오를 건너뛰어야 하는 시간(초)</span><span class="sxs-lookup"><span data-stu-id="ad400-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>

> [!NOTE]
> <span data-ttu-id="ad400-181">필수: 비디오를 제대로 전달할 수 있도록 비디오 길이와 일치하는 시간을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-181">REQUIRED: Put in the time that matches the length of the video to enable videos to properly forward.</span></span> <span data-ttu-id="ad400-182">예를 들어 비디오가 5분 길이인 경우 300초가 소요됩니다. 그렇지 않으면 비디오가 다음 콘텐츠로 건너뛰지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-182">For example, if your video is 5 minutes long put 300 seconds, otherwise your video won't skip to the next piece of content.</span></span>

* <span data-ttu-id="ad400-183">**볼륨** - 0(분) - 1(최대) 값의 비디오 볼륨입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-183">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="ad400-184">**시작 시간** - 비디오 시작부터 시작하는 시간(초)입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-184">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="ad400-185">**시작 거리 롤오프** - 멀티미디어 콘솔에서 이동할 때 볼륨이 떨어지기 시작하는 세계 미터의 거리입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-185">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="ad400-186">**비디오 작업 종료** - 비디오 끝에 도달하면 취할 작업입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-186">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="ad400-187">중지 - 비디오가 종료된 후 미디어 목록이 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-187">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="ad400-188">루프 - 수동으로 건너뛸 때까지 비디오가 반복됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-188">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="ad400-189">다음 재생 - 현재 비디오가 종료된 후 미디어 목록의 다음 미디어가 시작됩니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-189">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="ad400-190">JSON 직접 작업(고급/선택 사항)</span><span class="sxs-lookup"><span data-stu-id="ad400-190">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="ad400-191">멀티미디어 콘솔은 AltspaceVR에서 콘솔의 프롬프트에 직접 JSON 입력을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-191">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="ad400-192">JSON은 미디어 플레이어 구성을 사용하도록 설정하는 내부 메커니즘입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-192">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="ad400-193">JSON을 직접 설정하는 기능을 노출하면 고급 사용자가 자신의 요구 사항과 JSON에 익숙한 워크플로를 직접 빌드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-193">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="ad400-194">다음은 JSON 구조 및 JSON의 유효성을 검사하는 스키마에 대한 간략한 설명입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-194">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="ad400-195">아래 속성에 대한 자세한 설명은 멀티미디어 콘솔 구성에 대해 설명하는 위의 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ad400-195">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="ad400-196">이 섹션은 주로 JSON 데이터의 스키마 예제 및 구조화에 중점을 두고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-196">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="ad400-197">글로벌 미디어 설정</span><span class="sxs-lookup"><span data-stu-id="ad400-197">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="ad400-198">미디어 목록</span><span class="sxs-lookup"><span data-stu-id="ad400-198">Media list</span></span>

<span data-ttu-id="ad400-199">미디어 목록은 역할 및 재생 설정과 같은 JSON 구조의 루트에 설정된 속성입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-199">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="ad400-200">다음 미디어 구성 구조 중 하나를 포함할 수 있는 간단한 배열입니다.</span><span class="sxs-lookup"><span data-stu-id="ad400-200">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="ad400-201">(각 가 수행하는 일에 대한 자세한 내용은 위의 속성 설명을 참조하세요.)</span><span class="sxs-lookup"><span data-stu-id="ad400-201">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="ad400-202">**이미지 예제**</span><span class="sxs-lookup"><span data-stu-id="ad400-202">**Image example**</span></span>

<span data-ttu-id="ad400-203">*필수 필드: "name" 및 "imageUrl"*</span><span class="sxs-lookup"><span data-stu-id="ad400-203">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="ad400-204">**비디오 예제**</span><span class="sxs-lookup"><span data-stu-id="ad400-204">**Video example**</span></span>

<span data-ttu-id="ad400-205">*필수 필드: "name" 및 "videoUrl"*</span><span class="sxs-lookup"><span data-stu-id="ad400-205">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="ad400-206">예제 JSON</span><span class="sxs-lookup"><span data-stu-id="ad400-206">Example JSON</span></span>

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a><span data-ttu-id="ad400-207">스키마</span><span class="sxs-lookup"><span data-stu-id="ad400-207">Schema</span></span>

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> <span data-ttu-id="ad400-208">멀티미디어 콘솔 v0.5.0을 사용하여 최신</span><span class="sxs-lookup"><span data-stu-id="ad400-208">Up to date with Multimedia Console v0.5.0</span></span>