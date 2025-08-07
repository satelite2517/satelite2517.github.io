
# ✨ HTML & CSS 핵심 문법 요약 (깃헙 페이지 제작용)

> **간단한 소개용 웹페이지 (예: 자기소개, 이력서, 프로젝트 소개)** 만들 때 꼭 알아야 할 HTML + CSS 핵심만 정리한 문서입니다.

---

## 📄 1. HTML 기본 구조

```html
<!DOCTYPE html>
<html>
  <head>
    <title>페이지 제목</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <!-- 여기에 본문 -->
  </body>
</html>
```

---

## 🔡 2. 텍스트 관련

```html
<h1>큰 제목</h1>
<p>이건 문단</p>
줄1<br>줄2
<strong>중요</strong>
<code>x = 3</code>
<hr>
```

---

## 🔗 3. 링크 & PDF 열기

```html
<a href="https://google.com" target="_blank">구글 열기</a>
<a href="files/my_resume.pdf" target="_blank">📄 이력서 보기</a>
```

---

## 🖼 4. 이미지 넣기

```html
<img src="images/me.jpg" alt="나" width="150" style="border-radius: 50%;">
```

---

## 📋 5. 목록 (리스트)

```html
<ul>
  <li>사과</li>
  <li>바나나</li>
</ul>

<ol>
  <li>첫 번째</li>
  <li>두 번째</li>
</ol>
```

---

## 📐 6. 레이아웃 태그

```html
<header>상단</header>
<nav>메뉴</nav>
<main>내용</main>
<section>섹션</section>
<footer>하단</footer>
```

---

## 💅 7. CSS 기본 문법

```css
선택자 {
  속성: 값;
}

예:
color: red;
font-size: 20px;
text-align: center;
```

---

## 🎨 8. CSS 예시

```css
body {
  font-family: sans-serif;
  background-color: #f9f9f9;
}

img.profile {
  width: 150px;
  border-radius: 50%;
  box-shadow: 0 0 10px rgba(0,0,0,0.2);
}
```

---

## 🧭 9. 가운데 정렬 방법

### 텍스트
```html
<p style="text-align: center;">문장 가운데</p>
```

### 이미지
```html
<img src="me.jpg" style="display: block; margin: auto;" width="200">
```

### div 박스
```html
<div style="width: 300px; margin: 0 auto;">내용</div>
```

### 화면 정중앙 (flex)
```html
<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;">
  <div>정중앙!</div>
</div>
```

---

## 💠 10. 아이콘 (예: CV / ORCID / GitHub 등)

- **Font Awesome CDN 추가** (HTML `<head>`에 아래 추가)

```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
```

- **사용 예시**

```html
<!-- 아이콘 + 링크 -->
<p>
  <a href="https://orcid.org/0000-0001-2345-6789" target="_blank">
    <i class="fa-brands fa-orcid"></i> ORCID
  </a>
</p>

<p>
  <a href="files/CV.pdf" target="_blank">
    <i class="fa-solid fa-file-pdf"></i> Download CV
  </a>
</p>

<p>
  <a href="https://github.com/yourusername" target="_blank">
    <i class="fa-brands fa-github"></i> GitHub
  </a>
</p>
```

---

## 🗂 11. Projects 섹션 만들기

```html
<section id="projects">
  <h2>Projects</h2>
  <ul>
    <li><strong>Smart Cane</strong> — Arduino, Flutter, GPS</li>
    <li><strong>Plasma Visualization</strong> — Python + Julia</li>
    <li><a href="https://github.com/yourusername/project1" target="_blank">GitHub Project</a></li>
  </ul>
</section>
```

---

## 📦 폴더 구조 예시

```
my-website/
├── index.html
├── styles.css
├── images/
│   └── me.jpg
├── files/
│   └── CV.pdf
```

---

## ✅ 요약 슬로건

> **HTML은 구조, CSS는 꾸밈**  
> `<태그>`로 구성하고 `style` 또는 `class`로 꾸민다.
