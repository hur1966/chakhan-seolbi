# 착한설비 — 부산·경남 배관설비 SEO 사이트

정적 사이트 생성기. `scripts/build.py`가 `data/`의 설정·후기를 읽어 `dist/`에 모든 페이지를 자동 생성한다.

## 빌드
```
pip install -r requirements.txt
python3 scripts/build.py
```
결과물은 `dist/` 폴더. Netlify는 `netlify.toml`에 따라 빌드 후 `dist/`를 게시한다.

## 폴더 구조
- `data/config.json` — 상호·전화·서비스·지역 설정
- `data/posts/` — 후기 JSON
- `scripts/build.py` — 페이지 생성 엔진
- `assets/` — CSS, 이미지(파비콘 등)

## 아직 설정해야 할 것 (착한설비 신규)
- [ ] 도메인 구매 후 `data/config.json`의 `site.url` 채우기
- [ ] 카톡 채널 만들고 `business.kakao_url` 채우기
- [ ] 파비콘을 착한설비 로고로 교체 (`assets/img/`)
- [ ] 네이버·구글 인증 코드를 `scripts/build.py` head 부분에 추가
- [ ] 영업 지역 동 목록을 `regions`에 추가 (전화 많이 오는 곳 위주)
