# JinseokChun.github.io

Jinseok Chun의 개인 홈페이지 — https://jinseokchun.github.io

[al-folio](https://github.com/alshedivat/al-folio)로 만들었고, `master`에 push하면 GitHub Actions(`.github/workflows/pages-deploy.yml`)가 빌드해서 GitHub Pages에 배포합니다.

## 어디를 고치면 되나요?

| 바꾸고 싶은 것 | 파일 |
| --- | --- |
| 이름, 사이트 설명, 기능 켜고 끄기 | `_config.yml` |
| 메인 소개글 | `_pages/about.md` |
| 프로필 사진 | `assets/img/prof_pic.jpg` |
| 논문 목록 (Publications) | `_bibliography/papers.bib` (BibTeX 형식, `selected={true}`를 붙이면 첫 화면에도 표시 → `_pages/about.md`의 `selected_papers: true`) |
| 색상·글꼴 | `assets/css/main.scss` 맨 아래 "Site customizations" 부분 |
| 프로젝트 | `_projects/*.md` (카드 이미지는 `assets/img/projects/`) |
| 이력서 (CV) | `assets/pdf/Jinseok_Chun_CV.pdf` 교체 후 미리보기 이미지 다시 만들기: `pdftoppm -r 200 -png -singlefile assets/pdf/Jinseok_Chun_CV.pdf assets/img/cv/cv-page-1` |
| 소식(news) | `_news/YYYY-MM-DD-title.md` (첫 화면에는 "월 연도"로 표시) |
| 연락처·SNS 아이콘 | `_data/socials.yml` |

## 로컬에서 미리 보기

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000
```
