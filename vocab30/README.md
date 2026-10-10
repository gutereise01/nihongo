# 영단어 30일

A1·A2·B1·B2 영단어 6,263개를 레벨별 30일 진도표와 스와이프 카드로 외우는 단어장 웹앱입니다.
한국어 뜻, 영어 정의, 예문, 자연 음성 발음이 들어 있고, 아이폰 홈 화면에 추가하면 앱처럼 동작합니다.

## GitHub Pages로 올리기

1. GitHub에서 새 저장소(Repository)를 만듭니다. 예: `vocab30` (Public)
2. 이 폴더의 파일을 **폴더 구조 그대로** 올립니다.
   - `index.html`, `manifest.webmanifest`, `sw.js`, `README.md`
   - `audio/` 폴더 (audio-A1.json ~ audio-B2.json)
   - `icons/` 폴더 (아이콘 4개)
3. 저장소의 **Settings → Pages**에서
   - Source: **Deploy from a branch**
   - Branch: **main** / 폴더 **/(root)** → Save
4. 1~2분 뒤 `https://<GitHub아이디>.github.io/vocab30/` (이 저장소처럼 다른 저장소의 하위 폴더에 두면 `https://<아이디>.github.io/<저장소>/vocab30/`) 주소로 열립니다.

## 아이폰에 앱처럼 설치하기

1. 사파리에서 위 주소를 엽니다.
2. 공유 버튼 → **홈 화면에 추가**
3. 홈 화면의 "영단어30일" 아이콘으로 실행하면 주소창 없이 전체 화면으로 열립니다.
   한 번 열어 두면 인터넷이 없어도 공부할 수 있습니다.

## 참고

- 진도 기록은 각자의 기기(브라우저)에 저장됩니다.
- 단어 출처: Langeek CEFR A1·A2·B1·B2 단어 목록. 한국어 뜻과 예문은 별도로 작성했습니다.
- 발음은 Piper 신경망 음성(en-US lessac)으로 미리 녹음했습니다.
- 앱을 수정한 뒤 다시 올릴 때는 `sw.js`의 `CACHE` 이름(예: `vocab30-v2`)도 바꿔야 설치된 앱에 새 버전이 반영됩니다.
