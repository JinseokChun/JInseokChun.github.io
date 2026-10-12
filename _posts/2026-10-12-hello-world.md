---
title: 블로그를 시작합니다
date: 2026-10-12 09:00:00 +0900
categories: [Blog]
tags: [시작]
---

안녕하세요! 공부한 내용을 끄적끄적 기록하는 블로그입니다.

## 새 글 쓰는 법

1. `_posts`{: .filepath } 폴더에 `YYYY-MM-DD-제목.md`{: .filepath } 형식으로 파일을 만듭니다.
2. 파일 맨 위에 아래와 같은 머리말(Front Matter)을 적습니다.

   ```yaml
   ---
   title: 글 제목
   date: 2026-10-12 12:00:00 +0900
   categories: [대분류, 소분류]
   tags: [태그1, 태그2]
   ---
   ```

3. 그 아래에 마크다운으로 본문을 작성하고 `master` 브랜치에 커밋하면, 몇 분 뒤 자동으로 블로그에 반영됩니다.

> 수식이 필요하면 머리말에 `math: true`, 다이어그램이 필요하면 `mermaid: true`를 추가하세요.
{: .prompt-tip }
