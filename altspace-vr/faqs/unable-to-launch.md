---
title: AltspaceVR를 시작할 수 없습니다.
description: AltspaceVR 환경을 시작 하는 것과 관련 된 문제를 식별 하 고 보고 하 고 수정 하는 방법을 알아봅니다.
ms.date: 02/10/2021
ms.topic: article
keywords: 자주 묻는 질문(FAQ)
ms.openlocfilehash: fc49b5b7ed708e43a12616d782a397a364b2264e
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213134"
---
# <a name="i-cant-launch-altspacevr"></a>AltspaceVR를 시작할 수 없습니다.

AltspaceVR가 시작 되지 않는 이유는 여러 가지가 있습니다. 다음 단계를 수행 하 여 필요한 타사 소프트웨어와 함께 응용 프로그램이 올바르게 설치 되었는지 확인 합니다.

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>처음으로 AltspaceVR를 시작 하려는 경우:

1. 장치가 지원 되며 [지정 된 최소 요구 사항을](../getting-started/system-requirements.md)충족 하는지 확인 합니다.
2. 최신 [Oculus 소프트웨어가](https://www.oculus.com/setup) 설치 되어 있는지 확인 하 고, 설정-> 일반-알 수 없는 장치 > 설정 됨으로 설정 되어 있는지 확인 합니다. 2D 모드로 시작 하는 경우에는 Oculus를 설치할 필요가 없습니다.
3. 인터넷 연결이 작동 하는지 확인 합니다. 네트워크 방화벽 내에서 Altspace를 시작 하려는 경우 UDP 포트 5055 및 5056 및 TCP 포트 80 및 443을 엽니다. 회사 또는 교육용 방화벽의 네트워크 내에 있는 경우 네트워크 관리자 또는 IT 부서에 문의 해야 할 수 있습니다.
4. 참고 항목:
    * [Oculus Quest 용 AltspaceVR 설치](../getting-started/oculus-installation.md)
    * [Windows Mixed Reality 용 AltspaceVR 설치](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>AltspaceVR에서 현재 버전이 최신 버전이 아닌 것으로 보고 되는 경우:

* 사용 중인 응용 프로그램의 버전이 더 이상 지원 되지 않습니다. Storefront을 통해 AltspaceVR를 다운로드 한 경우 스토어에서 클라이언트를 업데이트 하기 전에 업데이트를 최근에 실행 했을 수 있습니다.
* 강제로 업데이트 하려면 다양 한 상점를 통해 수행할 수 있습니다.
    * **Microsoft Store:** [Microsoft Store 지원-Microsoft Store에서 앱 및 게임 업데이트 받기](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus:** Oculus 라이브러리를 열고 왼쪽 탐색 모음에서 ' 업데이트 '로 이동 합니다.
    * **스트림:** [스트림 Support-Update & 설치 문제](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>프로그램이 작동 중이 고 업데이트 후 시작 되지 않는 경우:

* 소프트웨어의 ' 치료 다시 설치 '를 수행 합니다. 이렇게 하려면 응용 프로그램의 기존 버전을 제거 하거나 제거 해야 합니다. 시스템에서 완전히 제거 되 면 스트림, Oculus 또는 Microsoft Store를 통해 Altspace를 설치 합니다.
* AltspaceVR을 시작 하는 데 문제가 있는 경우 [지원 티켓](https://help.altvr.com/hc/requests/new)을 통해 알려주세요. 세션의 [로그 파일](uploading-client-logs.md) 을 포함 합니다.

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>홈 공간을 사용자 지정한 후 AltspaceVR가 시작 되지 않는 경우:

* [홈 공간의 웹 사이트로](https://account.altvr.com/users/sign_in)이동 합니다.
* 세계 템플릿이 여전히 존재 하는지 확인 합니다. 템플릿을 사용자와 공유 하는 경우 소유자가 삭제 했을 수 있습니다. 그러면 홈 공간이 로드 되지 않습니다.
    * 템플릿이 삭제 된 경우 왼쪽 ' 세계 도구 ' 패널에서 세계를 ' 편집 ' 하 고 기존 템플릿을 다른 템플릿으로 바꾸고 ' 업데이트 '를 사용 하 여 변경 내용을 저장 하면 됩니다.
* 왼쪽 ' 세계 도구 ' 패널에서 ' 개체 '를 선택 하 여 로드 하지 못할 수 있는 개체를 모두 제거 합니다. 문제가 있는 개체는 다음과 같습니다.
    * 아직 전 세계에 있는 삭제 된 키트의 개체 또는 키트에서 삭제 된 개체입니다.
    * 실험적 인 Tfs입니다.
* 위의 항목을 해결 한 후 AltspaceVR를 다시 입력 해 봅니다.

Azure IP 범위 및 서비스 태그를 비롯 한 네트워크 관리자 또는 IT 부서에 대 한 고급 지원은 [다운로드 세부 정보](https://www.microsoft.com/en-us/download/details.aspx?id=56519)에서 찾을 수 있습니다.