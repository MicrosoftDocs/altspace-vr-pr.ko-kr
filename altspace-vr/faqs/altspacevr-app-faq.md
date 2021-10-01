---
title: AltspaceVR 앱에 대 한 질문과 대답
description: AltspaceVR 앱에 대 한 문제 해결 및 지원.
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr, AltspaceVR, 문제 해결, 지원
ms.openlocfilehash: a0df1e100ef8511fe3c9129548529577964c2336
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311898"
---
# <a name="frequently-asked-questions-about-the-altspacevr-app"></a>AltspaceVR 앱에 대 한 질문과 대답

## <a name="finding-the-altspacevr-app-version"></a>AltspaceVR app 버전 찾기

문제를 해결 하는 과정에서 현재 실행 중인 AltspaceVR 앱의 버전을 묻는 메시지가 표시 될 수 있습니다.

### <a name="in-altspacevr"></a>AltspaceVR에서

AltspaceVR에서 앱 버전을 찾으려면 **설정 메뉴로** 이동 하 여 왼쪽 탐색 모음에서 **정보** 를 선택 합니다. 아래 스크린샷에 표시 된 것 처럼 ' 앱 버전 '이 여기에 보고 됩니다.

![정보 패널 열기를 사용 하 여 설정 메뉴 열기](images/app-version-img-01.png)

### <a name="in-windows-system-settings"></a>Windows 시스템 설정

Microsoft Store을 통해 AltspaceVR를 설치한 경우 Windows 시스템 설정에서 앱 버전을 추가로 찾을 수 있습니다.  이 시나리오는 클라이언트에 성공적으로 로그인 할 수 없는 경우 앱 버전을 보고 하는 경우에 적합 합니다.

Windows 시스템 설정에서 앱 버전을 찾으려면 **시작 메뉴** 를 열고 **앱 & 기능** 을 입력 한 후 결과를 선택 합니다. 앱 목록에서 **AltspaceVR** 로 이동 합니다. AltspaceVR를 마우스 왼쪽 단추를 클릭 하 고 나타나는 메뉴에서 **고급 옵션** 을 선택 합니다.

![고급 옵션이 강조 표시 된 앱 및 기능 메뉴 열기](images/app-version-img-02.png)

**고급 옵션** 의 **사양** 헤더 아래에서 **응용 프로그램 버전이** **버전** 레이블 오른쪽에 나열 되어야 합니다.

![강조 표시 된 앱 버전으로 고급 옵션 열기](images/app-version-img-03.png)

### <a name="app-version-in-client-logs"></a>클라이언트 로그의 응용 프로그램 버전

AltspaceVR는 응용 프로그램 시작 중에 클라이언트 로그 파일의 앱 버전을 "Altspace Version"으로 보고 합니다. 이 옵션은 클라이언트에 성공적으로 로그인 할 수 없는 경우 앱 버전을 가져오는 것이 좋습니다. 그러나 실패 하기 전에 시작 하려고 했습니다.

### <a name="windows"></a>Windows

Windows에서 Windows 탐색기를 통해 클라이언트 로그 파일을 찾을 수 있습니다.

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

AltspaceVR를 시작할 때마다이 파일을 덮어씁니다. ' Player-prev '은 최신 세션을 나타내고 ' s s s. i n s. i n t '는 이전 세션을 나타냅니다.

### <a name="via-powershell"></a>PowerShell을 통해

고급 사용자는 다음과 같이 PowerShell을 통해이 문자열에 대 한 클라이언트 로그를 검색할 수 있습니다.

입력:

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

출력:

[2.047] AltspaceVR 버전: 3.2.23. e66c2

## <a name="how-do-i-upload-my-client-logs"></a>클라이언트 로그를 업로드 어떻게 할까요??

AltspaceVR client 응용 프로그램은 AltspaceVR를 사용 하는 동안 발생 하는 진단 데이터 및 이벤트 로그를 보관 합니다. 문제를 해결 하는 과정에서 팀에서 검토할 수 있도록 로그를 "업로드" 하 라는 메시지가 표시 될 수 있습니다. 이 기능을 사용 하 여 문제를 해결 하는 데 도움이 되도록 팀에 로컬 로그 콘텐츠를 보낼 수 있는 AltspaceVR의 기능입니다.

### <a name="in-altspacevr"></a>AltspaceVR에서

AltspaceVR에서 클라이언트 로그를 업로드 하려면 **설정 메뉴로** 이동 하 여 왼쪽 탐색 모음에서 **지원** 을 선택 합니다. 아래 스크린샷에 표시 된 것 처럼 로그를 업로드 하기 위한 몇 가지 옵션을 여기에서 사용할 수 있습니다.

![지원 패널 열기 및 로그 필드가 강조 표시 된 설정 메뉴](images/help-altvr-uploadlogs.png)

### <a name="fields"></a>필드

**"무엇이 문제 인가요?"**
발생 한 상황을 설명 합니다. 예를 들어, 버그를 발견 한 경우 실제로 발생 한 상황에 대비 하 여 예상 되는 결과를 설명 합니다. 이 정보는 업로드를 누를 때 로그와 함께 전송 됩니다.

**"업로드 로그"** 이 단추는 현재 세션에서 로그를 업로드 합니다. 이 세션에서 문제가 발생 하는 경우 (예: AltspaceVR client를 닫지 않은 경우)이 옵션을 사용 하 고 보고 하려는 경우에이 옵션을 사용 합니다.

**"마지막 로그 업로드"** 이 단추는 이전 세션에서 로그를 업로드 합니다.

**"마지막 크래시 로그 업로드"** 이 단추를 클릭 하면 발생 한 최신 크래시에서 더 많은 로그 콘텐츠가 업로드 됩니다.

### <a name="in-client-logs"></a>클라이언트 로그

컴퓨터에서 로그 파일을 검색할 수도 있습니다. 이러한 로그를 검색 하는 방법에 대 한 지침은 [여기](#app-version-in-client-logs)에서 찾을 수 있습니다.


이러한 파일을 찾았으면 제출을 클릭 하기 전에 [지원 티켓을 열고](https://help.altvr.com/hc/en-us/requests/new) 티켓 요청에 로그를 업로드 합니다.

## <a name="what-do-i-do-if-i-cant-launch-altspacevr"></a>AltspaceVR를 시작할 수 없는 경우 수행할 작업

AltspaceVR가 시작 되지 않는 이유는 여러 가지가 있습니다. 다음 단계를 수행 하 여 필요한 타사 소프트웨어와 함께 응용 프로그램이 올바르게 설치 되었는지 확인 합니다.

### <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>처음으로 AltspaceVR를 시작 하려는 경우:

1. 장치가 지원 되며 [지정 된 최소 요구 사항을](../getting-started/system-requirements.md)충족 하는지 확인 합니다.
2. 최신 [Oculus 소프트웨어가](https://www.oculus.com/setup) 설치 되어 있는지 확인 하 고, 설정 > 일반-> 알 수 없는 장치를 ON으로 설정 합니다. 2D 모드로 시작 하는 경우에는 Oculus를 설치할 필요가 없습니다.
3. 인터넷 연결이 작동 하는지 확인 합니다. 네트워크 방화벽 내에서 Altspace를 시작 하려는 경우 UDP 포트 5055 및 5056 및 TCP 포트 80 및 443을 엽니다. 회사 또는 교육용 방화벽의 네트워크 내에 있는 경우 네트워크 관리자 또는 IT 부서에 문의 해야 할 수 있습니다.
4. 참고 항목:
    * [Oculus Quest 용 AltspaceVR 설치](../getting-started/oculus-installation.md)
    * [Windows Mixed Reality에 대 한 AltspaceVR 설치](../getting-started/wmr-installation.md)

### <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>AltspaceVR에서 현재 버전이 최신 버전이 아닌 것으로 보고 되는 경우:

* 사용 중인 응용 프로그램의 버전이 더 이상 지원 되지 않습니다. Storefront을 통해 AltspaceVR를 다운로드 한 경우 스토어에서 클라이언트를 업데이트 하기 전에 업데이트를 최근에 실행 했을 수 있습니다.
* 강제로 업데이트 하려면 다양 한 상점를 통해 수행할 수 있습니다.
    * **Microsoft Store:** [Microsoft Store 지원-Microsoft Store에서 앱 및 게임 업데이트 받기](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus:** Oculus 라이브러리를 열고 왼쪽 탐색 모음에서 ' 업데이트 '로 이동 합니다.
    * **스트림:** [스트림 Support-Update & 설치 문제](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

### <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>프로그램이 작동 중이 고 업데이트 후 시작 되지 않는 경우:

* 소프트웨어의 ' 치료 다시 설치 '를 수행 합니다. 이렇게 하려면 응용 프로그램의 기존 버전을 제거 하거나 제거 해야 합니다. 시스템에서 완전히 제거 되 면 스트림, Oculus 또는 Microsoft Store를 통해 Altspace를 설치 합니다.
* AltspaceVR을 시작 하는 데 문제가 있는 경우 [지원 티켓](https://help.altvr.com/hc/requests/new)을 통해 알려주세요. 세션의 [로그 파일](altspacevr-app-faq.md#how-do-i-upload-my-client-logs) 을 포함 합니다.

### <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>홈 공간을 사용자 지정한 후 AltspaceVR가 시작 되지 않는 경우:

* [홈 공간의 웹 사이트로](https://account.altvr.com/users/sign_in)이동 합니다.
* 세계 템플릿이 여전히 존재 하는지 확인 합니다. 템플릿을 사용자와 공유 하는 경우 소유자가 삭제 했을 수 있습니다. 그러면 홈 공간이 로드 되지 않습니다.
    * 템플릿이 삭제 된 경우 왼쪽 ' 세계 도구 ' 패널에서 세계를 ' 편집 ' 하 고 기존 템플릿을 다른 템플릿으로 바꾸고 ' 업데이트 '를 사용 하 여 변경 내용을 저장 하면 됩니다.
* 왼쪽 ' 세계 도구 ' 패널에서 ' 개체 '를 선택 하 여 로드 하지 못할 수 있는 개체를 모두 제거 합니다. 문제가 있는 개체는 다음과 같습니다.
    * 아직 전 세계에 있는 삭제 된 키트의 개체 또는 키트에서 삭제 된 개체입니다.
    * 실험적 인 Tfs입니다.
* 위의 항목을 해결 한 후 AltspaceVR를 다시 입력 해 봅니다.

Azure IP 범위 및 서비스 태그를 비롯 한 네트워크 관리자 또는 IT 부서에 대 한 고급 지원은 [다운로드 세부 정보](https://www.microsoft.com/en-us/download/details.aspx?id=56519)에서 찾을 수 있습니다.

## <a name="support"></a>Support(지원)

AltspaceVR 팀에 대 한 질문이 나 피드백이 있나요? 

> [!div class="nextstepaction"]
> [지원 요청을 보내려면 여기를 클릭 하십시오.](https://help.altvr.com/hc/requests/new)