# KGM × LG CNS · Gemini Enterprise 1시간 교육 패키지

2주 파일럿 사용 데이터를 기반으로 만든 **1시간 콘솔 시연 교육**용 문서 2종입니다. 진행자 멘트와 사용자 배포본이 **별도 파일로 분리**되어 있습니다.

- **사용자 핸즈온 가이드 (`index.html`)** — 사용자에게 공유하는 배포본. 진행자 멘트는 빠져 있고, 콘솔 위치 안내 · Before/After · 복사용 프롬프트 · '이런 결과가 나와요' 효능감 포인트로 구성. 교육 후 그대로 링크로 전달.

구성: Intro(사용 현황) → Level 1 일상 업무 자동화 → Level 2 콘텐츠 생성·가공 → Level 3 나만의 AI 비서 → Wrap-up. 두 문서는 같은 순서이므로, 사용자 가이드를 화면에 띄우고 멘트 스크립트대로 진행하면 됩니다.

## 구성

| 파일 | 용도 | 공유 |
|------|------|------|
| `index.html` | 사용자 핸즈온 가이드 (배포본) | ✅ 사용자에게 공유 |
| `facilitator-script.html` | 진행자 멘트 스크립트 | ⛔ 진행자 전용 |
| `.nojekyll` | GitHub Pages 서빙용 빈 파일 | — |
| `README.md` | 이 문서 | — |

## 미리보기 (배포 없이 바로 보기)

각 `.html`을 더블클릭해 브라우저로 열면 그대로 보입니다. 배포는 링크로 공유할 때만 필요합니다.

## ⚠ 진행자 스크립트 공유 주의

`facilitator-script.html`을 같은 public repo에 올리면 URL을 아는 사람은 접근할 수 있습니다(검색 노출은 안 되지만 비공개는 아님). 멘트 노출이 부담되면 **이 파일은 업로드하지 말고 로컬에서만** 사용하고, `index.html`만 배포하세요.

## GitHub Pages 배포 (1~2분)

### 방법 A — 웹에서 (가장 쉬움, 터미널 불필요)

1. GitHub 로그인 → 우측 상단 **+** → **New repository**
2. Repository name 예: `gemini-enterprise-facilitator` → **Public** 선택 → **Create repository**
3. 새 repo 화면에서 **uploading an existing file** 클릭
4. `index.html` · `.nojekyll` · `README.md` 를 드래그해 업로드 → **Commit changes**
   - `.nojekyll`이 안 보이면 숨김 파일이라 그렇습니다. 업로드 창에서 직접 끌어다 놓으면 올라갑니다.
5. 상단 **Settings → Pages**
6. **Source** = `Deploy from a branch`, **Branch** = `main` / `/(root)` → **Save**
7. 1~2분 뒤 `https://<사용자명>.github.io/gemini-enterprise-facilitator/` 에서 열립니다.

### 방법 B — 터미널 (git)

```bash
# 이 폴더에서 실행
git init
git add index.html .nojekyll README.md
git commit -m "Add Gemini Enterprise facilitator guide"
git branch -M main
git remote add origin https://github.com/<사용자명>/gemini-enterprise-facilitator.git
git push -u origin main
```

이후 **Settings → Pages**에서 Branch = `main` / `/(root)` → Save (방법 A의 5~7단계와 동일).

### 사용자/조직 사이트로 쓰려면

repo 이름을 `<사용자명>.github.io` 로 만들면 경로 없이 `https://<사용자명>.github.io/` 로 바로 열립니다.

## 메모

- 내부 교육 자료입니다. 공개 repo로 올릴 경우 사내 민감정보가 본문에 없는지 확인하세요. 비공개로 두려면 GitHub Pages는 유료(Pro/조직) 플랜이 필요하거나, 사내 호스팅을 권장합니다.
- 내용 수정은 `index.html`만 편집하면 됩니다.

---
KG MOBILITY × LG CNS · Google Cloud팀 · CONFIDENTIAL
# ge-handson-guide
