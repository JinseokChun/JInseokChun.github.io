# JinseokChun.github.io

Jinseok Chun의 개인 홈페이지 — https://jinseokchun.github.io

[al-folio](https://github.com/alshedivat/al-folio)로 만들었고, `master`에 push하면 GitHub Actions(`.github/workflows/pages-deploy.yml`)가 빌드해서 GitHub Pages에 배포합니다.

## 어디를 고치면 되나요?

| 바꾸고 싶은 것 | 파일 |
| --- | --- |
| 이름, 사이트 설명, 기능 켜고 끄기 | `_config.yml` |
| 메인 소개글 | `_pages/about.md` |
| 프로필 사진 | `assets/img/prof_pic.jpg` |
| 블로그 글 | `_posts/YYYY-MM-DD-제목.md` |
| 프로젝트 | `_projects/*.md` |
| 소식(news) | `_news/*.md` |
| 연락처·SNS 아이콘 | `_data/socials.yml` |
| Repositories 페이지에 보일 저장소 | `_data/repositories.yml` |

## 로컬에서 미리 보기

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000
```
