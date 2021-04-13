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
# <a name="uploading-custom-skyboxes"></a>사용자 지정 Skyboxes 업로드

Skybox 환경을 더 몰입로 만드는 세계에 대 한 **배경을** 만드는 방법입니다. 다양 한 종류의 Skyboxes 있지만 현재는 **등 장방형** 를 지원 합니다. 다음은 360 카메라를 사용 하는 예제입니다 (추가 예제 [참조).](http://moments.mankindforward.com/) 

![등 장방형 실내의 360 보기](images/custom-skyboxes-img-01.jpeg)

[Unity 업 로더](world-building-toolkit-getting-started.md) 를 사용할 수도 있지만이 방법은 더 간단 합니다.

1. [> Skyboxes](https://account.altvr.com/skyboxes) 로 이동 하 여 오른쪽에 있는 **만들기** 단추를 누릅니다.

![Skyboxes 패널에 연결 되는 웹 사이트 페이지](images/custom-skyboxes-img-02.png)

2. 이름을 입력 하 고 360 이미지를 지정 합니다. 사진이 될 필요는 없으며, 사용자가 직접 그리거나 온라인으로 검색할 수 있는 프로그램이 있습니다. 준비가 되면 **만들기** 를 선택합니다. 

![Skybox 만들기 양식](images/custom-skyboxes-img-03.png)

3. 이 skybox 쉽게 식별할 수 있도록 **미리 보기** 이미지를 선택적으로 업로드할 수 있습니다. WAV 형식의 주변 오디오를 업로드할 수도 있습니다. 

> [!IMPORTANT]
> 360 이미지를 업로드 한 후 미리 보기 이미지와 주변 오디오를 별도로 업로드 하는 것이 좋습니다. 이러한 파일을 업로드 하는 경우 파일 크기는 프로세스를 정지 하기에 충분히 커질 수 있습니다. [Jetsons 세계](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) 는 주변 오디오와 함께 Skybox를 사용 하는 방법의 좋은 예입니다. 세계 빌더가 오디오 볼륨 부족 및 들리는 소리를 유지 하는 방법을 확인 하는 것은 표정이. 

4. 전 세계를 입력 하 고 전 세계 편집기를 여세요. Skyboxes에서 새 Skybox를 선택 합니다. 몇 초 후에는 하늘이 변경 됩니다. 전 세계의 다른 사람들이 공중 변화를 볼 수도 있습니다. 다시 전환 하려면 동일한 목록에서 **기본** skybox를 선택 합니다. 

## <a name="troubleshooting"></a>문제 해결

**하늘:-(에는 조인트 또는 선이 있습니다.** 곧 해결할 버그입니다.

**업로드 실패**
    * 360 이미지만 업로드 해 보세요.
    * 다른 작은 파일을 테스트로 사용해 보세요.

**360 사진을 찾을 수 없습니다.**
    * Flickr가 좋은 원본 (창의적인 commons 항목을 찾기 위해 필터 변경)
    * 사용자 고유의 참여! Ricoh의 카메라에 성공 했습니다. 
**하늘 모양이 거칠게 표시 되거나 blocky** 고해상도 이미지를 찾아야 할 수도 있습니다. 일반적으로 2-5 m b 및 ~ 5000 px x 2000 px

**세계의 프레임 속도가 아파!**
이미지가 너무 클 수 있습니다. 일부 생성 된 skyboxes은 8k 일 수 있습니다. 일반적으로는이를 사용 합니다.

**주변 오디오에 대 한 도움말**
    * Audacity와 같은 무료 소프트웨어를 사용 하 여 볼륨을 낮추고 사용자 고유의 루프를 만듭니다. 오디오가 반복 되 고 사용자의 귀를 재생 하는 것을 기억 하세요.
    * [무료 소리](https://freesound.org/) 는 로열티 없는 소리의 좋은 원본입니다.
