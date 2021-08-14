---
title: Unity 업로더 도움말
description: AltspaceVR Unity 업로더에 대한 자주 묻는 최신 질문과 해결 방법을 최신 상태로 유지하세요.
ms.date: 02/10/2021
ms.topic: article
keywords: 도움말, faq
ms.openlocfilehash: cb983ba4e23186f7cc62043f75e7ea1b2969e92b6bd30b132f1733b5e25e92dd
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125699"
---
# <a name="unity-uploader-help"></a>Unity 업로더 도움말

**1. 이 도구는 얼마나 멋진가요?**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

게이트 및 DND를 구동하는 SDK 앱이 있는 내 Stargate Unity 장면입니다.

**2. 비디오 학습자입니다. 내 비디오는 어디에 있나요?**

[비디오 확인](https://youtu.be/km9CnVYPzoM)

**3. 예제는 어디서 찾을 수 있나요?**

[주요 세계 및](https://account.altvr.com/worlds/featured) [Jimmy의 예제를](https://account.altvr.com/worlds/1046572460192825569) 시작하는 것이 좋습니다.

**4. 키트 및 새 SDK에서 작동합니까?**
예, 원하는 경우 모든 도구를 함께 사용할 수 있습니다. 원활하게 함께 작동하도록 개발하려고 합니다.

**5. 파티클 효과를 지원하나요?**

![눈 파티클 효과의 GIF](images/uploader-faq-img-01.gif)

**6. 공간화된 오디오를 얻을 수 있나요?**
지금은 아니지만 지역화된 영역에서 재생할 오디오 원본을 배치할 수 있습니다. 

**7. 베이킹 조명이 작동하나요?**
예, 하지만 조명은 "혼합"이 아닌 "베이킹"으로 설정해야 합니다.

**8. 전역 조명이 작동하나요?**
Yes

**9. 항상 세계를 다시 설정해야 합니까?**
예. 매번 Unity 자산 번들을 다시 로드해야 합니다. 

**10. 사용자 지정 재질 및 셰이더를 사용할 수 있나요?**

![사용자 지정 재질 및 셰이더의 GIF](images/uploader-faq-img-02.gif)

**11. 하나의 플랫폼에만 업로드할 수 있나요?**
예, 업로더 도구를 사용합니다. 그러나 Android에 있는 사람들은 해당 플랫폼에 대한 장면을 업로드할 때까지 세계에 아무것도 표시되지 않습니다. 

**12. 스크립트가 허용된가요?**
아니요, 보안상의 이유로 스크립트 또는 스크립트 참조를 허용할 수 없습니다. 업로드에 스크립트 또는 스크립트 참조가 포함되어 있으면 거부됩니다. World에 스크립팅이 필요한 경우 새 SDK를 살펴보십시오. 

**13. 얼마나 큰 장면을 업로드할 수 있나요?**
소규모로 시작하여 Altspace에서 PC가 없는 사람들을 염두에 두는 것이 좋습니다. 즉, 라이브 스트림에 대한 맵을 가져오는 게임(예: VR 게임)이 있었습니다.

![AltspaceVR의 VR 게임 스크린샷](images/uploader-faq-img-03.png)

**14. 장면 파일을 호스트해야 합니까?**
아니요, Altspace는 파일을 업로드한 후 서비스를 제공합니다.

**15. 그림자가 허용된가요?**
Yes

**16. 업로더를 사용하여 얼마나 빨리 반복할 수 있나요?**
이미 세계에 있는 경우 업로더에서 업로드 누르고, 세계를 다시 설정하며, 업데이트된 장면을 10초 이내에 볼 수 있습니다. 일반적으로 장면의 복잡성에 따라 30초에서 몇 분까지의 루프가 표시됩니다. 커피 한 잔을 마셔도 됩니다. World-Builder가 될 수 있습니다.

**17. 3D 모델은 어디서 얻을 수 있나요?**
Sketchfab, Sketchup, Minecraft, Unity Asset Store 등입니다.

**18. 애니메이션을 지원하나요?**

![실행되는 사용자 지정 애니메이션의 GIF](images/uploader-faq-img-04.gif)

**19. 공간 오디오를 설정하기 위해 어떻게 해야 합니까?** 선택한 wav 파일을 가져오고, 장면에서 빈 게임 개체를 만들고, 이 개체를 선택합니다. 가져온 소리를 개체의 검사기로 끌어서 놓으면 오디오 원본이 만들어집니다. 그런 다음 볼륨을 0.5 이하로 조정하고, 공간 혼합을 3D로 변경하고, 최소 및 최대 거리를 조정하여 적절한 소리 영역을 만듭니다. 기본적으로 충돌체와 같은 구로 표시됩니다. 진정한 드롭오프를 얻으려면 드롭오프 곡선을 원하는 대로 조정해야 합니다. [(를 @IsThatToasted 통해)](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20. 크로스-비동기/불충분은 어떻게 표시하나요?**
업로더가 렌더링 설정을 재정의하지 못하는 경우가 있습니다. "편집 > Project 설정 > 플레이어로 이동". PC와 Android 모두에 대해 "XR 설정 > Virtual Reality Supported"가 선택되어 있고 "스테레오 렌더링 방법"이 "Single Pass" 또는 "Single Pass(미리 보기)"인지 확인합니다(로봇 아이콘 선택). 그런 다음, + 업로드를 다시 빌드하고 세계를 다시 설정합니다. 