---
title: 최신 Unity 버전으로 콘텐츠 업데이트
description: 최신 버전의 Unity로 콘텐츠를 업데이트 하는 방법에 대해 알아봅니다.
ms.date: 06/4/2021
ms.topic: article
keywords: 키트, 세계, unity, 업데이트, 셰이더, 업 로더, 문제 해결
ms.openlocfilehash: f8a805c4b3350f2c97c43d3d48c35733ec7e9710
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/25/2021
ms.locfileid: "112961255"
---
# <a name="updating-content-to-the-latest-unity-version"></a><span data-ttu-id="5b3c0-104">최신 Unity 버전으로 콘텐츠 업데이트</span><span class="sxs-lookup"><span data-stu-id="5b3c0-104">Updating Content to the Latest Unity Version</span></span>

## <a name="moving-to-unity-202039"></a><span data-ttu-id="5b3c0-105">Unity 2020.3.9로 이동</span><span class="sxs-lookup"><span data-stu-id="5b3c0-105">Moving to Unity 2020.3.9</span></span>

<span data-ttu-id="5b3c0-106">오늘부터 AltspaceVR이 최신 버전의 Unity (2020.3.9)로 업그레이드 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-106">Starting today, AltspaceVR has upgraded to a recent version of Unity (2020.3.9).</span></span> <span data-ttu-id="5b3c0-107">이 업데이트는 몇 가지 성능 향상 외에도 향후 제공 될 것으로 기대 하는 향후 기능을 증명 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-107">In addition to some performance improvements, this update future-proofs us for forthcoming features that we're excited to incorporate.</span></span> <span data-ttu-id="5b3c0-108">이 변경은 모든 기존 콘텐츠와 호환 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-108">This change should be compatible with all existing content.</span></span> <span data-ttu-id="5b3c0-109">그렇지 않은 경우 지원 담당자에 게 문의 하세요. altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="5b3c0-109">If it isn't, feel free to contact support: altvr.com/support</span></span>

<span data-ttu-id="5b3c0-110">2020.3.9로의 사용자 생성 콘텐츠는 영향을 받지 않지만, 몇 주 후에 [사용자가 콘텐츠를 업데이트 해야 하는 AltspaceVR의 스테레오 렌더링 모드]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)를 변경 하 게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-110">Though this move to 2020.3.9 hasn't affected user-generated content, in a few weeks we're making a change to AltspaceVR's [stereo rendering mode that will require users to update their content]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html).</span></span> <span data-ttu-id="5b3c0-111">[단일 Pass](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 로 업그레이드 하는 경우 사용자는 상당한 성능 향상이 가능 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-111">This upgrade to [Single Pass Instancing](https://docs.unity3d.com/Manual/SinglePassInstancing.html) will allow for significant performance improvements in your worlds.</span></span> <span data-ttu-id="5b3c0-112">이 새 빌드는 2019.4 이전 콘텐츠와의 이전 버전과의 호환성을 더 이상 지원 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-112">Keep in mind that this new build will no longer support backwards-compatibility with content from 2019.4 and older.</span></span> <span data-ttu-id="5b3c0-113">모든 작성자 소유 콘텐츠가 가능한 한 빨리 업데이트 되어 주요 변경 사항이 발생 하지 않도록 하는 것이 긴급 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-113">It's urgent that all creator-owned content is updated as soon as possible to avoid breaking changes.</span></span> <span data-ttu-id="5b3c0-114">아래 가이드에 따라 콘텐츠를 업데이트 하 고 Unity 2020.3.9의 단일 패스 인스턴스에 원활한 전환을 확인 하세요.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-114">Follow the guide below to update your content and ensure a smooth transition to Single Pass Instancing on Unity 2020.3.9.</span></span>

> [!NOTE]
> <span data-ttu-id="5b3c0-115">다른 사용자가 소유 하 고 있는 콘텐츠를 정기적으로 사용 하는 경우에는 세계/키트 소유자에 게 문의 하 여 콘텐츠 업데이트를 계획 하 고 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-115">If you are regularly using content that is owned by someone else and has been shared with you, contact the world/kit owner and make sure they are planning to update their content.</span></span>

> <span data-ttu-id="5b3c0-116">콘텐츠 작성자이 고 질문이 있거나 도움이 필요한 경우 지원 팀에 문의 하 여 도움을 받으세요. altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="5b3c0-116">If you are a content creator and you have questions or require assistance, please contact our support team for help: altvr.com/support</span></span>

## <a name="testing-your-spi-content"></a><span data-ttu-id="5b3c0-117">SPI 콘텐츠 테스트</span><span class="sxs-lookup"><span data-stu-id="5b3c0-117">Testing your SPI content</span></span>

<span data-ttu-id="5b3c0-118">AltspaceVR의 다음 미리 보기 버전을 사용 하 여 VR에서 새로 업데이트 된 콘텐츠를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-118">Use the following preview versions of AltspaceVR to test your newly updated content in VR.</span></span> <span data-ttu-id="5b3c0-119">미리 보기 버전은 테스트 목적 으로만 사용 되며 플랫폼의 일반적인 사용에는 사용 하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-119">The preview versions are for testing purposes only, and shouldn't be used for a general use of the platform.</span></span>

* [<span data-ttu-id="5b3c0-120">Windows Mixed Reality AltspaceVR SPI 미리 보기</span><span class="sxs-lookup"><span data-stu-id="5b3c0-120">AltspaceVR SPI Preview for Windows Mixed Reality</span></span>](https://aka.ms/AvrSpiMr)
* [<span data-ttu-id="5b3c0-121">SteamVR에 대 한 AltspaceVR SPI 미리 보기</span><span class="sxs-lookup"><span data-stu-id="5b3c0-121">AltspaceVR SPI Preview for SteamVR</span></span>](https://aka.ms/AvrSpiSteam)
* [<span data-ttu-id="5b3c0-122">AltspaceVR SPI Preview for Oculus Rift</span><span class="sxs-lookup"><span data-stu-id="5b3c0-122">AltspaceVR SPI Preview for Oculus Rift</span></span>](https://aka.ms/AvrSpiRift)

> <span data-ttu-id="5b3c0-123">참고: PC VR 미리 보기만 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-123">Note: Only PC VR previews have been provided.</span></span> <span data-ttu-id="5b3c0-124">단일 패스 인스턴스화된 렌더링은 Android에서 사용할 수 없으며, Mac과 같은 VR 이외의 플랫폼에서는 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-124">Single pass instanced rendering is not available on Android, and is not needed on non-VR platforms like Mac.</span></span> <span data-ttu-id="5b3c0-125">따라서 일반 릴리스 버전을 사용 하 여 이러한 장치를 테스트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-125">Thus, you can use the general release version to test these devices.</span></span>


## <a name="storecompatibilitycheck"></a><span data-ttu-id="5b3c0-126">저장소 호환성 검사</span><span class="sxs-lookup"><span data-stu-id="5b3c0-126">Store Compatibility Check</span></span>

<span data-ttu-id="5b3c0-127">Unity 2020.3.9 업그레이드는 헤드셋 및 스토어 빌드 호환성에도 영향을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-127">The upgrade to Unity 2020.3.9 will also affect headset and store-build compatibility.</span></span> <span data-ttu-id="5b3c0-128">이제 헤드셋과 호환 되는 스토어에서 AltspaceVR를 다운로드 하는 것이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-128">It's now a requirement that you download AltspaceVR from the store that is compatible with your headset.</span></span> <span data-ttu-id="5b3c0-129">예를 들어 WinMR 또는 Oculus 헤드셋의 경우 Windows 스토어 또는 Oculus 스토어에서 각각 AltspaceVR를 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-129">As an example: For a WinMR or Oculus headset, download AltspaceVR from the Windows Store or Oculus Store, respectively.</span></span> <span data-ttu-id="5b3c0-130">Windows Mixed Reality 사용자는 Windows 스토어에서 AltspaceVR를 다운로드 하 고, 스트림의 사용자를 SteamVR 하 고, Oculus 매장에서 사용자를 다운로드 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-130">Windows Mixed Reality users should download AltspaceVR from the Windows Store, SteamVR users from Steam, and Oculus Rift users from the Oculus Store.</span></span>

## <a name="altspacevr-uploader-v090-upgrade-guide"></a><span data-ttu-id="5b3c0-131">AltspaceVR 업 로더 v 0.9.0 업그레이드 가이드</span><span class="sxs-lookup"><span data-stu-id="5b3c0-131">AltspaceVR Uploader v0.9.0 Upgrade Guide</span></span> 

<span data-ttu-id="5b3c0-132">업 로더 0.9는 이전 버전의 업 로더와 다르게 패키지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-132">Uploader 0.9 is packaged differently than previous versions of the Uploader.</span></span> <span data-ttu-id="5b3c0-133">이 패키징을 변경 하는 동시에 새 업 로더를 사용 하려면 새 버전의 Unity가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-133">Simultaneous with this packaging change, the new Uploader requires a new version of Unity.</span></span> <span data-ttu-id="5b3c0-134">이 가이드는이 업그레이드 프로세스를 더 안전 하 고 관련 된 모든 사용자에 게 제공 하기 위한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-134">This guide is intended to make this upgrade process smoother and safer for all who are involved.</span></span>

1. <span data-ttu-id="5b3c0-135">**프로젝트 백업** -전체 프로젝트 디렉터리의 복사본을 만들어 안전한 위치에 배치 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-135">**BACK UP YOUR PROJECT** - Create a copy of your entire project directory, and put it somewhere safe.</span></span> <span data-ttu-id="5b3c0-136">이 업그레이드는 파괴적인 업그레이드 이므로 완료 된 후에 Unity 2019.4에 대 한 번들을 만들거나 업로드할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-136">This upgrade is a destructive upgrade, so you won't be able to create or upload bundles for Unity 2019.4 after you complete it.</span></span> <span data-ttu-id="5b3c0-137">업그레이드 하는 동안 문제가 발생 하는 경우 다시 사용할 프로젝트의 정리 된 복사본이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-137">If you come across any problems during this upgrade, you'll NEED a clean copy of your project to fall back on.</span></span> <span data-ttu-id="5b3c0-138">Unity 2020.3.9로 공식적으로 업그레이드 하기 전에 라이브 키트 또는 템플릿을 업데이트 하는 데에도이 AltspaceVR 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-138">You'll also need it to update any live kits or templates before AltspaceVR officially upgrades to Unity 2020.3.9.</span></span>

2. <span data-ttu-id="5b3c0-139">**이전 업 로더 제거** -Unity를 닫은 후 다음 파일/폴더를 삭제 합니다. 해당 하는 메타 파일은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-139">**REMOVE OLD UPLOADER** - With Unity closed, delete the following files/folders, and it's corresponding .meta files:</span></span>

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. <span data-ttu-id="5b3c0-140">**엔진 버전 다운로드** -unity 허브를 열고 unity 2020.3.9를 설치 합니다 (또는 직접 설치 하려면 [여기를 클릭](https://unity3d.com/ru/unity/whats-new/2020.3.9) ).</span><span class="sxs-lookup"><span data-stu-id="5b3c0-140">**DOWNLOAD ENGINE VERSION** - Open the Unity Hub, and install Unity 2020.3.9 (or [click here](https://unity3d.com/ru/unity/whats-new/2020.3.9) to install directly).</span></span>

4. <span data-ttu-id="5b3c0-141">**프로젝트 업그레이드** -unity 2020.3.9에서 정리 프로젝트를 열고 unity에서 프로젝트를 업그레이드 하도록 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-141">**UPGRADE PROJECT** - Open your cleaned project in Unity 2020.3.9, and allow Unity to upgrade your project.</span></span>

5. <span data-ttu-id="5b3c0-142">(PC만 해당) **혼합 현실 기능 도구 다운로드** -지침에 따라 업 로더 패키지의 설치를 관리 하는 데 사용할 [혼합 현실 기능 도구](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)를 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-142">(PC Only) **DOWNLOAD MIXED REALITY FEATURE TOOL** - Follow the instructions to download the [Mixed Reality Feature Tool](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool), which you'll use to manage the installation of the Uploader package.</span></span>

6. <span data-ttu-id="5b3c0-143">**업 로더를 설치** 합니다. MR 기능 도구를 사용 하 여 Unity 프로젝트를 선택 하 고 AltspaceVR 제목 아래에 AltspaceVR 업 로더 기능을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-143">**INSTALL THE UPLOADER** - Use the MR Feature Tool to select your Unity project, and add the AltspaceVR Uploader feature (under the AltspaceVR heading).</span></span> <span data-ttu-id="5b3c0-144">도구의 지시를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-144">Follow the instructions in the tool.</span></span>

<span data-ttu-id="5b3c0-145">MacOS에서 [레지스트리에서](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)최신 버전을 수동으로 다운로드 하 고 Unity 편집기의 패키지 관리자 (Windows > 패키지 관리자 > + > tarball에서 패키지 추가) 내에서 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-145">On macOS, manually download the latest version from the [registry](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions), and install it from within the Unity Editor's package manager (Windows > Package Manager > + > Add package from tarball).</span></span>

<span data-ttu-id="5b3c0-146">패키지가 가져오기를 완료 하면 친숙 한 업 로더 창이 AltspaceVR 메뉴 항목에서 사용 가능 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-146">Once the package finishes importing, the familiar Uploader window should be available in the AltspaceVR menu item.</span></span>

## <a name="troubleshooting-tips"></a><span data-ttu-id="5b3c0-147">문제 해결 팁</span><span class="sxs-lookup"><span data-stu-id="5b3c0-147">Troubleshooting Tips</span></span>

1. <span data-ttu-id="5b3c0-148">WinMR 헤드셋에 컨트롤러 또는 입력 문제가 있는 경우 현재 상태 센서를 제대로 활용 하려면 헤드에 배치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-148">If you're having controller or input issues on your WinMR headset, ensure it's positioned on your head to properly engage the presence sensor.</span></span> <span data-ttu-id="5b3c0-149">이것은 알려진 문제 이며 Microsoft에서 문제를 해결 하기 위해 적극적으로 노력 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-149">This is a known issue and Microsoft is actively working to resolve it.</span></span>

2. <span data-ttu-id="5b3c0-150">헤드셋 및 스토어 빌드 호환성을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-150">Check your headset and store-build compatibility.</span></span> <span data-ttu-id="5b3c0-151">예를 들어 WinMR 헤드셋을 사용 하는 경우 Windows 스토어를 통해 AltspaceVR 빌드를 가져왔는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-151">If you're using a WinMR headset, for example, make sure that your AltspaceVR build was acquired through the Windows Store.</span></span>

3. <span data-ttu-id="5b3c0-152">테스트 하는 동안 콘텐츠가 VR 모드에서 한 눈에만 표시 되는 경우 사용 하는 사용자 지정 셰이더가 SPI 렌더링을 지원 하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-152">If during testing you discover that your content only appears in one eye in VR mode, it is likely that the custom shaders you use do not support SPI rendering.</span></span> <span data-ttu-id="5b3c0-153">다른 셰이더를 선택 하거나 [Unity의 SPI 업그레이드 가이드](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 에 따라 셰이더를 수동으로 편집 하 고 지원을 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-153">You’ll need to choose a different shader, or follow [Unity’s SPI upgrade guide](https://docs.unity3d.com/Manual/SinglePassInstancing.html) to manually edit the shader and add support.</span></span>

4. <span data-ttu-id="5b3c0-154">WinMR의 경우 AltspaceVR에서 VR 모드에 액세스 하려면 먼저 다음을 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-154">For those on WinMR, please remember that before you can access VR mode in AltspaceVR, you must:</span></span> 
    1. <span data-ttu-id="5b3c0-155">Microsoft Store에서 Windows Mixed Reality 용 OpenXR를 다운로드 하 여 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-155">Download and install OpenXR for Windows Mixed Reality from the Microsoft Store.</span></span>
        1. <span data-ttu-id="5b3c0-156">혼합 현실 포털 앱을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-156">Open the Mixed Reality Portal app</span></span>
        2. <span data-ttu-id="5b3c0-157">앱의 왼쪽 아래에 있는 "자세히 보기"를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-157">On the lower-left corner of the app select "See More"</span></span>
        3. <span data-ttu-id="5b3c0-158">표시 되는 메뉴에서 OpenXR 설정을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-158">In the menu that appears select Set Up OpenXR.</span></span> <span data-ttu-id="5b3c0-159">이렇게 하면 Windows 스토어가 런타임을 설치할 수 있는 위치에서 시작 됩니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-159">Doing this will cause the Windows Store to launch from where you can install the runtime.</span></span> <span data-ttu-id="5b3c0-160">이 메뉴 항목이 표시 되지 않으면 OpenXR가 PC에 이미 설치 되어 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5b3c0-160">If this menu item does not appear, OpenXR may already be installed on your PC.</span></span>