# 그누보드 알림 플러그인

# Table Of Contents

1. [요약](#1-요약)
2. [요구사항](#2-요구사항)
3. [설치](#3-설치)
4. [벤더 설정](#4-벤더-설정)
5. [관리자 벤더설정](#5-관리자-벤더설정)
6. [관리자 설정에 의한 앱 동작 확인](#6-관리자-설정에-의한-앱-동작-확인)
7. [관리자 전송내역](#7-관리자-전송내역)
8. [참고](#8-참고)

# 1. 요약

-   미리 작성된 Hook 기반 이벤트에 등록된 알림을 전송합니다.
-   그누보드 코어파일 수정없이 동작합니다.
-   미리 준비된 메시지 템플릿 이외에도 필요한 곳에서는 직접 알림 함수를 사용하여 메시지를 확장할 수 있습니다.
-   utf-8 환경에서 안정적으로 동작합니다.
-   PHP 5.5.0 버전 이상 필요합니다.
-   그누보드 5.4.0.2 버전 이상 필요합니다.

# 2. 요구사항

-   php >= 5.5.0
-   php cURL 라이브러리 사용 가능 환경
-   gnuboard >= 5.4.0.2

# 3. 설치

-   압축 해제후 그누보드-설치폴더 에 그대로 업로드
    -   그누보드-설치폴더/extend
    -   그누보드-설치폴더/plugin

# 4. 벤더 설정

## 4-1. Slack API

-   [Slack API 설정 ![](resources/images/00-common/Icon_External_Link_12x12.png)](README-slack-api.md)
-   관리자 벤더설정을 위해 필요한 값
    -   `token` : _Bot User OAuth Token_
    -   `target` : _UserID (DM)_ or _ChannelID (그룹전송)_

# 5. 관리자 벤더설정

플러그인 설치/재설치 후 관리자 초기화면

![](resources/images/06-gnuboard-adm-config/gnuboard-adm-conf-01.jpg)

`token` (_Bot User OAuth Token_), `target` (_UserID_) 설정 및 사용설정

![](resources/images/06-gnuboard-adm-config/gnuboard-adm-conf-02.jpg)

Hook 템플릿 중 일부 사용설정

![](resources/images/06-gnuboard-adm-config/gnuboard-adm-conf-03.jpg)
![](resources/images/06-gnuboard-adm-config/gnuboard-adm-conf-04.jpg)

# 6. 관리자 설정에 의한 앱 동작 확인

![](resources/images/07-device-notification/IMG_0133.PNG)
![](resources/images/07-device-notification/IMG_0134.PNG)
![](resources/images/07-device-notification/IMG_0135.PNG)

# 7. 관리자 전송내역

![](resources/images/06-gnuboard-adm-config/gnuboard-adm-conf-05.jpg)

# 8. 참고

-   소프트웨어 특성상 구매 후 환불은 불가능 합니다.
-   이 기능은 그누보드의 버전에 따라 사용 가능한지 여부가 달라집니다. 최신 버전의 문서 또는 공식 리소스를 참고하여 버전에 맞는 정보를 확인하세요.
-   이 플러그인은 상용 라이선스로 제공되며, 저작자의 동의 없이 무단 복제, 배포, 전송, 기타 침해 행위를 거부하며, 발견 시 관련 법에 의해 처벌될 수 있습니다.  
    또한, 본 플러그인은 일부 난독화가 적용되어 있어 이를 무단으로 해제하거나 리버스 엔지니어링을 통한 저작물 변조 등의 행위를 허용하지 않습니다.  
    이와 같은 행위는 저작물의 보호를 위해 엄격히 금지되며, 위반 시 법적 조치가 취해질 수 있습니다.  
    난독화가 적용되지 않은 버전의 구매를 희망하는 경우 별도 문의바랍니다.
