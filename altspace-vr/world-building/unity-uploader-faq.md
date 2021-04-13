---
title: Unity 업 로더 도움말
description: AltspaceVR Unity 업 로더에 대 한 최신 질문과 대답 및 솔루션을 최신 상태로 유지 합니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 도움말, faq
ms.openlocfilehash: 814ff293cb98490900cd929f33477d15d3d668ae
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213385"
---
# <a name="unity-uploader-help"></a>Unity 업 로더 도움말

**1 .이 도구는 어떻게 되나요?**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

이는 SDK 앱을 사용 하 여 게이트 및 DND를 켜는 내 Stargate Unity 장면입니다.

**2. 동영상 학습자는 어디 인가요?**

[비디오 확인](https://youtu.be/km9CnVYPzoM)

**3. 예를 어디에서 찾을 수 있나요?**

[주요 세계](https://account.altvr.com/worlds/featured) 및 [Jimmy의 예제](https://account.altvr.com/worlds/1046572460192825569) 는 시작 하는 데 적합 합니다.

**4 .이 작업은 키트와 새 SDK에서 작동 하나요?**
예, 원하는 경우 모든 도구를 함께 사용할 수 있습니다. 공동 작업을 위해 개발 하려고 노력 하 고 있습니다.

**5. 파티클 효과가 지원 되나요?**

![눈 파티클 효과의 GIF](images/uploader-faq-img-01.gif)

**6. spatialized 오디오를 받을 수 있나요?**
현재는 아니지만 오디오 소스를 지역화 된 영역에 저장할 수 있습니다. 

**7. 구운 조명이 작동 하나요?**
예, 하지만 조명을 "mixed"가 아닌 "구운"로 설정 해야 합니다.

**8. 글로벌 조명이 작동 하나요?**
예

**9. 항상 전 세계를 다시 설정 해야 하나요?**
예. 매번 Unity 자산 번들을 다시 로드 해야 합니다. 

**10. 나만의 사용자 지정 자료와 셰이더를 사용할 수 있나요?**

![사용자 지정 자료 및 셰이더의 GIF](images/uploader-faq-img-02.gif)

**11. 한 플랫폼에만 업로드할 수 있나요?**
예, 업 로더 도구를 사용 합니다. 그러나 Android를 수행 하는 사용자는 해당 플랫폼에 대 한 장면을 업로드할 때까지 전 세계에 아무것도 표시 되지 않습니다. 

**12. 스크립트가 허용 되나요?**
아니요, 보안상의 이유로 스크립트나 스크립트 참조를 허용할 수 없습니다. 업로드에 스크립트나 스크립트 참조가 포함 된 경우 거부 됩니다. 스크립팅이 필요한 경우 새 SDK를 살펴보세요. 

**13. 얼마나 큰 장면을 업로드할 수 있나요?**
사소한 Pc가 없는 Altspace의 사람들에 게는 사소한 시작을 제안 하는 것이 좋습니다. 즉, 게임에서 라이브 스트림의 맵 (예: 생일, VR 슈팅 게임)을 가져옵니다.

![AltspaceVR의 VR 게임 스크린샷](images/uploader-faq-img-03.png)

**14. 장면 파일을 호스팅해야 하나요?**
아니요, 파일을 업로드 한 후에는 Altspace에서 파일을 처리 합니다.

**15. 그림자가 허용 되나요?**
예

**16. 업 로더를 사용 하 여 얼마나 신속 하 게 반복할 수 있나요?**
이미 전 세계에 있는 경우 업 로더에서 업로드를 누르고 전 세계를 다시 설정 하 고 업데이트 된 장면을 10 초 내에 볼 수 있습니다. 일반적으로 장면의 복잡도에 따라 30 초의 루프가 몇 분에서 표시 됩니다. 음료를 보유 하 고 있습니다.

**17.3D 모델은 어디에서 얻을 까 요?**
Sketchfab, Sketchup, Minecraft, Unity Asset Store 등이 있습니다.

**18. 애니메이션이 지원 되나요?**

![사용자 지정 애니메이션을 실행 하는 GIF](images/uploader-faq-img-04.gif)

**19. 공간 오디오를 설정 하려면 어떻게 해야 하나요?** 선택한 wav 파일을 가져오고 장면에서 빈 게임 개체를 만든 다음이 개체를 선택 합니다. 가져온 소리를 개체의 검사기로 끌어 놓고 오디오 소스를 만듭니다. 그런 다음 볼륨을 0.5 미만으로 조정 하 고, 공간 blend를 3D로 변경 하 고, 최소 및 최대 거리를 조정 하 여 적절 한 소리 영역을 만듭니다. 이는 기본적으로 colliders와 같은 구로 표시 됩니다. True를 해제 하려면 드롭다운 곡선을 원하는 대로 조정 해야 합니다. [(via @IsThatToasted )](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20. eyed/weirdness를 어떻게 볼 까 요?**
업 로더가 렌더링 설정을 성공적으로 재정의 하지 않는 경우가 있습니다. "편집 > 프로젝트 설정 > 플레이어로 이동"으로 이동 합니다. PC와 Android 모두에 "XR 설정 > 가상 현실 지원 됨"이 선택 되어 있고 "스테레오 렌더링 방법"이 "단일 패스" 또는 "단일 패스 (미리 보기)" 인지 확인 합니다 (로봇 아이콘 선택). 이후에 빌드 + 업로드를 다시 하 고 전 세계를 다시 설정 합니다. 