# SABLE device modules

This repository hosts the signed device modules that the SABLE app downloads for the devices connected to a PC. The app's source code is not published here.

- The release [`modules`](https://github.com/IHATECODING-lab/SABLE/releases/tag/modules) holds `index.json` (the module list), its signature `index.sig`, and the files of each module version.
- Every list, manifest and model pack is signed with an ECDSA P-256 key pinned in the app (`sable-modules-1`). A manifest fixes its executable's exact size and SHA-256.
- The app installs a module only after these checks pass. It sends no device information: it downloads the whole list and compares it with the connected devices on the PC.

---

SABLE가 PC에 연결된 장치에 맞춰 내려받는 서명된 장치 모듈을 올려 두는 저장소입니다. 앱 소스 코드는 올리지 않습니다.

- Release `modules`에는 모듈 목록 `index.json`과 서명 `index.sig`, 모듈 버전별 파일이 있습니다.
- 목록과 매니페스트는 앱에 고정된 ECDSA P-256 키(`sable-modules-1`)로 서명합니다. 매니페스트에는 실행 파일의 정확한 크기와 SHA-256이 적혀 있습니다.
- 앱은 서명과 해시 검사를 통과한 모듈만 설치합니다. 장치 정보는 보내지 않습니다.
