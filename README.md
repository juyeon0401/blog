"# 내 블로그

GitHub Pages와 Jekyll로 만든 블로그입니다.

## 시작하기

### 1. GitHub 저장소 설정

1. GitHub에서 이 저장소로 이동
2. Settings > Pages 메뉴로 이동
3. Source를 "GitHub Actions"로 선택

### 2. 블로그 설정 수정

`_config.yml` 파일을 열어서 다음 항목들을 수정하세요:

```yaml
title: 내 블로그          # 블로그 제목
description: ...         # 블로그 설명
author: juyeo           # 작성자 이름
email: your-email@...   # 이메일 주소
url: https://username.github.io  # GitHub Pages URL
```

### 3. 변경사항 GitHub에 올리기

```bash
git add .
git commit -m "블로그 설정 완료"
git push origin main
```

푸시 후 약 1-2분 뒤 GitHub Actions에서 자동으로 배포됩니다!

## 글 작성하기

### 새 글 작성 방법

1. `_posts` 폴더에 새 파일 만들기
2. 파일명 형식: `YYYY-MM-DD-제목.md`
   - 예: `2025-10-26-hello-world.md`

3. 파일 내용 작성:

```markdown
---
layout: post
title: "글 제목"
date: 2025-10-26 20:00:00 +0900
categories: 카테고리명
---

여기에 본문 내용을 작성합니다.

## 소제목

내용 작성...
```

### 마크다운 문법

```markdown
# 제목 1
## 제목 2
### 제목 3

**굵게**
*기울임*

- 목록 1
- 목록 2

[링크 텍스트](https://example.com)

![이미지 설명](이미지 URL)
```

### 글 발행하기

```bash
git add _posts/2025-10-26-새글.md
git commit -m "새 글 작성"
git push origin main
```

## 로컬에서 미리보기 (선택사항)

Ruby가 설치되어 있다면 로컬에서 블로그를 미리 볼 수 있습니다:

```bash
# 처음 한 번만 실행
bundle install

# 로컬 서버 실행
bundle exec jekyll serve

# 브라우저에서 http://localhost:4000 접속
```

## 파일 구조

```
blog/
├── _config.yml          # 블로그 설정 파일
├── _posts/              # 블로그 글 폴더
│   └── 2025-10-26-welcome.md
├── index.md             # 홈페이지
├── about.md             # 소개 페이지
├── Gemfile              # Ruby 패키지 설정
└── .github/
    └── workflows/
        └── jekyll.yml   # 자동 배포 설정
```

## 팁

1. **카테고리 사용**: `categories`에 여러 개를 넣을 수 있습니다
   ```yaml
   categories: [일상, 여행]
   ```

2. **태그 추가**:
   ```yaml
   tags: [태그1, 태그2]
   ```

3. **글 초안 작성**: `_drafts` 폴더에 날짜 없이 저장하면 발행되지 않습니다

4. **페이지 추가**: 루트 폴더에 `.md` 파일을 만들면 새 페이지가 됩니다

## 문제 해결

- 배포 상태 확인: GitHub 저장소의 "Actions" 탭 확인
- 에러가 있으면 빨간색으로 표시됨
- 로그를 클릭해서 어떤 문제인지 확인 가능

## 더 알아보기

- Jekyll 공식 문서: https://jekyllrb.com/docs/
- GitHub Pages 가이드: https://docs.github.com/pages
- Minima 테마: https://github.com/jekyll/minima" 
