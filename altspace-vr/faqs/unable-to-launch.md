---
title: AltspaceVR을 시작할 수 없습니다.
description: AltspaceVR 환경 시작과 관련된 문제를 식별, 보고 및 해결하는 방법을 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 자주 묻는 질문(FAQ)
ms.openlocfilehash: 50edddef669aca14640fd6e910c12c15864cf46a099e54bceed40494e9817de4
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127932"
---
# <a name="i-cant-launch-altspacevr"></a>AltspaceVR을 시작할 수 없습니다.

AltspaceVR이 시작되지 않을 수 있는 몇 가지 이유가 있습니다. 다음 단계를 시도하여 필요한 타사 소프트웨어와 함께 애플리케이션이 올바르게 설치되었는지 확인합니다.

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>처음으로 AltspaceVR을 시작하려는 경우:

1. 디바이스가 지원되고 지정된 최소 요구 사항 을 충족하는지 [확인합니다.](../getting-started/system-requirements.md)
2. 최신 [Oculus Software가](https://www.oculus.com/setup) 설치되어 있고 설정 > 일반 > 알 수 없는 디바이스가 ON으로 설정되어 있는지 확인합니다. 2D 모드로 시작하는 경우 Oculus를 설치할 필요가 없습니다.
3. 작동하는 인터넷 연결이 있는지 확인합니다. 네트워크 방화벽 내에서 Altspace를 시작하려는 경우 UDP 포트 5055 및 5056과 TCP 포트 80 및 443을 엽니다. 회사 또는 교육용 방화벽의 네트워크 내에 있는 경우 네트워크 관리자 또는 IT 부서에 문의해야 할 수 있습니다.
4. 참고 항목:
    * [Oculus Quest용 AltspaceVR 설치](../getting-started/oculus-installation.md)
    * [Windows Mixed Reality 대한 AltspaceVR 설치](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>AltspaceVR에서 현재 버전이 만료되었다고 보고하는 경우:

* 사용 중인 애플리케이션의 버전은 더 이상 지원되지 않습니다. 상점을 통해 AltspaceVR을 다운로드한 경우 스토어에서 클라이언트를 업데이트하기 전에 최근에 업데이트가 시작되었을 수 있습니다.
* 업데이트를 강제로 수행하려는 경우 다양한 상점을 통해 업데이트할 수 있습니다.
    * **Microsoft Store:** Microsoft Store 지원 - Microsoft Store [앱 및 게임에 대한 업데이트 받기](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **오실러스:** Oculus 라이브러리를 열고 왼쪽 탐색 모음에서 '업데이트'로 이동합니다.
    * **Steam:** [Steam 지원 - & 설치 문제 업데이트](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>프로그램이 작동 중이지만 업데이트 후 시작이 중단된 경우:

* 소프트웨어의 '정리 다시 설치'를 수행합니다. 이렇게 하려면 기존 버전의 애플리케이션을 제거하거나 제거해야 합니다. 시스템에서 완전히 제거되면 Steam, Oculus 또는 Microsoft Store 통해 Altspace를 설치합니다.
* AltspaceVR을 시작하는 데 문제가 있는 경우 [지원 티켓을](https://help.altvr.com/hc/requests/new)통해 알려주세요. 세션에서 [로그 파일을](uploading-client-logs.md) 포함합니다.

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>홈 공간을 사용자 지정한 후 AltspaceVR이 시작되지 않는 경우:

* [홈 공간의 웹 사이트](https://account.altvr.com/users/sign_in)로 이동합니다.
* 세계의 템플릿이 여전히 존재하는지 확인합니다. 템플릿이 사용자와 공유된 경우 소유자가 템플릿을 삭제했을 수 있으며 이로 인해 홈 공간이 로드되지 않을 수 있습니다.
    * 템플릿이 삭제된 경우 왼쪽 'World Tools' 패널에서 전 세계를 '편집'하고, 기존 템플릿을 다른 템플릿으로 바꾸고, '업데이트'를 사용하여 변경 내용을 저장합니다.
* 왼쪽 'World Tools' 패널에서 '개체'를 선택하여 로드에 실패할 수 있는 개체를 제거합니다. 문제가 있는 개체에는 다음이 포함될 수 있습니다.
    * 삭제된 키트의 개체 또는 키트에서 삭제된 개체는 여전히 전 세계에 존재합니다.
    * 실험적 GLTF.
* 위의 항목의 주소를 지정한 후 AltspaceVR을 다시 입력합니다.

Azure IP 범위 및 서비스 태그를 포함하여 네트워크 관리자 또는 IT 부서에 대한 고급 지원은 [다운로드 세부 정보](https://www.microsoft.com/en-us/download/details.aspx?id=56519)에서 찾을 수 있습니다.