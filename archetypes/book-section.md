---
title: "Part {{ if (ne .Name "post") }}{{ .Name }}{{ else }}{{ index (split .File.ContentBaseName "-") 1 }}{{ end }}: {{ replace (replaceRE "^part-\\d+-" "" .File.ContentBaseName) "-" " " | title }}"
date: {{ .Date }}
featured_image: "/images/old-man-sea.jpg"
description: ""
book: ""
author: ""
part: {{ if (ne .Name "post") }}{{ .Name }}{{ else }}{{ index (split .File.ContentBaseName "-") 1 }}{{ end }}
tags: ["hemingway"]
draft: true
---

# Part {{ if (ne .Name "post") }}{{ .Name }}{{ else }}{{ index (split .File.ContentBaseName "-") 1 }}{{ end }}: {{ replace (replaceRE "^part-\\d+-" "" .File.ContentBaseName) "-" " " | title }}

*By Ernest Hemingway*

**Bilingual Reading for Solomon, Christian, Miriam, and Shiloh**

---

## Table of Contents

- [Section 1 (Lines 1-X)](#section-1-lines-1-x)
- [Section 2 (Lines X-X)](#section-2-lines-x-x)
<!-- Add more sections as needed -->

---

## Section 1 (Lines 1-X) <a name="section-1-lines-1-x"></a>

1. **English:** [English text goes here]  
   **Español:** [Spanish text goes here]

2. **English:** [English text goes here]  
   **Español:** [Spanish text goes here]

[Back to TOC](#table-of-contents)

---

## Section 2 (Lines X-X) <a name="section-2-lines-x-x"></a>

X. **English:** [English text goes here]  
   **Español:** [Spanish text goes here]

X. **English:** [English text goes here]  
   **Español:** [Spanish text goes here]

[Back to TOC](#table-of-contents)