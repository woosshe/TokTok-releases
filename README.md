# TokTok

Windows용 스티키 노트 관리자. Electron 트레이 앱으로, 프레임리스 메모 창을 바탕화면에
띄우고 접으면 화면 가장자리에 "알약(pill)"으로 도킹됩니다.

## 다운로드

**[최신 버전 1.2.2 내려받기](https://github.com/woosshe/TokTok-releases/releases/latest)** — `TokTok-1.2.2-Setup.exe`

[Releases](https://github.com/woosshe/TokTok-releases/releases/latest)에서 `TokTok-<버전>-Setup.exe`를
받아 실행하면 됩니다. 마법사 없이 바로 설치되며 관리자 권한은 필요 없습니다.

> **"Windows의 PC 보호" 경고가 뜬다면** — **자세히** → **실행**을 누르면 설치됩니다.
> 코드 서명 인증서가 없어서 나오는 경고입니다. 백신이 의심 파일로 표시하는 것도 같은 이유이며
> (서명이 없고 내려받은 사람이 적은 프로그램은 평판 정보가 없습니다), 파일 자체의 문제는
> 아닙니다. 설치한 뒤 앱이 스스로 하는 업데이트에서는 이 경고가 나오지 않습니다.

설치 후에는 앱이 새 버전을 스스로 확인·다운로드하고, 클릭 한 번으로 설치합니다.

## 기능

- **프레임리스 메모** — 리치텍스트(B/I/U/S, 글머리·번호 목록), 글자색
  (선택 영역만 또는 전체), 어두운 배경이면 툴바 아이콘 자동 반전
- **우클릭 메뉴** — 메모 위에서 우클릭하면(또는 상단바 `⋯`) 배경색·투명도·항상 위·알림·접기·삭제가
  한 곳에 모여 있습니다. 접어 둔 알약 위에서도 열립니다
- **알림(리마인더)** — 메모마다 알림 시각을 걸어 두면 그 시각에 Windows 알림으로 알려줍니다.
  10분 후 / 1시간 후 / 오늘 저녁 / 내일 아침 프리셋, **`N 분/시간 후`**, 달력·시계로 직접 지정 중
  아무 쪽이나 쓰면 됩니다. 알림을 클릭하면 그 메모가 화면에 뜨고(닫아 둔 메모도, 접어 둔 알약도)
  확인한 알림은 해제됩니다. 알림 시각은 기기 간에 공유됩니다.
  > **앱이 떠 있어야 알림이 옵니다.** TokTok은 백그라운드 서비스가 아니라 트레이 앱이라
  > 종료한 동안에는 알림이 울리지 않습니다(다시 켤 때 하루 이내로 지난 것만 알려줍니다).
  > 트레이 메뉴의 **Windows 시작 시 자동 실행**을 켜 두시길 권합니다.
- **접기/펼치기** — 접으면 화면 가장자리에 알약으로 도킹, 부드러운 애니메이션.
  알약끼리 겹치지 않게 자동 배치, 안쪽 그립으로 폭 조절(100–300px).
  트레이에서 **모두 접기 / 모두 펼치기**
- **메모 숨기기** — ✕로 창을 닫으면 메모가 지워지지 않고 **목록에만 남습니다.** 목록에서 다시
  띄울 수 있고, 이 상태는 기기 간에도 공유됩니다
- **메모 목록** — `Ctrl+Alt+F`. 모든 메모 본문 검색(검색어 강조 + 그 위치로 자동 스크롤),
  메모 색으로 걸러 보기, **색 그룹 단위로 한꺼번에 보이기/숨기기**, 목록에서 바로 삭제
- **메모별 투명도** 30–100%, **글자 크기** 본문에서 `Ctrl+휠`로 50–300%
- **다크 모드** — 자동(Windows 설정 따라감) / 밝게 / 어둡게
- **화면 밖 메모 복구** — 모니터를 빼거나 해상도를 바꿔 메모가 보이지 않는 곳에 남으면
  자동으로 화면 안으로 되돌린다
- **항상 위 고정**, 창 드래그 이동, 생성/수정일 표시
- **휴지통** — 삭제한 메모 30일 보관 후 자동 삭제, 복구/영구삭제/**비우기**, 실시간 갱신
- **백업** — 설정 창에서 메모 전체를 파일로 내보내고, 다른 기기/시점의 백업을 가져올 수
  있습니다. 자동으로 남는 백업 파일 목록도 설정 창에서 열거나 폴더로 이동할 수 있습니다
- **트레이 상주** — 트레이 더블클릭/`Ctrl+Alt+N`으로 새 메모,
  `Ctrl+Alt+V`로 클립보드 내용을 담은 새 메모
- **업데이트** — 새 버전이 나오면 알려주고, **물어본 뒤에** 내려받아 설치합니다.
  자동 확인은 설정에서 끌 수 있고, 마지막으로 확인한 시각도 보여줍니다
  (설정 창에서 변경점 확인 가능)
- **체크리스트** — 본문에 할 일 체크박스, 클릭으로 완료 처리

## 버전 히스토리

- **1.2.2** — **여러 줄을 한 번에 체크리스트로 만들 수 있습니다.** 줄을 여러 개 선택하고 체크리스트
  버튼을 누르면 줄마다 체크 항목이 됩니다(예전에는 선택한 글이 지워지고 빈 항목 하나만 남았습니다).
  이미 만들어 둔 글머리·번호 목록을 골라 눌러도 그대로 체크리스트가 됩니다.
  **`- ` 이나 `1. ` 로 시작하는 글을 붙여넣으면 글머리·번호 목록으로 들어옵니다** — 다른 곳에
  적어 둔 목록을 그대로 가져올 수 있습니다.
  메모의 **`+` 버튼으로 만든 새 메모는 그 메모와 같은 색**으로 나옵니다(트레이 아이콘과 단축키로
  만들 때는 기본색 그대로입니다).
  설정 창의 **변경 내용**은 이제 서식대로 보입니다 — 지금 읽고 계신 이 글처럼 굵게·목록·인용이
  그대로 그려집니다(예전에는 기호가 글자 그대로 보였습니다).

- **1.2.1** — **Google Drive 동기화가 드라이브의 앱 전용 숨김 공간을 씁니다.** 이제 내 드라이브에
  `TokTok` 폴더가 보이지 않습니다 — 열어 볼 일이 없는 폴더가 눈에 띄지 않고, 그 파일을 실수로
  옮기거나 지워서 동기화가 깨질 일도 없습니다. 앱은 여전히 자기 데이터 외에는 드라이브의 어떤
  파일도 볼 수 없습니다.

  > ⚠️ **Drive 동기화를 쓰고 계셨다면 설정 창에서 `연결 해제` → `Google 계정 연결`을 한 번 해
  > 주세요.** 그 전까지는 예전 위치로 그대로 동기화되므로 메모가 사라지지는 않지만, **재연결한
  > 기기와 안 한 기기는 서로 다른 곳을 보게 되어 그 사이에는 메모가 오가지 않습니다** — 쓰시는
  > 기기 모두에서 해 주시는 게 좋습니다. 전부 재연결한 뒤에는 **내 드라이브에 남은 `TokTok`
  > 폴더를 지우셔도 됩니다.**

- **1.2.0** — **앱을 한국어와 영어로 쓸 수 있습니다.** 설정 창의 **언어**에서 고르며, 기본값인
  `자동`은 Windows 언어를 따라갑니다(한국어면 한국어, 그 밖에는 영어). 바꾸면 다시 시작할지
  물어보고, 나중에 하더라도 다음 실행부터 적용됩니다. 이 변경 내용도 앱 언어에 맞춰 보입니다.
  메모 내용은 그대로입니다 — 바뀌는 것은 버튼·메뉴 같은 앱 화면의 글자뿐입니다.

- **1.1.0** — **메모에 이미지를 붙여넣을 수 있습니다.** 스크린샷은 저장될 때 자동으로 가볍게
  변환되고(용량이 크게 줄어듭니다), 웹에서 복사한 이미지는 메모 안에 담기므로 인터넷이 없어도
  보입니다. 메모 목록과 휴지통에서는 작은 미리보기로 나옵니다.
  붙여넣기도 깔끔해졌습니다 — 웹에서 글을 복사해도 **배경색과 글자색이 따라오지 않고** 목록·굵게
  같은 구조만 남습니다.
  **항상 위**는 이제 메모 아래쪽 도구 모음의 **핀 버튼**으로 바로 켜고 끌 수 있습니다(접어서 알약
  상태일 때는 가장자리에 핀 표시가 남습니다).
  고친 것: 지웠던 빈 메모가 동기화 후 **저절로 다시 나타나던** 문제, 이미지만 붙여넣은 메모를
  ✕로 닫으면 **메모가 사라지던** 문제, 휴지통에서 이미지 메모가 `(빈 메모)`로 보이던 문제,
  트레이 아이콘을 두 번 눌러 새 메모를 만들 때 **메모 목록이 같이 뜨거나 메모가 두 개 생기던**
  문제, 붙여넣은 움직이는 GIF가 **정지 화면이 되던** 문제, 검색이 `<` `>` `&` 도 찾도록 한 것

  > ⚠️ **여러 기기에서 쓰신다면 모두 이 버전으로 업데이트해 주세요.**
  > 이번 버전부터 **완전 삭제가 기기 간에 제대로 전파됩니다.** 예전에는 한 기기에서 메모를
  > 완전히 지워도 다른 기기에 남아 있던 사본이 동기화될 때 되살아났는데, 이제 "지웠다"는 기록을
  > 남겨 그것을 막습니다. 다만 **예전 버전 기기는 그 기록을 알아보지 못해** 휴지통에 빈 항목으로
  > 보입니다(그 항목을 복구하면 빈 메모가 생깁니다). 모두 업데이트하면 이 현상은 사라집니다.

- **1.0.1** — 고친 것: 메모가 하나도 안 보이는 상태에서 작업 표시줄의 TokTok 버튼을 눌러 뜬
  메모 목록 창을 닫아도, 버튼을 다시 누를 때마다 그 창이 계속 다시 떠 있던 문제. 화면에 떠
  있던 마지막 메모를 닫는 순간에도 목록 창이 저절로 뜨던 문제.
- **1.0.0** — 메모를 여러 개 띄워도 **작업 표시줄에는 TokTok 버튼이 하나만** 뜹니다(예전에는 띄운
  메모 수만큼 늘어났습니다). 그 버튼을 누르면 트레이 아이콘을 누른 것과 같이 떠 있는 메모가 모두
  앞으로 나오고, 마우스를 올렸을 때 나오는 미리보기에는 TokTok 아이콘이 표시됩니다. 작업 표시줄에서
  아예 감추고 싶다면 설정 창의 **작업 표시줄 → 트레이 아이콘만 사용**을 켜면 트레이 아이콘으로만
  열 수 있습니다.
  고친 것: 화면 배율이 서로 다른 모니터(예: 100%와 125%) 사이로 메모를 여러 번 옮기면 **메모와
  알약이 조금씩 커지던** 문제
- **0.9.0** — 설정 창에 **백업**이 생겼습니다. 메모 전체를 파일로 내보내고, 다른 기기나 시점의
  백업을 가져올 수 있습니다(가져온 메모는 목록에 숨겨진 채로 들어오므로, 확인한 뒤 원하는 것만
  띄우면 됩니다). 자동으로 남는 백업 파일도 설정 창에서 바로 열거나 폴더로 이동할 수 있습니다.
  휴지통에 **비우기**가 생겨 쌓인 메모를 한 번에 완전히 지울 수 있고, 우클릭 메뉴에는 **같은 색
  모두 접기**가 생겼습니다. 빈 메모는 이제 ✕로 닫을 때 목록에 남기지 않고 바로 지웁니다.
  고친 것: 모니터를 두 대 이상 쓸 때 알약이 다른 모니터에 있는 알약 때문에 엉뚱한 자리로 밀려
  붙던 문제
- **0.8.2** — 알림 메뉴의 `N 분/시간 후` 줄을 고쳤습니다. 숫자 칸을 눌렀을 때 **자주 쓰는 값이
  하나만 보이던 문제**, **어두운 테마에서 `분/시간` 목록의 글자가 잘 보이지 않던 문제**를
  고쳤고, 숫자 칸과 단위 칸의 폭을 같게 맞췄습니다. `내일 저녁` 프리셋이 추가됐습니다
- **0.8.1** — 알림 메뉴에 **`N 분/시간 후`**가 생겼습니다. 숫자는 직접 입력할 수도 있고 자주 쓰는
  값에서 고를 수도 있어, 프리셋으로 딱 맞지 않는 간격("40분 뒤")을 바로 걸 수 있습니다.
  `직접 지정`에서 **달력·시계 피커**도 쓸 수 있게 됐습니다(키보드 입력도 그대로 됩니다)
- **0.8.0** — **메모마다 알림을 걸 수 있습니다.** 우클릭 메뉴(또는 상단바 `⋯`) → **알림**에서
  10분 후 / 1시간 후 / 오늘 저녁 / 내일 아침을 고르거나 시각을 직접 지정하면, 그 시각에 Windows
  알림으로 알려줍니다. **알림을 클릭하면 그 메모가 화면에 뜹니다** — 닫아 둔 메모도 되살아나고,
  접어 둔 알약은 펼쳐지며, 확인한 알림은 자동으로 해제됩니다. 알림 시각은 기기 간에 공유되고
  (알림은 기기마다 한 번씩 옵니다), 메모 목록과 메모 창에 종 아이콘으로 표시됩니다.
  > 앱이 떠 있어야 알림이 옵니다. 종료한 동안에는 울리지 않고, 다시 켤 때 이틀 이내로 지난 것만
  > 알려줍니다. 트레이 메뉴의 **Windows 시작 시 자동 실행**을 권합니다.

  우클릭 메뉴에 **같은 색 모두 보기**가 생겼습니다 — 같은 색인데 닫아 둔 메모를 한 번에
  되살립니다. **새 메모가 열리는 자리**도 달라졌습니다: 기존 메모와 겹치지 않게 방금 작업한 메모
  옆에 놓이고(`+`를 누른 메모가 기준), 화면에 펼친 메모가 없으면 화면 중앙에 뜹니다.
  고친 것: 메모 본문에서 우클릭할 때 복사·붙여넣기 같은 **윈도우 기본 편집 메뉴**가 나오도록
  되돌렸습니다(툴바·알약 우클릭은 그대로 TokTok 메뉴), 메모가 '항상 위'이고 크면 **삭제 확인
  창이 메모에 가려 보이지 않던** 문제
- **0.7.0** — 메모를 **지우지 않고 화면에서만 내릴 수 있습니다.** 창의 ✕(또는 `Alt+F4`)로 닫으면
  메모는 사라지지 않고 `Ctrl+Alt+F` **목록에 남고**, 거기서 다시 띄울 수 있습니다. 이 상태는
  기기 간에도 공유되므로 한쪽에서 정리하면 다른 PC에서도 정리됩니다. 목록에서는 **메모 색을
  그룹처럼 써서 한꺼번에 보이기/숨기기**가 되고(검색 결과에도 그대로 적용됩니다), 메모를 바로
  삭제할 수도 있습니다. 메모 창 툴바를 정리해 배경색·투명도·항상 위·접기·삭제를 **우클릭
  메뉴**로 옮겼습니다 — 상단바의 `⋯`로도 열리고, 접어 둔 알약 위에서도 열립니다. 메모를 여러 개
  띄울 때 **메모리 사용량이 크게 줄었습니다**(20개 기준 프로세스 23개 → 4개).
  고친 것: 툴바 ✕로 닫은 상태가 저장되지 않아 재시작하면 메모가 도로 나오던 문제,
  메모 창을 오른쪽 버튼으로 끌면 창이 움직이던 문제
- **0.6.3** — `Ctrl+Alt+F` 창이 **메모 목록**을 겸합니다. 검색어를 비우면 모든 메모가 최근 수정
  순으로 나오고, 메모 색으로 걸러 볼 수 있습니다. 검색 결과와 휴지통에서 메모 내용이 잘린 요약이
  아니라 **원래 모양 그대로** 보이고(체크리스트·서식 포함), 검색어에는 색이 칠해지며 그 위치로
  자동으로 스크롤됩니다. 고친 것: 메모 창을 `Alt+F4`로 닫으면 다시 열 방법이 없어 프로그램을
  재시작해야 했던 문제(이제 트레이의 "모든 메모 보이기"와 목록에서 되살아납니다),
  검색·휴지통·설정 창의 스크롤바 모양이 메모 창과 달랐던 문제
- **0.6.2** — 업데이트를 받아오는 저장소를 이전 위치로 되돌렸습니다. **0.6.1을 쓰고 계셨다면
  이 버전은 직접 받아 설치해 주세요** — 0.6.1은 자동 업데이트를 받지 못합니다. 설치하고 나면
  이후 버전부터는 다시 자동으로 갱신됩니다
- ~~**0.6.1** — 업데이트를 받아오는 곳을 잠시 옮겼던 버전입니다~~ (내려받을 수 없습니다. 0.6.2를 쓰세요)
- **0.6.0** — 다크모드 추가(자동/밝게/어둡게, 설정 창 맨 위에서 선택). 어둡게 볼 때는 본문이
  어두운 회색이 되고 메모 색은 상단 바·알약에 남아 어느 메모인지 그대로 구분됩니다.
  `Ctrl+Alt+V`로 클립보드 내용을 담은 새 메모. 고친 것: 체크리스트에서 엔터로 목록을 벗어난 뒤
  입력한 글자에 취소선이 남던 문제, 트레이 "모두 접기"에서 알약이 겹치던 문제,
  창이 뜰 때 흰 배경이 잠깐 보이던 문제, 본문 스크롤바 위에서 커서가 글자 입력 모양이던 문제
- **0.5.1** — 업데이트를 **물어본 뒤에** 내려받고 설치합니다(전에는 묻지 않고 받았습니다).
  자동 확인을 끌 수 있는 설정과 마지막으로 확인한 시각 표시 추가. 재설치할 때 실행 중인
  TokTok을 자동으로 닫습니다 — 편집 중이던 내용을 저장하고 동기화한 뒤 닫으므로 안전합니다
  (전에는 "TokTok을 닫을 수 없습니다"가 뜨고 직접 종료해야 했습니다)
- **0.5.0** — 화면 밖으로 사라진 메모 자동 복구(모니터를 빼거나 해상도를 바꿔도 메모가 보이는
  곳으로 돌아온다), 트레이에서 모두 접기/모두 펼치기, 메모별 투명도 조절(상단 툴바 슬라이더,
  30–100%), `Ctrl+휠`로 본문 글자 크기 조절(50–300%), exe 아이콘을 크기별로 만든 `.ico`로 교체해
  작업표시줄·탐색기에서 또렷하게. 다른 기기에서 켠 "항상 위"가 이 기기의 창에 반영되지 않던 문제,
  메모를 여러 개 빠르게 접을 때 알약이 겹치던 문제 수정
- **0.4.0** — 자동 업데이트(새 버전 자동 다운로드 + 클릭 한 번 설치, 설정 창에 변경 내역
  표시), 본문 체크리스트, 전체 검색(`Ctrl+Alt+F`), 펼친 메모 최소 크기 240×240으로 조정
- **0.3.0** — Google Drive API 직접 동기화 (드라이브 데스크톱 앱 불필요), 본문
  암호화가 항상 켜짐(암호문구 입력 없이 앱 내장 키로 자동 처리), 중복 실행 방지,
  배포 형식을 portable exe에서 설치본(oneClick)으로 변경, 설정 창·트레이에 버전 및
  최신 버전 여부 표시
- **0.2.1** — Windows 시작 시 자동 실행(트레이 메뉴 토글) 추가
- **0.2.0** — 알약 도킹 오버행 제거(듀얼모니터 삐짐 방지), 마크다운식 리스트 단축키
  (`-`/`1` + Tab → ul/ol), 본문 Tab 포커스 이동 비활성화, 실행 시 메모 없으면 새 메모
  자동 생성, 어두운 배경에서 기본 본문색 자동 밝게(직접 지정색은 유지)
- **0.1.0** — 최초 버전: 프레임리스 메모, 접기/펼치기·가장자리 도킹, 리치텍스트,
  배경색, 알약 폭 조절, 휴지통, 트레이 상주, exe 빌드

## Version history

- **1.2.2** — **Turn several lines into a checklist at once.** Select multiple lines and press the
  checklist button and every line becomes its own item (it used to wipe the selection and leave a
  single empty item). Picking an existing bulleted or numbered list works the same way.
  **Paste text whose lines start with `- ` or `1. ` and it comes in as a bulleted or numbered
  list** — handy for bringing over a list you wrote somewhere else.
  A note made with a note's **`+` button now takes that note's colour** (the tray icon and the
  keyboard shortcut still make the default yellow one).
  **What's new** in Settings is now rendered with its formatting — bold, lists and quotes appear
  the way you're reading them here, instead of showing the raw markup.

- **1.2.1** — **Google Drive sync now uses the hidden app-only area of your Drive.** The `TokTok`
  folder no longer shows up in My Drive — a folder you never open stays out of your way, and the
  file can't be moved or deleted by accident and break your sync. As before, TokTok can't see any
  file in your Drive other than its own data.

  > ⚠️ **If you were using Drive sync, open Settings and do `Disconnect` → `Connect Google
  > account` once.** Until you do, that device keeps syncing to the old location, so nothing is
  > lost — but **a reconnected device and a device that hasn't reconnected point at different
  > places, so notes stop travelling between them.** Best to do it on every device you use. Once
  > they're all reconnected, you can **delete the leftover `TokTok` folder in My Drive.**

- **1.2.0** — **TokTok now speaks English as well as Korean.** Pick your language under
  **Language** in Settings; the default `Auto` follows your Windows language (Korean if your
  system is Korean, English otherwise). Changing it asks whether to restart, and if you say
  later it applies the next time you start TokTok. These release notes follow the app language
  too. Your notes are untouched — only the app's own text changes.

- **1.1.0** — **You can paste images into notes.** Screenshots are automatically converted to a
  lighter format when saved (a large size reduction), and images copied from the web are stored
  inside the note, so they still show up with no internet connection. Notes list and Trash show
  them as small previews.
  Pasting is cleaner too — copying text from the web no longer brings **background and font
  colors** with it, only structure such as lists and bold.
  **Always on top** now has its own **pin button** in the note's bottom toolbar (when a note is
  collapsed into a pill, the pin shows along its edge instead).
  Fixes: deleted empty notes **reappearing on their own** after a sync, closing an image-only
  note with ✕ **losing the note**, image notes showing as `(empty note)` in Trash,
  double-clicking the tray icon to create a note **also opening the notes list or creating two
  notes**, pasted animated GIFs **turning into a still frame**, and search now matches
  `<` `>` `&` as well

  > ⚠️ **If you use TokTok on more than one device, please update them all to this version.**
  > From this version, **permanent deletion propagates correctly between devices.** Previously,
  > permanently deleting a note on one device could bring it back when a copy on another device
  > synced; TokTok now records that it was deleted and blocks that. However, **devices on older
  > versions do not understand that record** and show it as an empty item in Trash (restoring
  > that item creates an empty note). Once every device is updated, this goes away.

- **1.0.1** — Fixes: with no notes on screen, the notes list opened from the TokTok taskbar
  button kept coming back every time the button was pressed, even after closing it. The notes
  list also opened by itself the moment the last visible note was closed.
- **1.0.0** — However many notes are on screen, **the taskbar now shows a single TokTok button**
  (it used to show one per note). Pressing it brings every visible note to the front, exactly
  like clicking the tray icon, and its hover preview shows the TokTok icon. To keep TokTok off
  the taskbar entirely, turn on **Taskbar → Use the tray icon only** in Settings and open it
  from the tray icon instead.
  Fixes: notes and pills **growing slightly larger** each time they were dragged between
  monitors with different display scaling (for example 100% and 125%)
- **0.9.0** — Settings now has **Backup**. You can export all your notes to a file and import a
  backup from another device or point in time (imported notes arrive hidden in the notes list,
  so you can review them and show only the ones you want). Automatic backup files can be opened
  or revealed in their folder straight from Settings.
  Trash gained **Empty trash** to permanently delete everything at once, and the context menu
  gained **Collapse same color**. Empty notes are now deleted outright when closed with ✕
  instead of being left in the list.
  Fixes: with two or more monitors, pills docking to the wrong spot because of pills on another
  monitor
- **0.8.2** — Fixed the `in N minutes/hours` row in the reminder menu: **only one suggested
  value appearing** when the number box was clicked, and **the minutes/hours list being hard to
  read in the dark theme**. The number and unit boxes are now the same width. Added a
  `Tomorrow evening` preset
- **0.8.1** — The reminder menu gained **`in N minutes/hours`**. You can type the number or pick
  a common one, so intervals the presets don't cover ("in 40 minutes") can be set directly.
  `Pick a time` can also use the **calendar and clock pickers** now (typing still works)
- **0.8.0** — **You can set a reminder on any note.** In the context menu (or `⋯` in the title
  bar) → **Reminder**, choose in 10 minutes / in 1 hour / this evening / tomorrow morning, or
  pick a time, and Windows notifies you then. **Clicking the notification brings that note up** —
  a closed note comes back, a collapsed pill expands, and the reminder clears itself once seen.
  Reminder times are shared between devices (each device notifies you once), and a bell icon
  marks them in the notes list and on the note.
  > TokTok has to be running to notify you. Nothing fires while it is closed, and on the next
  > start you only hear about reminders from the last two days. **Start with Windows** in the
  > tray menu is recommended.

  The context menu gained **Show same color** — it brings back every closed note of that color
  at once. **Where a new note opens** changed too: it is placed next to the note you last worked
  on without overlapping (the note whose `+` you pressed wins), or in the center of the screen
  when no note is open.
  Fixes: right-clicking inside a note's text now brings back **the standard Windows edit menu**
  with copy and paste (right-clicking the toolbar or a pill still opens the TokTok menu), and
  **the delete confirmation being hidden behind** a large always-on-top note
- **0.7.0** — **You can take a note off the screen without deleting it.** Closing a note with ✕
  (or `Alt+F4`) no longer discards it — **it stays in the `Ctrl+Alt+F` list** and can be shown
  again from there. This is shared between devices, so tidying up on one PC tidies the other.
  In the list you can **use note colors as groups to show or hide notes in bulk** (this applies
  to search results too), and delete notes directly. The note toolbar was trimmed: background
  color, opacity, always on top, collapse and delete moved to the **context menu** — also
  reachable from `⋯` in the title bar, and from a collapsed pill.
  **Memory use dropped sharply** with many notes open (23 processes → 4 with 20 notes).
  Fixes: closing with the toolbar ✕ not being saved, so notes came back after a restart, and
  notes being dragged with the right mouse button
- **0.6.3** — The `Ctrl+Alt+F` window doubles as a **notes list**. Clear the search box and every
  note appears, most recently edited first, and you can filter by note color. Search results and
  Trash now show note content **as it really looks** instead of a trimmed summary (checklists and
  formatting included), search terms are highlighted, and the view scrolls to them automatically.
  Fixes: a note closed with `Alt+F4` could not be reopened without restarting TokTok (it now
  comes back from "Show all notes" in the tray and from the list), and the scrollbars in the
  search, Trash and Settings windows not matching the note window
- **0.6.2** — Moved the update source back to its previous location. **If you were using 0.6.1,
  please download and install this version manually** — 0.6.1 cannot receive automatic updates.
  Once installed, later versions update automatically again
- ~~**0.6.1** — A version that briefly moved where updates were fetched from~~ (no longer
  available — please use 0.6.2)
- **0.6.0** — Added a dark theme (auto / light / dark, at the top of Settings). In dark mode the
  note body turns dark gray while the note color stays on the title bar and pill, so notes are
  still easy to tell apart. `Ctrl+Alt+V` creates a new note from the clipboard.
  Fixes: text typed after leaving a checklist with Enter keeping the strikethrough, pills
  overlapping after "Collapse all" from the tray, a white flash when a window opened, and the
  cursor showing as a text cursor over the body scrollbar
- **0.5.1** — Updates are now downloaded and installed **only after asking you** (previously they
  were downloaded silently). Added a setting to turn off automatic checks and a display of when
  TokTok last checked. Reinstalling closes a running TokTok automatically — it saves and syncs
  your edits first, so nothing is lost (previously "TokTok cannot be closed" appeared and you had
  to quit it yourself)
- **0.5.0** — Notes stranded off-screen are recovered automatically (unplugging a monitor or
  changing resolution brings them back into view), Collapse all / Expand all in the tray, per-note
  opacity (toolbar slider, 30–100%), `Ctrl`+wheel to change body text size (50–300%), and the exe
  icon was replaced with a multi-size `.ico` so it stays sharp in the taskbar and Explorer.
  Fixes: "always on top" set on another device not reaching this one, and pills overlapping when
  several notes were collapsed quickly
- **0.4.0** — Automatic updates (new versions download on their own and install with one click,
  with the changelog shown in Settings), checklists, full-text search (`Ctrl+Alt+F`), and the
  minimum size of an expanded note adjusted to 240×240
- **0.3.0** — Direct Google Drive sync via the Drive API (no Drive desktop app required), note
  content always encrypted (handled automatically with a built-in key, no passphrase to type),
  a guard against running twice, the download changed from a portable exe to a one-click
  installer, and the current and latest version shown in Settings and the tray
- **0.2.1** — Added Start with Windows (a toggle in the tray menu)
- **0.2.0** — Docked pills no longer overhang the screen edge (which looked broken on dual
  monitors), Markdown-style list shortcuts (`-`/`1` + Tab → bulleted/numbered list), Tab no
  longer moves focus out of the body, a new note is created on startup when there are none, and
  the default body color brightens automatically on dark backgrounds (colors you picked yourself
  are kept)
- **0.1.0** — First release: frameless notes, collapse/expand with edge docking, rich text,
  background colors, adjustable pill width, Trash, a tray icon, and an exe build

---

이 페이지는 릴리스할 때마다 자동으로 갱신됩니다. 배포물 전용 저장소이며, 소스는 비공개입니다.
