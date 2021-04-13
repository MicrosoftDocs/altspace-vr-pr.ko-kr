---
title: AltspaceVR가 동작 sickness을 야기 하나요?
description: VR 환경에서 진행 sickness에 대 한 최신 질문과 대답을 최신 상태로 유지 합니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 동작 sickness, vr, nausea
ms.openlocfilehash: 54f746bc2b213f011dbf94c2703ed039b4717d72
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213369"
---
# <a name="will-altspacevr-cause-motion-sickness"></a><span data-ttu-id="bbc10-104">AltspaceVR가 동작 sickness을 야기 하나요?</span><span class="sxs-lookup"><span data-stu-id="bbc10-104">Will AltspaceVR cause motion sickness?</span></span>

## <a name="why-do-some-people-feel-ill-in-vr"></a><span data-ttu-id="bbc10-105">몇 명의 사용자가 VR에서 잘못 생각 하는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="bbc10-105">Why do some people feel ill in VR?</span></span>

<span data-ttu-id="bbc10-106">모든 VR에서 vertigo 및 nausea를 야기 하는 인기 있는 하다 신념으로입니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-106">It's a popular belief that all VR causes vertigo and nausea.</span></span> <span data-ttu-id="bbc10-107">이 문제는 눈에 보이는 내용과 내부 귀를 두뇌에 게 전송 하는 것 간의 불일치를 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-107">The problem stems from a discrepancy between what your eyes are seeing, and what your inner ear is transmitting to your brain.</span></span> <span data-ttu-id="bbc10-108">눈이 동작을 감지 하 고 귀는 계속 해 서 지속적으로 유도 dizziness 및 nausea에 대응할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-108">When your eyes detect motion, and your ears communicate that you're standing still, some individuals' brain may react by inducing dizziness and nausea.</span></span> <span data-ttu-id="bbc10-109">동작 sickness에 더 많은 영향을 주는 일부 사람들은 이러한 현상에 더 중요 한 것이 고 다른 사람들에 게는 문제가 없을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-109">Some people who are more susceptible to motion sickness may be more sensitive to this phenomenon, while others may not have an issue with it.</span></span> 

<span data-ttu-id="bbc10-110">하드웨어 수준에서 몇 가지 작업을 수행 하 고, AltspaceVR의 소프트웨어에서 몇 가지 작업을 수행 하 여 VR의 nausea 유도 동작을 심각 하 게 줄이거나 완전히 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-110">There are several things that are done at the hardware level, and some in AltspaceVR's software that severely reduces or completely eliminate the nausea-inducing motion in VR.</span></span>

## <a name="hardware-based-nausea-reduction"></a><span data-ttu-id="bbc10-111">Hardware-Based Nausea 감소</span><span class="sxs-lookup"><span data-stu-id="bbc10-111">Hardware-Based Nausea Reduction</span></span>

<span data-ttu-id="bbc10-112">Oculus Rift 및 HTC Vive와 같은 최신 VR 하드웨어는 nausea를 발생 시킬 수 있는 대기 시간을 제거 하는 속도로 비디오 프레임을 제시 하 여 동작 sickness를 줄입니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-112">Contemporary VR hardware like the Oculus Rift and HTC Vive, reduces motion sickness by presenting video frames at a rate that eliminates the latency that can cause nausea.</span></span> <span data-ttu-id="bbc10-113">소프트웨어를 최적화 하는 경우에는 AltspaceVR가 사용 되는 경우에는 VR의 헤드를 켤 때 인식 된 지연 시간이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-113">If the software is optimized, as AltspaceVR is, then there's no perceived delay when you turn your head in VR.</span></span> <span data-ttu-id="bbc10-114">HMD의 accelerometers은 이동 통신을 진행 하 고 사용자가 대기 시간을 검색할 수 있는 것 보다 더 빠르게 해당 원격 분석을 전송 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-114">The accelerometers in the HMD are communicating movement and transmitting that telemetry faster than the human eye can detect any latency.</span></span> <span data-ttu-id="bbc10-115">HMD 모델에서 위치 카메라를 outfitted 하는 경우에는이 단계가 더 진행 됩니다. 회전 이동이 표시 되는 것이 아니라 측면 (사이드 to side) 동작입니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-115">On HMD models outfitted with positional cameras, this goes a step further, not only is rotational movement represented, so is lateral (side to side) motion.</span></span>

## <a name="software-based-nausea-reduction"></a><span data-ttu-id="bbc10-116">Software-Based Nausea 감소</span><span class="sxs-lookup"><span data-stu-id="bbc10-116">Software-Based Nausea Reduction</span></span>

<span data-ttu-id="bbc10-117">AltspaceVR는 하드웨어 개선 및 framerate 외에도 사용자가 nausea를 줄이고 제거할 수 있도록 지 원하는 몇 가지 기능을 구현 했습니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-117">In addition to hardware improvements and framerates, AltspaceVR has implemented several features that help people reduce and eliminate nausea:</span></span>

* <span data-ttu-id="bbc10-118">**Teleporting** -지점 간에 이동 하는 것은 동작을 두뇌로 전달 하 여 동작 sickness을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-118">**Teleporting** - Moving instantaneously from point-to-point doesn't communicate motion to the brain, thereby eliminating motion sickness.</span></span>
* <span data-ttu-id="bbc10-119">**Snap 켜는** 모든 하드웨어 ALTSPACEVR는 VR에서 보기의 "ratcheted" 또는 "단계별" 회전을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-119">**Snap Turning** - On all hardware, AltspaceVR provides means for "ratcheted" or "stepped" rotation of the view in VR.</span></span> <span data-ttu-id="bbc10-120">즉, 보기를 켜면 20 도씩 회전 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-120">In other words when turning, your view will pivot about 20 degrees of rotation.</span></span> <span data-ttu-id="bbc10-121">이는 대부분의 사람들에 nausea를 트리거하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-121">Again, this doesn't trigger nausea in most people.</span></span>
* <span data-ttu-id="bbc10-122">**맞추기 동작** -특정 하드웨어에서 터치 패드를 앞으로 밀어 sickness 동작을 트리거하지 않는 증분에서 큐브 뷰를 앞으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-122">**Snap Motion** - On certain hardware, swiping forward on the touchpad will move the perspective forward in an increment that doesn't trigger motion sickness.</span></span> 
 
## <a name="suggestions-for-eliminating-motion-sickness"></a><span data-ttu-id="bbc10-123">동작 Sickness 제거에 대 한 제안</span><span class="sxs-lookup"><span data-stu-id="bbc10-123">Suggestions for Eliminating Motion Sickness</span></span>

<span data-ttu-id="bbc10-124">**계속**</span><span class="sxs-lookup"><span data-stu-id="bbc10-124">**Stand Still**</span></span>

<span data-ttu-id="bbc10-125">컨트롤러를 사용 하 여 너무 많이 이동 해서는 안 됩니다 .이 경우에는 h t t p/또는 위쪽/아래쪽으로 이동 하 여 VR를 확인 하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-125">Try not to move around too much using the controllers, just rotate your head/or up/down to look around in VR.</span></span>

<span data-ttu-id="bbc10-126">**마우스/k b 또는 컨트롤러 사용 안 함**</span><span class="sxs-lookup"><span data-stu-id="bbc10-126">**Don't Use a Mouse/KB or Controller**</span></span>

<span data-ttu-id="bbc10-127">AltspaceVR는 비디오 게임과 같이 사용자에 게 마우스/키보드 및 게임 컨트롤러와 같은 표준 게임 주변 장치를 사용 하 여 VR로 이동할 수 있는 옵션을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-127">AltspaceVR offers users the option to use standard gaming peripherals such as Mouse/Keyboard and Game controllers to move in VR as you would in a video game.</span></span> <span data-ttu-id="bbc10-128">여기에는 여러 방향 이동, strafing 및 터보 단추가 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-128">This includes multi-directional movement, strafing, and a turbo button.</span></span> <span data-ttu-id="bbc10-129">이는 VR에 익숙한 후에만 사용 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-129">We recommend using these only after becoming accustomed to being in VR.</span></span> <span data-ttu-id="bbc10-130">이 경우에도 속도가 느립니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-130">Even then, take it slow.</span></span>

<span data-ttu-id="bbc10-131">**언제 든 지 Bail 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="bbc10-131">**You Can Always Bail Out**</span></span>

<span data-ttu-id="bbc10-132">Nausea을 경험 하는 경우 HMD를 즉시 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-132">If you experience nausea, remove your HMD immediately.</span></span> <span data-ttu-id="bbc10-133">Stomach을 확보 하 고, 준비가 되 면 VR 환경으로 돌아갈 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-133">Regain your equilibrium, calm your stomach, and when ready return to the VR environment.</span></span> <span data-ttu-id="bbc10-134">하루아침를 발생 시킨 이동을 잊지 말고 반복 해 보세요.</span><span class="sxs-lookup"><span data-stu-id="bbc10-134">Try to remember the movement that caused the sensation and refrain from repeating it.</span></span>

<span data-ttu-id="bbc10-135">**VR 종료 시점을 알 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="bbc10-135">**Know When it's Time to Exit VR**</span></span>

<span data-ttu-id="bbc10-136">가장 중요 한 점은 언제 중단 될 때를 알고 있어야 한다는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-136">Most importantly, know when it's time to take a break.</span></span> <span data-ttu-id="bbc10-137">본문을 알고 있으며, 무언가 잘못 되었음을 나타내는 강력한 표시를 제공 하는 경우 수신 대기 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-137">You know your body, and when it's giving you strong indication that something is wrong, listen.</span></span> <span data-ttu-id="bbc10-138">중단 하 고 일부 공기를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-138">Take a break and get some air.</span></span> <span data-ttu-id="bbc10-139">평형을 탐색 하 고 다시 조정 합니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-139">Walk around and realign your equilibrium.</span></span> <span data-ttu-id="bbc10-140">다시 양호 하다 고 생각 되 면 파티를 계속 진행 하 고 있음을 확신 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="bbc10-140">Once you feel good again, come back, we're confident the party will still be going!</span></span>