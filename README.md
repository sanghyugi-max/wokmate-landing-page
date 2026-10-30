# 웍메이트 랜딩페이지

기존 그릴메이트 페이지의 섹션 순서, 반응형 디자인, 영상 교체 기능, FAQ, 상담 버튼을 바탕으로 제작했습니다.

## 열어보기

dist 폴더의 index.html을 더블클릭하면 열립니다. 설치가 필요하지 않습니다.

## 문구 수정

dist/config.js에 모든 주요 문구가 모여 있습니다. hero는 첫 화면, problem은 고민, how는 작동 흐름, benefits는 장점, cases는 사례, comparison은 비교, specs는 사양, faq는 질문, cta는 마지막 상담 영역입니다. 따옴표 안의 글을 수정하고 저장하세요. 줄바꿈은 \n입니다.

## 영상·사진 교체

영상 파일을 dist/assets에 넣고 video.type을 mp4, video.src를 assets/wokmate.mp4로 설정하세요. 유튜브는 type을 youtube로 바꾸고 src에 영상 링크를 입력하세요. video.poster에는 썸네일 경로를, captions에는 VTT 자막 경로를 입력할 수 있습니다. hero의 영상 안내 문구와 buttons.watch도 함께 바꾸세요.

how.items의 image에 단계별 GIF/사진 경로를 넣으면 표시됩니다. cases.items의 image와 alt에 실제 사례 사진 경로와 설명을 입력하세요.

## 제품 사양·연락처

specs.rows에서 사양을 수정합니다. 모델별 카드가 필요하면 specs.models에 name, code, image, alt, size, gas, power, weight 필드를 갖춘 항목을 추가하세요. contact.phone과 contact.url에서 전화와 카카오톡 링크를 변경할 수 있습니다. 현재는 기존 그릴메이트 페이지의 쿡메이트 회사·상담 정보를 계승했습니다.

## 공개 전 확인할 내용

웍메이트 원본 폴더가 비어 있어 실제 제품 영상·사진·모델명·처리량·열원·보증 조건은 임의로 채우지 않았습니다. 볶음 조리 관련 문구는 제작 초안이므로 실제 지원 기능에 맞게 확인하세요. 사례와 사양 등록을 마치면 해당 placeholder를 false로, 상단 시안 안내는 draft.show를 false로 바꾸세요. 그릴메이트 전용 영상과 사양은 포함하지 않았습니다.

## 설치 사례 사진 슬라이드 (2026-10-30)

`dist/config.js`의 `cases.items[0].images`에서 사진 순서와 설명을 수정합니다.
사진은 `dist/assets/installations/`에 있으며 1:1 비율로 표시합니다.
4.5초 간격으로 자동 전환하고 이전/다음, 일시정지/재생을 지원합니다.
마우스를 올리거나 키보드로 버튼에 접근하면 자동 전환이 잠시 멈춥니다.
기기의 동작 줄이기 설정을 사용하면 수동 재생으로 시작합니다.
