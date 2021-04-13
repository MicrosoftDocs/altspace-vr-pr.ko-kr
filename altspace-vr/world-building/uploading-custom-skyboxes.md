---
title: 사용자 지정 Skyboxes 업로드
description: AltspaceVR 환경에서 사용자 지정 skyboxes을 업로드 하 고 문제를 해결 하는 방법에 대 한 단계별 지침을 확인 하세요.
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes, 문제 해결
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213264"
---
# <a name="uploading-custom-skyboxes"></a><span data-ttu-id="af6e1-104">사용자 지정 Skyboxes 업로드</span><span class="sxs-lookup"><span data-stu-id="af6e1-104">Uploading custom Skyboxes</span></span>

<span data-ttu-id="af6e1-105">Skybox 환경을 더 몰입로 만드는 세계에 대 한 **배경을** 만드는 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-105">A Skybox is a way to create a **background** for your World that makes the experience more immersive.</span></span> <span data-ttu-id="af6e1-106">다양 한 종류의 Skyboxes 있지만 현재는 **등 장방형** 를 지원 합니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-106">There are different kinds of Skyboxes but we currently support **equirectangular**.</span></span> <span data-ttu-id="af6e1-107">다음은 360 카메라를 사용 하는 예제입니다 (추가 예제 [참조).](http://moments.mankindforward.com/)</span><span class="sxs-lookup"><span data-stu-id="af6e1-107">Here's an example taken with a 360 camera (more example [here](http://moments.mankindforward.com/)):</span></span> 

![등 장방형 실내의 360 보기](images/custom-skyboxes-img-01.jpeg)

<span data-ttu-id="af6e1-109">[Unity 업 로더](world-building-toolkit-getting-started.md) 를 사용할 수도 있지만이 방법은 더 간단 합니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-109">You can also use the [Unity Uploader](world-building-toolkit-getting-started.md) but this approach is simpler.</span></span>

1. <span data-ttu-id="af6e1-110">[> Skyboxes](https://account.altvr.com/skyboxes) 로 이동 하 여 오른쪽에 있는 **만들기** 단추를 누릅니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-110">Navigate to [Worlds > Skyboxes](https://account.altvr.com/skyboxes) and press the **Create** button on the right</span></span>

![Skyboxes 패널에 연결 되는 웹 사이트 페이지](images/custom-skyboxes-img-02.png)

2. <span data-ttu-id="af6e1-112">이름을 입력 하 고 360 이미지를 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-112">Fill in a name and specify your 360 image.</span></span> <span data-ttu-id="af6e1-113">사진이 될 필요는 없으며, 사용자가 직접 그리거나 온라인으로 검색할 수 있는 프로그램이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-113">It doesn't have to be a photo, there are programs that let you draw your own or you can search for some online.</span></span> <span data-ttu-id="af6e1-114">준비가 되면 **만들기** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-114">When you're ready, select **Create**.</span></span> 

![Skybox 만들기 양식](images/custom-skyboxes-img-03.png)

3. <span data-ttu-id="af6e1-116">이 skybox 쉽게 식별할 수 있도록 **미리 보기** 이미지를 선택적으로 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-116">You can optionally upload a **preview** image so you can easily identify this skybox.</span></span> <span data-ttu-id="af6e1-117">WAV 형식의 주변 오디오를 업로드할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-117">You can also upload ambient audio in WAV format.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="af6e1-118">360 이미지를 업로드 한 후 미리 보기 이미지와 주변 오디오를 별도로 업로드 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-118">We recommend you upload preview images and ambient audio separately, after you upload the 360 image.</span></span> <span data-ttu-id="af6e1-119">이러한 파일을 업로드 하는 경우 파일 크기는 프로세스를 정지 하기에 충분히 커질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-119">If you upload them together the file sizes can be large enough to stall the process.</span></span> <span data-ttu-id="af6e1-120">[Jetsons 세계](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) 는 주변 오디오와 함께 Skybox를 사용 하는 방법의 좋은 예입니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) is a great example of how to use a Skybox with ambient audio.</span></span> <span data-ttu-id="af6e1-121">세계 빌더가 오디오 볼륨 부족 및 들리는 소리를 유지 하는 방법을 확인 하는 것은 표정이.</span><span class="sxs-lookup"><span data-stu-id="af6e1-121">Notice how the World-Builder kept the audio volume low and sounds you hear are sporadic so people don't get annoyed.</span></span> 

4. <span data-ttu-id="af6e1-122">전 세계를 입력 하 고 전 세계 편집기를 여세요.</span><span class="sxs-lookup"><span data-stu-id="af6e1-122">Enter your World and open the World Editor.</span></span> <span data-ttu-id="af6e1-123">Skyboxes에서 새 Skybox를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-123">Under Skyboxes, select your new Skybox.</span></span> <span data-ttu-id="af6e1-124">몇 초 후에는 하늘이 변경 됩니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-124">In a few seconds, the sky will literally change.</span></span> <span data-ttu-id="af6e1-125">전 세계의 다른 사람들이 공중 변화를 볼 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-125">Others in your World will also see the sky change.</span></span> <span data-ttu-id="af6e1-126">다시 전환 하려면 동일한 목록에서 **기본** skybox를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-126">To switch back, choose the **default** skybox in that same list.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="af6e1-127">문제 해결</span><span class="sxs-lookup"><span data-stu-id="af6e1-127">Troubleshooting</span></span>

<span data-ttu-id="af6e1-128">**하늘:-(에는 조인트 또는 선이 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="af6e1-128">**There's a seam or line in the sky :-(.**</span></span> <span data-ttu-id="af6e1-129">곧 해결할 버그입니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-129">It's a bug that we'll fix soon</span></span>

<span data-ttu-id="af6e1-130">**업로드 실패**</span><span class="sxs-lookup"><span data-stu-id="af6e1-130">**Upload failed**</span></span>
    * <span data-ttu-id="af6e1-131">360 이미지만 업로드 해 보세요.</span><span class="sxs-lookup"><span data-stu-id="af6e1-131">try uploading just the 360 image on its own</span></span>
    * <span data-ttu-id="af6e1-132">다른 작은 파일을 테스트로 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="af6e1-132">try with another, smaller file as a test</span></span>

<span data-ttu-id="af6e1-133">**360 사진을 찾을 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="af6e1-133">**I can't find a 360 photo**</span></span>
    * <span data-ttu-id="af6e1-134">Flickr가 좋은 원본 (창의적인 commons 항목을 찾기 위해 필터 변경)</span><span class="sxs-lookup"><span data-stu-id="af6e1-134">Flickr is a good source (change the filters to find creative commons ones)</span></span>
    * <span data-ttu-id="af6e1-135">사용자 고유의 참여!</span><span class="sxs-lookup"><span data-stu-id="af6e1-135">Take your own!</span></span> <span data-ttu-id="af6e1-136">Ricoh의 카메라에 성공 했습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-136">We've had success with Ricoh's cameras.</span></span> 
<span data-ttu-id="af6e1-137">**하늘 모양이 거칠게 표시 되거나 blocky** 고해상도 이미지를 찾아야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-137">**The sky looks grainy or blocky** You may need to find a higher-resolution image.</span></span> <span data-ttu-id="af6e1-138">일반적으로 2-5 m b 및 ~ 5000 px x 2000 px</span><span class="sxs-lookup"><span data-stu-id="af6e1-138">Typically around 2-5 MB and ~5000 px x 2000 px</span></span>

<span data-ttu-id="af6e1-139">**세계의 프레임 속도가 아파!**</span><span class="sxs-lookup"><span data-stu-id="af6e1-139">**It hurts my World's framerate!**</span></span>
<span data-ttu-id="af6e1-140">이미지가 너무 클 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-140">The image is probably too large.</span></span> <span data-ttu-id="af6e1-141">일부 생성 된 skyboxes은 8k 일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-141">Some generated skyboxes can be 8k.</span></span> <span data-ttu-id="af6e1-142">일반적으로는이를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-142">They usually come with mobile-friendly 2k versions--use that.</span></span>

<span data-ttu-id="af6e1-143">**주변 오디오에 대 한 도움말**</span><span class="sxs-lookup"><span data-stu-id="af6e1-143">**Help me with the ambient audio**</span></span>
    * <span data-ttu-id="af6e1-144">Audacity와 같은 무료 소프트웨어를 사용 하 여 볼륨을 낮추고 사용자 고유의 루프를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-144">Use free software like Audacity to lower the volume or create your own loops.</span></span> <span data-ttu-id="af6e1-145">오디오가 반복 되 고 사용자의 귀를 재생 하는 것을 기억 하세요.</span><span class="sxs-lookup"><span data-stu-id="af6e1-145">Remember that the audio will be repeated and playing in people's ears so keep it low and not annoying</span></span>
    * <span data-ttu-id="af6e1-146">[무료 소리](https://freesound.org/) 는 로열티 없는 소리의 좋은 원본입니다.</span><span class="sxs-lookup"><span data-stu-id="af6e1-146">[Free Sound](https://freesound.org/) is a good source of royalty-free sounds</span></span>
