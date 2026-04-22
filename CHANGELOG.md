# 변경 이력 (CHANGELOG)

오토샷 (autoshot)
Copyright (C) 2026 박병진. All Rights Reserved.

본 문서는 공개 배포본의 시계열 변경 이력만을 기록한다.
구판 내부 단계(v1.x ~ v3.13.x)는 비공개로 보관한다.

---

## v3.15.1 (2026-04-22, 정본)

수리 — Windows windowed 빌드에서 자식 프로세스(Tesseract OCR, wmic) 호출 시 cmd 창이 순간 깜빡이며 노출되던 현상 차단.
- 모듈 상수 `_CREATE_NO_WINDOW = 0x08000000` 신설
- subprocess 호출부 `creationflags=_CREATE_NO_WINDOW` 일괄 적용
- 기존 함수·클래스 시그니처 무변경, 기능 무변경

산출물
- `autoshot.exe` 19,668,811 bytes (18.76 MB)
- 빌드 도구 PyInstaller (single-file, windowed, UPX)

---

## v3.15.0 (2026-04-22)

제호 승격 — `딸깍블랙박스(clickblackbox)` → `오토샷(autoshot)`.
- 코드 식별자 AUTOSHOT 도입, 제호 일치 확보
- 엔트리 파일 개명 `blackbox_v3_14.py` → `autoshot_v3_15.py`
- VersionInfo 리소스 ProductName·InternalName·OriginalFilename·FileDescription 갱신
- FREE_BUILD_ID 접두 `CBB` → `AUS` 승격
- BRAND_CAPTIONS 20슬롯 용도 중심 재편 (소송·행정심판·온라인 거래·원격근무·강의 스틸컷·영상 감상·교육자료·화상회의·실험일지·전산 오류·근무시간·저작권 침해 기록)

브랜드
- 회사명 표기 `딸깍컴퍼니(예정)` 고착
- 자매 도구 `딸깍 법무킷(ClickLegalKit)` 명칭 확정

무결성
- SentinelHyperV530 클래스 시그니처 및 기존 메서드 시그니처 무변경
- 함수·클래스 골격 무변경

---

## v3.14.1 (2026-04-21, 비공개 보관)

저작권 등록 복제물 동결 시점 정본.
공개 배포 채널에는 게시하지 아니한다.

---

## 이전 버전

v1.x ~ v3.13.x 내부 개발 단계. 비공개 보관.
공개 배포 시점 기준 v3.15.0이 최초 외부 공표 버전이다.
