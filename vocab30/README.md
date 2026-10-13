# 영단어 30일

A1~C2 영단어 9,680개를 레벨별 30일 진도표와 스와이프 카드로 외우는 단어장 웹앱입니다.
한국어 뜻, 영어 정의, 예문, 자연 음성 발음이 들어 있고, 아이폰·안드로이드 홈 화면에 추가하면 앱처럼 동작합니다.

## GitHub Pages로 올리기

1. GitHub에서 새 저장소(Repository)를 만듭니다. 예: `vocab30` (Public)
2. 이 폴더의 파일을 **폴더 구조 그대로** 올립니다.
   - `index.html`, `manifest.webmanifest`, `sw.js`, `README.md`
   - `audio/` 폴더 (audio-A1.json ~ audio-C2.json)
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

## 안드로이드에서 쓰기

두 가지 방법 중 편한 것을 고르면 됩니다.

**방법 1. 크롬에서 바로 설치 (가장 간단)**
1. 안드로이드 크롬에서 https://gutereise01.github.io/nihongo/vocab30/ 를 엽니다.
2. 화면 위의 **앱 설치** 버튼을 누르거나, 크롬 메뉴(⋮) → **앱 설치** / **홈 화면에 추가**를 누릅니다.
3. 앱 목록의 "영단어30일" 아이콘으로 실행합니다. 업데이트는 자동으로 반영됩니다.

**방법 2. 설치 파일(APK)로 설치**
1. 휴대폰에서 https://github.com/gutereise01/nihongo/releases/download/vocab30-android/vocab30.apk 를 내려받습니다.
2. 내려받은 파일을 열고, 처음이라면 "출처를 알 수 없는 앱 설치"를 허용합니다.
3. 음성·단어가 모두 앱 안에 들어 있어 인터넷 없이 바로 쓸 수 있습니다.
   새 버전이 나오면 같은 주소에서 다시 받아 설치하면 진도 기록은 그대로 유지됩니다.

APK는 이 저장소의 GitHub Actions(`.github/workflows/vocab30-android.yml`)가 `vocab30/` 폴더가 바뀔 때마다 자동으로 만들어 Releases에 올립니다.

## 참고

- 진도 기록은 각자의 기기(브라우저)에 저장됩니다.
- 단어 출처: A1~C1은 Langeek CEFR 단어 목록, C2는 [Octanove Vocabulary Profile C1/C2](https://github.com/openlanguageprofiles/olp-en-cefrj) (Octanove Labs, CC BY-SA 4.0)에서 A1~C1과 겹치지 않는 C2 단어 936개를 골랐습니다. 한국어 뜻·예문과 C2 영어 정의는 별도로 작성했습니다.
- 발음은 Kokoro 신경망 음성(af_heart)으로 미리 녹음했습니다.
- 앱을 수정한 뒤 다시 올릴 때는 `sw.js`의 `CACHE` 이름(예: `vocab30-v2`)도 바꿔야 설치된 앱에 새 버전이 반영됩니다.
