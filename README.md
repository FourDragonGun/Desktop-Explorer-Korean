# Desktop Explorer 한글 패치 (비공식)

스팀 게임 **Desktop Explorer** 의 비공식 한국어 번역 패치입니다.

기계번역(구글·파파고 등)이 아니라 AI 직접 번역했으며, 게임 자체의 로컬라이제이션(언어) 시스템에 한글을 넣는 **네이티브 방식**이라 대사·문서·일기·터미널·웹·메뉴 등 게임 내 텍스트가 자연스럽게 한글로 표시됩니다.

- 대상 게임 버전: **v1.0.50**
- 한글 폰트: 나눔고딕(SIL Open Font License) / 윈도우 맑은 고딕 폴백

---

## 다운로드 방법

1. 이 페이지 오른쪽의 **[Releases](../../releases)** (또는 **[최신 릴리즈](../../releases/latest)**) 를 클릭합니다.
2. 최신 버전의 **`Assets`** 항목을 펼칩니다.
3. `DesktopExplorer_KoreanPatch_...zip` 파일을 클릭해 내려받습니다.
4. 내려받은 zip을 압축 해제합니다.

> `Source code (zip / tar.gz)` 는 소스 코드라 패치가 아닙니다. 반드시 위의 `DesktopExplorer_KoreanPatch_...zip` 을 받으세요.

---

## 설치 방법

1. 스팀 라이브러리에서 **Desktop Explorer** 를 우클릭 → **관리 → 로컬 파일 보기** 를 눌러 게임 폴더를 엽니다.
   - 폴더 안에 `DesktopExplorer.exe` 가 보이면 올바른 위치입니다.
2. 압축을 푼 폴더 안의 **내용물 전체**를 게임 폴더에 **그대로 복사**합니다.
   - "덮어쓰시겠습니까?" 창이 뜨면 **모두 예(예/덮어쓰기)** 를 누르세요.
3. 게임을 실행합니다.
4. 텍스트가 한국어로 나오면 설치 성공입니다.

복사되는 항목:

```
winhttp.dll
doorstop_config.ini
.doorstop_version
BepInEx\                (한글 폰트·줄바꿈 플러그인)
DesktopExplorer_Data\StreamingAssets\aa\catalog.json
DesktopExplorer_Data\StreamingAssets\aa\StandaloneWindows64\localization-string-tables-english(unitedstates)(en-us)_assets_all.bundle
```

---

## 중요 사항

- 스팀의 **"게임 파일 무결성 검사"** 를 하면 교체된 게임 파일(위 `catalog.json`, `...bundle`)이 원본(영어)으로 되돌아갑니다. → 그럴 때는 zip을 다시 복사하면 됩니다.
- 게임이 업데이트되면 파일 구조가 바뀌어 패치가 맞지 않을 수 있습니다. (본 패치는 **v1.0.50** 기준)
- 이미 진행 중인 세이브에서 **이미 열려 있던 창**은 영어로 남을 수 있습니다. 창을 닫았다 다시 열면 한글로 바뀝니다.

---

## 의도적으로 영어로 남긴 부분

게임 진행(퍼즐 풀이)에 직접 관련된 부분은 한글로 바꾸면 정상적으로 풀 수 없으므로 원문(영어)을 유지했습니다.

- 직접 입력해야 하는 명령어·비밀번호·정답
- 정답 판별에 쓰이는 일부 텍스트·기호
- 고유명사(등장인물·프로그램 이름 등)와 파일명
- 이미지(그림)에 그려진 글자

---

## 삭제(원상복구) 방법

1. 게임 폴더에서 `winhttp.dll`, `doorstop_config.ini`, `.doorstop_version` 파일과 `BepInEx\` 폴더를 삭제합니다.
2. 스팀에서 **"게임 파일 무결성 검사"** 를 실행하면 교체됐던 게임 파일이 원본으로 복원됩니다.

---

## 라이선스 / 크레딧

- 팬 번역 패치이며 자유롭게 재배포할 수 있습니다.
- 게임 원본 에셋·코드는 포함하지 않으며, 문자열(텍스트) 데이터만 한글로 교체합니다.
- [BepInEx](https://github.com/BepInEx/BepInEx) (LGPL-2.1)
- 나눔고딕 (SIL Open Font License 1.1)
