# Jekyll GitHub Pages Site

이 프로젝트는 Jekyll을 사용하여 GitHub Pages에 배포되는 정적 사이트입니다.

## 로컬 개발 환경 설정

### 필요한 도구
- Ruby (2.7 이상)
- Bundler

### 설치 및 실행

1. 의존성 설치:
```bash
bundle install
```

2. 로컬 서버 실행:
```bash
bundle exec jekyll serve
```

3. 브라우저에서 `http://localhost:4000` 접속

## 사이트 구조

- `_posts/`: 블로그 포스트 파일들
- `_layouts/`: 페이지 레이아웃 템플릿
- `_includes/`: 재사용 가능한 컴포넌트
- `assets/`: CSS, JS, 이미지 등 정적 파일
- `_config.yml`: 사이트 설정 파일

## 새 포스트 작성

`_posts` 디렉토리에 `YYYY-MM-DD-title.md` 형식으로 파일을 생성하고 다음과 같이 작성:

```markdown
---
layout: post
title: "포스트 제목"
date: 2025-07-17
categories: category1 category2
---

포스트 내용을 여기에 작성하세요.
```

## GitHub Pages 배포

1. GitHub 저장소 생성
2. 코드 푸시
3. 저장소 Settings > Pages에서 Source를 "GitHub Actions"로 설정
4. 자동으로 배포됩니다

## 커스터마이징

- `_config.yml`에서 사이트 기본 정보 수정
- `assets/main.scss`에서 스타일 커스터마이징
- `_layouts/`에서 페이지 레이아웃 수정