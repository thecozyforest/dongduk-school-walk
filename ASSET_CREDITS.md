# 에셋 출처와 제작 기록

## 가상의 여학생 탐방 캐릭터 (2026-10-23)

- `src/campus-student.ts`는 이 프로젝트에서 Three.js 기본 도형과 직접 작성한 곡면·관절 동작으로 제작한 원본 캐릭터다. 코드와 모형은 저장소의 MIT 라이선스를 따른다.
- 실제 학생의 얼굴·사진·명찰이나 외부 캐릭터 에셋을 사용하지 않았다. 어깨 길이의 머리, 남색 재킷과 주름치마는 가상의 탐방 안내자 디자인이며 실제 학교 교복을 확인해 재현한 것은 아니다.
- 서기·걷기·앉기·손 흔들기 동작을 코드로 구현했다. 기존 Meshy 원본과 CC BY 4.0 제작 기록은 그대로 보존한다.

이 저장소의 모형·이미지·소리를 누가, 무엇으로, 어떤 조건으로 만들었는지 적는다. 다른 학교가 캐릭터나 모형을 바꾸면 이 문서의 해당 항목을 그 학교의 기록으로 바꾼다([학교 캐릭터 만들기](docs/학교-캐릭터-만들기.md)).

Meshy 모형과 그 파생본은 CC BY 4.0이다. 공유할 때는 제작 정보, [라이선스 링크](https://creativecommons.org/licenses/by/4.0/), 바꾼 사실을 함께 제공한다. 사이트 도움말에도 출처를 표시한다(`src/school-config.ts`의 `about.credits`).

## 학생 캐릭터 — 청학고 교복

- 제작: 청학고 도쌤(dossamlab), [Meshy](https://www.meshy.ai/) **Meshy 6 Lite**, 2026-10-15. Meshy 작업 이름 「Tiny Scholar」, 작업 식별자 `01a13d18-7fed-74bb-bb2f-dc5f880296ca`.
- 라이선스: **CC BY 4.0** — 2026-10-22 제작 계정의 Meshy 에셋 상세 화면에서 확인. 무료 요금제로 만든 모형이다.
- 원본: `assets/school-player-meshy-source.glb` — 관절·동작이 없고 한쪽 다리를 든 자세의 모형. 고치지 않고 보존한다.
- 사이트용: `public/school-player-meshy.glb`. `assets/prepare_school_meshy.py`가 18개 관절을 심고, 아래 기본 주인공의 걷기 동작을 옮겨 붙이고, 키 1.70m·22,000삼각형으로 정리한다. 재킷의 버건디색과 피부색을 보정했다. 과정은 [청학고 교복 기록](docs/cheonghak/SCHOOL_UNIFORM_PLAN.md)에 있다.
- 교복은 사용자가 제공한 교복 사진의 색과 형태만 참고했다. 학생의 얼굴·체형·명찰은 따라 만들지 않았고, 사진은 저장소와 외부 서비스에 넣지 않았다.

## 교직원 캐릭터 4명

- 교장선생님·교감선생님·학교보안관·숙직실 경비원. 제작: 청학고 도쌤(dossamlab), Meshy. 제작자가 CC BY 4.0으로 공개한다.
- Meshy 무료 요금제의 결과물은 CC BY 4.0이고, 유료 요금제의 결과물은 제작자 소유라 제작자가 이용 조건을 정한다. 2026-10-22 확인한 제작 계정의 에셋 목록에는 이 네 모형이 없어 어느 요금제로 만들었는지는 확인하지 못했다. 어느 경우든 위 조건으로 공개할 수 있다.
- 원본: `assets/principal-meshy-source.glb`, `vice-principal-meshy-source.glb`, `school-marshal-meshy-source.glb`, `night-guard-meshy-source.glb`.
- 사이트용: `public/school-residents.glb`. `assets/prepare_school_residents_meshy.py`가 키 1.70m에 맞추고 학생과 같은 큰 머리 비율로 다듬는다. 숙직실 경비원은 앉은 자세로 바꾼다. 스탠딩 책상과 화장실 세면대·변기는 이 프로젝트에서 직접 만든 모형이다.
- 교장선생님·교감선생님 모형은 두 분의 동의를 받아 참고 사진으로 만들었다. 참고 사진은 저장소에 넣지 않았다.

## 기본 주인공 — 걷기 동작 원본

- 제작: dossamlab, 2026-10-04, Meshy **Meshy 6 Lite**. 모형에 표시된 라이선스: CC BY 4.0.
- 모형·색 원본: `assets/player-meshy-source.glb`(내려받은 이름 `Meshy_AI_A_single_original_cut_1004134528_texture.glb`). 관절·동작 원본: `assets/player-meshy-rig.glb` — Meshy에서 사람형 관절을 넣고 걷기 동작을 추가해 Mixamo 형식으로 내려받았다.
- 파생본: `assets/player.glb`. `assets/prepare_player.py`가 24,000삼각형 이내, 1024px 색 이미지, 큰 머리·짧은 몸의 비율로 다듬고 서기 동작을 더했다. 사이트에는 직접 나오지 않고, 학생 캐릭터에 걷기 동작을 옮겨 줄 때와 검사에 쓴다.
- 무료 크레딧 20(모형 10 + 색 10)을 사용했다. 구독·크레딧 구매는 하지 않았다.

> 생성 요청문: A single original cute human island explorer, full body in neutral A-pose for animation rigging, arms angled down 40 degrees away from torso, hands empty and separate, feet apart on ground. Chibi 2.5-heads-tall proportions, very large round head, short stocky torso, short thick limbs, rounded mitten hands, round cream boots. (이하 생략)

## 안내자 루미의 얼굴

- 화면 아래 안내 말풍선의 얼굴 그림 `public/lumi-portrait.png`(256×256 투명 PNG).
- 원본 모형: 수달 연구원 루미. 제작 dossamlab, 2026-10-04, Meshy 6 Lite, CC BY 4.0, 생성 작업 식별자(텍스처) `01a106f9-b6c9-72a9-ab7c-b99152235ace`. Blender로 다듬은 모형을 정면에서 촬영한 파생 이미지다. 3D 모형 자체는 이 저장소에 들어 있지 않다.
- 다른 학교는 학교 마스코트 그림으로 바꿔도 된다(`src/school-main.ts`의 안내 말풍선).

## 학교 건물·가구 모형

- `assets/build_school.py`, `assets/build_school_classrooms.py`로 이 프로젝트에서 직접 만든 Blender 모형이다. 벽돌·나무 무늬도 스크립트가 그린다. 상용 게임의 모형이나 텍스처를 쓰지 않았다.
- 청학고 외관 참고: [학교 공식 시설 사진](https://cheonghak-h.goegn.kr/cheonghak-h/cm/cntnts/cntntsView.do?cntntsId=3028&mi=7677), 지도 서비스의 위성사진과 거리뷰, 사용자가 제공한 현장 영상·사진. 실 이름 참고: [다산캠프 학교 안내](https://dasancamp.netlify.app/). 배치·치수 참고: 학교 설계 도면과 교실 배치도.
- 참고 사진·지도 타일·도면은 모형과 배포 파일에 넣지 않았다. 치수·문·가구·장식은 탐방을 위한 해석이며 실측 복원이 아니다.

## 소리

- 배경음악과 성공·상호작용 소리는 `src/audio.ts`의 악보·합성 코드로 이 프로젝트에서 만들었다. 브라우저 안에서 음을 생성하며 외부 음원 파일을 쓰지 않는다.

## 공유 이미지

- `public/school-share-v1.jpg`(1200×630)는 `assets/school-share-card.html`을 브라우저에서 열어 촬영한 이미지다. 학교 3D 모형 화면으로 만들었다.

## 배치도 기반 탐방 초안 (2026-10-22)

- `src/campus-plan-cells.ts`의 공간 이름과 상대 구획은 사용자가 제공한 교실배치도에서 옮겼다. 원본 문서·페이지 이미지와 개인 이름은 코드나 배포에 포함하지 않는다.
- `src/campus-scene.ts`는 이 배치 데이터로 벽·복도·문·가구를 브라우저에서 생성한다. 지도 사진·학교 사진을 재질로 사용하지 않았다. 치수·외관·문과 가구 위치·야외 공간은 탐방 초안용 추정이다.
- 주인공은 기존 `public/school-player-meshy.glb`와 `src/player.ts`의 동작을 재사용한다. 원작자 dossamlab의 CC BY 4.0 출처를 유지하며 실제 학교 학생이나 교복을 재현한 캐릭터가 아니다.
- `public/school-share-v2.jpg`(1200×630)는 이 초안의 실제 첫 화면을 브라우저에서 촬영한 공유 이미지다.

## 사진을 참고한 외관 보완 (2026-10-22)

- 사용자가 제공한 정문·건물 전경 사진 6장(파일명 기준 2025-02-07, 2026-04-30, 2026-05-04)을 주 참고로 삼았다. 공개 참고는 [정문·전경 사진 게시물](https://hj630lee.tistory.com/564)(2024-02-21), [뉴시스 사진을 수록한 파이낸셜뉴스 기사](https://www.fnnews.com/news/202411232124127626)(2024-11-23)다.
- 사진의 색·형태를 관찰해 붉은 벽돌·아치 창·기와를 얹은 석재 교문·경비실·단차와 농구대를 `src/campus-scene.ts`에서 새 기하 모형으로 표현했다. 벽돌 무늬는 코드로 직접 그렸다. 사진 파일과 사진을 잘라 만든 텍스처는 배포하지 않는다.
- 건물 본관 외곽은 공통 층 배치에서 계산한다. 창 개수·비율·지붕·문·야외 거리와 높이는 개략 표현이며, 왼쪽 별동은 외관 참고용이다. 외관과 단차는 전체 보기에서, 내부와 안내용 평지 야외는 층별 탐방에서 표시한다. 사진 속 사람·차량은 옮기지 않았다.
- `public/school-share-v3.jpg`(1200×630)는 외관을 보완한 실제 시작 화면을 브라우저에서 촬영한 이미지다.

## 운동장과 산책로 보완 (2026-10-23)

- 사용자가 제공한 운동장 전경 사진 두 장의 형태·색·상대 배치를 참고했다. 원본 사진, 사진 속 사람·차량 식별 정보는 배포하지 않는다.
- `src/campus-landscape.ts`의 소나무·수목·관목·보행로·난간·벤치·가로등·물결 차양과 관람석, 중앙 지붕 구조물은 Three.js 기하 모형으로 자체 제작했다. 흙의 미세 무늬도 코드로 그렸다. 새 외부 에셋은 없다.
- `public/school-share-v5.jpg`(1200×630)는 `assets/campus-share-card.html`에서 이 모형을 렌더링해 촬영했다. 배치와 치수는 개략 표현이다.

## 추가 전경과 체험 보완 (2026-10-23)

- 학교전경 폴더의 사진 27장(앞서 받은 2장 포함)에서 강당 옆 목재 계단·데크·난간·벤치·유리창, 농구장 옆 오르막, 동진회관의 아치 창과 붉은 현관 차양, 교문 옆 조형물의 추상적 형태를 관찰했다. 모형은 `src/campus-rear-scene.ts`에서 새로 만들었으며 축·치수·높이·개수는 추정이다. 원본 사진과 인물·차량 식별 정보는 게시하지 않는다.
- 같은 폴더의 청학고 급식 체험 영상은 로컬 프레임으로 행동 순서만 확인했다. 영상·프레임·캐릭터·식판 에셋을 복사하거나 배포하지 않는다. `campus-meal.ts`, `campus-hand-props.ts`의 식판·음식·수저·열린 책과 학생 팔 동작은 새로 제작한 가상 체험이다. 실제 학교 식단과 책 본문을 재현하지 않는다.
- 도서관의 공용 테이블, 2층 학봉1·학봉2·난심독서실의 칸막이형 개별 좌석 구분은 사용자 확인을 반영한다. 정확한 가구 수와 위치는 개략이다.
- `public/school-share-v6.jpg`는 갱신한 모형을 `assets/campus-share-card.html`에서 렌더링해 촬영했다. 새 외부 에셋은 없다.
