# Hangul for Little Hands — 음원 페이지

책 뒤쪽 QR이 가리키는 페이지입니다. 정적 파일뿐이라 서버가 필요 없습니다.

```
index.html      페이지 전체 (CSS·JS 인라인)
data.js         자모 24 · 낱말 49 데이터
audio/          mp3 97개 (평준화 -16 LUFS, 64kbps 모노)
icons/          낱말 아이콘 49개 (webp)
fonts/          Gaegu-Bold 서브셋 (102자, 25KB, OFL)
```

## GitHub Pages 올리는 법

1. github.com 에서 새 저장소 만들기 → 이름 `hangul-sounds`, **Public**
2. 이 폴더의 파일 전부를 저장소에 업로드 (드래그 앤 드롭 가능)
3. 저장소 Settings → Pages → Source를 `Deploy from a branch`,
   Branch를 `main` / `/ (root)` 로 두고 Save
4. 1~2분 뒤 아래 주소가 열립니다

```
https://<본인_깃허브_아이디>.github.io/hangul-sounds/
```

이 주소를 알려주시면 `matter.py`의 `QR_URL`을 바꾸고 본문 67페이지를 다시 굽습니다.

## 용량

전체 2.5MB. 첫 화면은 오디오를 미리 받지 않고(`preload="none"`),
탭한 것만 내려받습니다. 아이콘도 지연 로딩이라 셀룰러에서도 가볍습니다.

## 폰트 라이선스

Gaegu는 SIL Open Font License 1.1입니다. 웹 임베딩과 상업적 사용 모두 허용되며,
서브셋으로 재배포하는 것도 허용됩니다. 저작권 고지는 책 판권지에 이미 있습니다.
