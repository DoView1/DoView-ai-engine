# DoView AI Engine

## 처음 사용하는 분께 — Windows 1.2.12

DoView의 AI 번역을 처음 사용할 때 한 번 내려받는 선택 기능입니다. 이미지와 문서를 보기만 한다면 엔진을 설치하지 않아도 됩니다. **API 키나 별도 Python 설치는 필요하지 않습니다.**

1. [DoView Windows 1.2.12](https://github.com/DoView1/DoView-release/releases/tag/v1.2.12)를 설치하고 번역할 이미지나 문서를 엽니다.
2. **번역**을 누르면 AI 엔진 설치 화면이 열립니다. [구성 요소 이용 조건](TERMS.md)을 확인한 뒤 **엔진 다운로드**를 누르세요. 버튼을 누르기 전에는 엔진 다운로드가 시작되지 않습니다.
3. 다운로드와 파일 검증이 끝날 때까지 같은 문서·페이지에서 기다리세요. 문서나 번역 설정을 바꾸지 않았다면 설치 화면이 닫히고 요청한 번역이 이어서 시작됩니다.

다운로드 크기는 약 **11.3GB**이며, 새 설치에는 최소 **11.57GB**의 여유 공간이 필요합니다. 설치한 엔진은 이후 번역·글자 인식(OCR)·요약·질문에 다시 사용합니다. 설정에서 직접 설치하려면 **설정 → AI → 엔진 다운로드**를 누르세요.

### 다운로드를 멈췄다면

다운로드를 취소하거나 앱을 다시 실행해도 이미 받은 파일은 유지됩니다. 같은 앱에서 **엔진 다운로드** 또는 **다운로드 이어받기**를 누르면 받은 파일을 확인한 뒤 남은 부분을 이어받습니다. 이어받기 전 파일 확인 중에는 잠시 진행률 대신 검증 상태가 표시될 수 있습니다.

설정 화면을 닫으면 요청한 번역의 자동 재개가 취소됩니다. **다운로드 자체를 멈추려면 다운로드 진행 중의 취소 버튼을 누르세요.** 설치가 끝난 뒤 번역을 다시 눌러도 됩니다.

### 사용 환경과 이용 조건

이 패키지는 **Windows x64**용입니다. 설치 후 번역은 사용자의 컴퓨터에서 처리합니다. 엔진 다운로드와 뷰어 업데이트 확인에는 인터넷 연결이 필요합니다. 처리 속도와 GPU 사용 가능 여부는 기기·드라이버·다른 프로그램의 자원 사용량에 따라 달라지며, 모든 기기나 일정한 처리 시간을 보장하지 않습니다. 자원 보호와 파일 검증은 계속 적용됩니다.

이미지 번역의 우선 대상은 말풍선 안의 대사입니다. OCR과 번역 결과에는 오류가 있을 수 있으므로 저장하기 전에 확인하세요. DoView 1.2.11의 다운로드 버튼은 이 파일 공개만으로 활성화되지 않으므로 **1.2.12로 업데이트**해 주세요.

다운로드를 선택하면 [구성 요소 고지와 해당 NVIDIA 이용 조건](TERMS.md)에 동의하게 됩니다. 각 구성 요소에는 해당 라이선스가 적용됩니다. 아래의 기존 영문 안내와 [이용 조건](TERMS.md), [OCR 대응 소스 안내](SOURCES.md)를 함께 확인하세요.

## English

Optional local AI engine files for [DoView](https://github.com/DoView1/DoView-release).
Use the viewer's **Settings → AI → Download and install** control in a version
whose download button is enabled. The viewer downloads and checks the compatible
package before activating it. You do not need a separate Python installation.

DoView 1.2.11 predates public engine download configuration and only imports a
prepared engine folder. Install the viewer update that advertises engine download
support; uploading files here does not activate the old application's button.

The engine installs once and is reused for local translation, OCR, summaries and
questions. Viewing images and documents does not require it. This repository is
for engine distribution documents and component/source assets, not the whole
viewer source repository.

- [Download/component terms](TERMS.md)
- [Corresponding source and modification](SOURCES.md)
- [Release assets](https://github.com/DoView1/DoView-ai-engine/releases)

The engine includes its component notices and immutable file hashes. NVIDIA
libraries, models, GEOS and fonts retain their own licenses. The OCR corresponding
source archive is available alongside the engine assets. No usage telemetry or
account registration is added by this engine distribution.
