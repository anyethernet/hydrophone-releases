# Hydrophone installer exit codes

Product: Hydrophone (하이드로폰) 1.0.0  
Installer: HydrophoneSetup.exe (Inno Setup 6)  
The package is a standalone offline installer. It does not download files during setup.

| Code | Meaning |
| --- | --- |
| 0 | Installation finished successfully. |
| 1 | Setup failed to initialize. |
| 2 | The user cancelled before installation started. |
| 3 | A fatal error occurred while preparing the installation. |
| 4 | A fatal error occurred during installation. Not enough disk space is reported with this code. There is no separate disk-full code. |
| 5 | The user cancelled during installation. |
| 7 | Setup determined that installation cannot proceed. |
| 8 | Setup cannot proceed until Windows is restarted. |

Any other non-zero code means the installation did not finish. The installer does not return a network-failure code, and it does not return a separate code when a device security policy blocks the package.

# 하이드로폰 설치 종료 코드

설치 파일은 단독 실행형이며, 설치 중에 다른 파일을 받지 않습니다.

| 코드 | 의미 |
| --- | --- |
| 0 | 설치가 끝났습니다. |
| 1 | 설치 프로그램을 시작하지 못했습니다. |
| 2 | 설치가 시작되기 전에 취소했습니다. |
| 3 | 설치를 준비하는 동안 치명적인 오류가 났습니다. |
| 4 | 설치 중에 치명적인 오류가 났습니다. 디스크 공간이 부족한 경우도 이 코드입니다. |
| 5 | 설치 중에 취소했습니다. |
| 7 | 설치를 진행할 수 없습니다. |
| 8 | Windows를 다시 시작한 뒤에야 설치를 진행할 수 있습니다. |

그 외 0이 아닌 코드는 설치가 끝나지 않은 것입니다. 네트워크 오류용 코드와, 보안 정책으로 패키지가 거부됐을 때의 별도 코드는 없습니다.
