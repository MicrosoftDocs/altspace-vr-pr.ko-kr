---
title: 인 글 Tf 모델 가져오기
description: 3D가 나 AltspaceVR 환경을 적절 하 게 가져오고 문제를 해결 하는 방법에 대해 알아봅니다.
ms.date: 03/11/2021
ms.topic: article
keywords: 모델,가 중, 가져오기, sketchfab, 문제 해결
ms.openlocfilehash: 4489f90832bd1cf85ff161caed11684257cce6ab
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213257"
---
# <a name="importing-gltf-models"></a><span data-ttu-id="1c345-104">인 글 Tf 모델 가져오기</span><span class="sxs-lookup"><span data-stu-id="1c345-104">Importing glTF models</span></span>

> [!NOTE]
> <span data-ttu-id="1c345-105">이 기능은 초기 액세스 프로그램에서 선택한 사용자에 게 제공 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-105">This feature is available for select users in the Early Access program at this time.</span></span>

<span data-ttu-id="1c345-106">3D 모델 및 장면을 Altspace으로 가져오는 한 가지 방법은 [글 tf 표준](https://en.wikipedia.org/wiki/GlTF)을 사용 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-106">One way to bring 3D models and scenes into Altspace is using the [glTF standard](https://en.wikipedia.org/wiki/GlTF).</span></span> <span data-ttu-id="1c345-107">나중에 세계 편집기에서 생성할 수 있는 모델을 만들기 위해 .bb 파일 (압축 된 고 지 수)을 업로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-107">You can upload a .glb file (packed glTF) to create a Model that you can later spawn in the World Editor.</span></span> <span data-ttu-id="1c345-108">사용자 [고유의 키트를 업로드](uploading-custom-kits.md)하는 대신 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-108">It's an alternative to [uploading your own Kits](uploading-custom-kits.md).</span></span> <span data-ttu-id="1c345-109">성능 및 재사용을 최대화 하려는 경우 Unity 및 키트를 사용할 필요가 없기 때문에 신속한 데모를 위한 모델을 만드는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-109">We recommend creating Models for quick demonstrations because you won't need to use Unity, and Kits when you want to maximize performance and reusability.</span></span> 

1. <span data-ttu-id="1c345-110">몇 가지 유용한 3D 자산을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-110">Find some glTF 3D assets.</span></span> <span data-ttu-id="1c345-111">검색할 한 곳은 Sketchfab (예: **다운로드 가능한** 모델에 대해 필터링 [시도).](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)</span><span class="sxs-lookup"><span data-stu-id="1c345-111">One place to search is Sketchfab (try filtering for **Downloadable** models like [this](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span></span> <span data-ttu-id="1c345-112">찾은 후 **3D 모델 다운로드** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-112">Once you find it, select **Download 3D Model**:</span></span>

![Sketchfab의 3D 강아지 모델](images/importing-models-img-01.png)

2. <span data-ttu-id="1c345-114">모델에 대 한 링크를 복사 하 고 라이선스 요구 사항을 읽습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-114">Copy the link to the model and read the licensing requirements.</span></span> 
3. <span data-ttu-id="1c345-115">**자동 변환 된 형식 (글 tf)** 버전 다운로드</span><span class="sxs-lookup"><span data-stu-id="1c345-115">Download the **Autoconverted Format (glTF)** version</span></span>

![자동 변환 된 서식을 사용 하는 Sketchfab 다운로드 옵션 강조 표시](images/importing-models-img-02.png)

4. <span data-ttu-id="1c345-117">인 사이트를 열고 **PNG를 JPEG (베타)로 변환** 상자를 [선택 합니다.](https://glb-packer.glitch.me)</span><span class="sxs-lookup"><span data-stu-id="1c345-117">Open the [GLB Packer](https://glb-packer.glitch.me) site and check the box **Convert PNG to JPEG (beta)**</span></span>
5. <span data-ttu-id="1c345-118">다운로드 한 글 어 파일의 압축을 풀고 모든 항목을 한 번에 한 번에 끌어서 브라우저 탭으로 끌어서 놓습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-118">Uncompress the glTF files you downloaded and drag them all at once into the GLB Packer browser tab</span></span>

![모델 압축 해제를 표시 하는 창](images/importing-models-img-03.png)

6. <span data-ttu-id="1c345-120">파일의 수와 크기에 따라 처리 하는 데 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-120">Depending on the number and size of the files, it may take a while to process.</span></span> <span data-ttu-id="1c345-121">처리가 완료 되 면 **출력** 파일이 다운로드 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-121">When processing is done, an **out.glb** file will be downloaded.</span></span> <span data-ttu-id="1c345-122">해당 파일의 이름을 정보로 바꿉니다 .이는 세계의 개체 이름입니다 (예: **Low Poly).**</span><span class="sxs-lookup"><span data-stu-id="1c345-122">Rename that file to something informative--this will be the name of the object in the world (e.g **Low Poly Wolf.glb**)</span></span>
7. <span data-ttu-id="1c345-123">[Altvr.com > 더 많은 > 모델로](https://account.altvr.com/users/sign_in) 이동 하 고 **만들기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-123">Navigate to [altvr.com > More > Models](https://account.altvr.com/users/sign_in) and select **Create**</span></span>
8. <span data-ttu-id="1c345-124">.Bb 파일의 위치를 지정 하 고 Sketchfab 링크를 특성의 설명에 복사 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-124">Specify the location of the .glb file and make sure you copy the Sketchfab link into the description for attribution.</span></span> <span data-ttu-id="1c345-125">원하는 경우 미리 보기 이미지를 지정 하 고 **모델 만들기** 를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-125">You can specify a preview image if you want, then select **Create Model**:</span></span>

![AltspaceVR의 모델 미리 보기](images/importing-models-img-04.png)

9. <span data-ttu-id="1c345-127">**클립보드로 복사를 선택 합니다** .</span><span class="sxs-lookup"><span data-stu-id="1c345-127">Select **Copy to Clipboard**</span></span>
10. <span data-ttu-id="1c345-128">**세계 편집기 > Altspace > 기본 사항 >** 공개 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-128">Open the **World Editor > Altspace > Basics > GLTF**</span></span>
11. <span data-ttu-id="1c345-129">Url에 붙여 넣고 **확인** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-129">Paste in your url and select **Confirm**</span></span>

<span data-ttu-id="1c345-130">축하합니다!</span><span class="sxs-lookup"><span data-stu-id="1c345-130">Congrats!</span></span> <span data-ttu-id="1c345-131">방금 첫 번째 모델을 생성 했습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-131">You just spawned your first Model.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1c345-132">문제 해결</span><span class="sxs-lookup"><span data-stu-id="1c345-132">Troubleshooting</span></span>

<span data-ttu-id="1c345-133">**클릭 한 내용이 **없는지 확인** 합니다.**</span><span class="sxs-lookup"><span data-stu-id="1c345-133">**When I clicked **Confirm** nothing happened**</span></span>
    * <span data-ttu-id="1c345-134">현재는 100,000 개의 다각형 한도가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-134">We currently have a 100k polygon limit.</span></span> <span data-ttu-id="1c345-135">실패 한 경우 개체를 삭제 하 여 전 세계에 참가 하는 사용자의 잠재적인 문제를 방지 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-135">If it fails, delete the Object to avoid potential problems with users joining your World</span></span>
    * <span data-ttu-id="1c345-136">자산에 다른 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-136">There may be other problems with the asset.</span></span> <span data-ttu-id="1c345-137">가능한 한 적은 수의 다각형이 포함 된 자산을 사용 하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-137">Try to use assets with as few polygons as possible.</span></span>
    * <span data-ttu-id="1c345-138">가져오는 모델이 작거나 클 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-138">The model you're bringing in may be small or large.</span></span> <span data-ttu-id="1c345-139">규모를 늘리거나 줄여 보거나 아바타를 이동 해 보세요. 모델 내부에 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-139">Try increasing/decreasing the Scale or move your avatar around, you might be standing inside the model!</span></span>

<span data-ttu-id="1c345-140">**로드 속도가 느립니다** . 전 세계의 다른 사용자가이를 로드 하는 속도는 연결 속도에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-140">**It's slow to load** How quickly other users in the World load it will depend on their connection speeds.</span></span> <span data-ttu-id="1c345-141">또한 키트 자산과 마찬가지로 캐시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-141">It's also not cached like Kit assets.</span></span> <span data-ttu-id="1c345-142">홈에 저장 한 경우에는 조인할 때마다 동일한 모델을 다시 다운로드 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-142">If you place one in your Home, you'll end up redownloading the same Model every time you join, which isn't great.</span></span>

<span data-ttu-id="1c345-143">**충돌이 발생 하지 않습니다** . 기본적으로 이러한 방식으로 가져오는 개체에는 충돌이 발생 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-143">**There's no collision** By default there's no collision on the objects that are brought in this way</span></span>

<span data-ttu-id="1c345-144">**이를 생성 하면 6 개의 DOF에서 컨트롤이 손실 되거나 내부에 있으므로 조작 하기 어렵습니다** . 예, 이러한 문제를 알고 있으며 곧 해결할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1c345-144">**When I spawn it, I lose my controls on six DOF or I'm inside so it's hard to manipulate it** Yes, we're aware of these issues and hope to address them soon.</span></span>  