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
# <a name="importing-gltf-models"></a>인 글 Tf 모델 가져오기

> [!NOTE]
> 이 기능은 초기 액세스 프로그램에서 선택한 사용자에 게 제공 됩니다.

3D 모델 및 장면을 Altspace으로 가져오는 한 가지 방법은 [글 tf 표준](https://en.wikipedia.org/wiki/GlTF)을 사용 하는 것입니다. 나중에 세계 편집기에서 생성할 수 있는 모델을 만들기 위해 .bb 파일 (압축 된 고 지 수)을 업로드할 수 있습니다. 사용자 [고유의 키트를 업로드](uploading-custom-kits.md)하는 대신 사용할 수 있습니다. 성능 및 재사용을 최대화 하려는 경우 Unity 및 키트를 사용할 필요가 없기 때문에 신속한 데모를 위한 모델을 만드는 것이 좋습니다. 

1. 몇 가지 유용한 3D 자산을 찾습니다. 검색할 한 곳은 Sketchfab (예: **다운로드 가능한** 모델에 대해 필터링 [시도).](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models) 찾은 후 **3D 모델 다운로드** 를 선택 합니다.

![Sketchfab의 3D 강아지 모델](images/importing-models-img-01.png)

2. 모델에 대 한 링크를 복사 하 고 라이선스 요구 사항을 읽습니다. 
3. **자동 변환 된 형식 (글 tf)** 버전 다운로드

![자동 변환 된 서식을 사용 하는 Sketchfab 다운로드 옵션 강조 표시](images/importing-models-img-02.png)

4. 인 사이트를 열고 **PNG를 JPEG (베타)로 변환** 상자를 [선택 합니다.](https://glb-packer.glitch.me)
5. 다운로드 한 글 어 파일의 압축을 풀고 모든 항목을 한 번에 한 번에 끌어서 브라우저 탭으로 끌어서 놓습니다.

![모델 압축 해제를 표시 하는 창](images/importing-models-img-03.png)

6. 파일의 수와 크기에 따라 처리 하는 데 시간이 걸릴 수 있습니다. 처리가 완료 되 면 **출력** 파일이 다운로드 됩니다. 해당 파일의 이름을 정보로 바꿉니다 .이는 세계의 개체 이름입니다 (예: **Low Poly).**
7. [Altvr.com > 더 많은 > 모델로](https://account.altvr.com/users/sign_in) 이동 하 고 **만들기** 를 선택 합니다.
8. .Bb 파일의 위치를 지정 하 고 Sketchfab 링크를 특성의 설명에 복사 해야 합니다. 원하는 경우 미리 보기 이미지를 지정 하 고 **모델 만들기** 를 선택할 수 있습니다.

![AltspaceVR의 모델 미리 보기](images/importing-models-img-04.png)

9. **클립보드로 복사를 선택 합니다** .
10. **세계 편집기 > Altspace > 기본 사항 >** 공개 합니다.
11. Url에 붙여 넣고 **확인** 을 선택 합니다.

축하합니다! 방금 첫 번째 모델을 생성 했습니다.

## <a name="troubleshooting"></a>문제 해결

**클릭 한 내용이 **없는지 확인** 합니다.**
    * 현재는 100,000 개의 다각형 한도가 있습니다. 실패 한 경우 개체를 삭제 하 여 전 세계에 참가 하는 사용자의 잠재적인 문제를 방지 합니다.
    * 자산에 다른 문제가 있을 수 있습니다. 가능한 한 적은 수의 다각형이 포함 된 자산을 사용 하려고 합니다.
    * 가져오는 모델이 작거나 클 수 있습니다. 규모를 늘리거나 줄여 보거나 아바타를 이동 해 보세요. 모델 내부에 있을 수 있습니다.

**로드 속도가 느립니다** . 전 세계의 다른 사용자가이를 로드 하는 속도는 연결 속도에 따라 달라 집니다. 또한 키트 자산과 마찬가지로 캐시 되지 않습니다. 홈에 저장 한 경우에는 조인할 때마다 동일한 모델을 다시 다운로드 하는 것이 좋습니다.

**충돌이 발생 하지 않습니다** . 기본적으로 이러한 방식으로 가져오는 개체에는 충돌이 발생 하지 않습니다.

**이를 생성 하면 6 개의 DOF에서 컨트롤이 손실 되거나 내부에 있으므로 조작 하기 어렵습니다** . 예, 이러한 문제를 알고 있으며 곧 해결할 것입니다.  