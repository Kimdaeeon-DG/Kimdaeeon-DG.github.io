---
title: "GitHub 블로그 포스팅 방법 완벽 가이드"
excerpt: "Jekyll 기반 GitHub 블로그에 포스트 작성하는 방법을 알아봅시다"

categories:
  - Blog
tags:
  - [Github, Jekyll, Blog, Markdown]

permalink: /blog/github-blog-posting-guide/

toc: true
toc_sticky: true

date: 2025-01-08
last_modified_at: 2025-01-08
---

## 1. 포스트 파일 생성하기

GitHub 블로그에 새 포스트를 작성하기 위해서는 `_posts` 폴더에 새로운 마크다운 파일을 생성해야 합니다. 파일 이름은 다음과 같은 형식을 따라야 합니다:

```
YYYY-MM-DD-제목.md
```

예시: `2025-01-08-github-blog-posting-guide.md`

## 2. 포스트 머리말(Front Matter) 작성하기

모든 포스트는 YAML 형식의 머리말로 시작해야 합니다. 머리말은 `---`로 감싸며, 다음과 같은 정보를 포함합니다:

```yaml
---
title: "포스트 제목"
excerpt: "포스트 요약"
categories: 
  - 카테고리명
tags:
  - [태그1, 태그2]
date: YYYY-MM-DD
last_modified_at: YYYY-MM-DD
---
```

## 3. 마크다운 문법으로 본문 작성하기

### 3.1 기본 문법

```markdown
# 제목 1
## 제목 2
### 제목 3

- 목록 1
- 목록 2
  - 하위 목록

1. 순서 있는 목록
2. 순서 있는 목록

**굵게** 또는 *기울임*
```

### 3.2 코드 블록 사용하기

````markdown
```python
def hello_world():
    print("Hello, World!")
```
````

### 3.3 이미지 삽입하기

```markdown
![이미지 설명](/assets/images/example.jpg)
```

## 4. 포스트 미리보기

로컬에서 포스트를 미리보기 하려면 다음 명령어를 실행합니다:

```bash
bundle exec jekyll serve
```

그러면 `http://localhost:4000`에서 블로그를 확인할 수 있습니다.

## 5. 포스트 업로드하기

작성한 포스트를 GitHub에 업로드하려면 다음 git 명령어를 사용합니다:

```bash
git add .
git commit -m "Add new post: 제목"
git push origin main
```

## 6. 유용한 팁

1. 이미지는 `assets/images/` 폴더에 저장하는 것이 좋습니다.
2. 카테고리와 태그는 일관성 있게 사용하세요.
3. 포스트 미리보기 텍스트는 excerpt에 명확하게 작성하세요.
4. 날짜는 미래 날짜를 사용하지 마세요.

이렇게 하면 깔끔하고 체계적인 블로그 포스트를 작성할 수 있습니다. 실제로 포스트를 작성할 때 이 가이드를 참고하시면 도움이 될 것입니다!
