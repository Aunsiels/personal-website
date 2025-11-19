---
layout: post
title: "Writing Computer Science Papers: A Few (Updated) Tips"
lang: en
categories: [en, blog]
tags: [writing, phd, research]
---

Writing a paper is rarely easy, especially in computer science, where we mix theory, code, mathematics, and systems into a single narrative. Over the years, I collected a series of practical tips that help keep papers clean, readable, and publishable.  
This article is still evolving, but I hope it can be useful to students, colleagues, and anyone writing technical articles.

## General Tips

### **1. Don’t plagiarize — cite properly**
It should go without saying, but it must be said: **never reuse text from papers or books without citation**.  
If you quote something, use quotation marks. If you reuse an idea or structure, cite the source. Academic publishing has become extremely good at detecting plagiarism.

### **2. Fight typos and strange sentences**
Typos and awkward constructions interrupt reading flow and sometimes even change the meaning of a sentence.  
I am not a native English speaker, so I always run my drafts through a writing assistant (Grammarly, LanguageTool, ChatGPT, ...). They catch the obvious issues and sometimes offer improvements.  
But never auto-apply everything and always do a final manual proofreading.

### **3. Use simple English**
Many researchers are non-native speakers. Simple sentences tend to be clearer, shorter, and harder to misinterpret. You don’t need fancy words.

### **4. Use examples generously**
Examples are the best tools to explain a complex concept. They work everywhere: in the introduction, in the motivation, in the experimental section, and even when presenting limitations.  
I especially like showing **actual system outputs**, because they make your contributions concrete and much less abstract than tables of numbers.

### **5. Use high-resolution, readable figures**
Pixelated or tiny-font diagrams ruin an otherwise good paper.  
Whenever possible, use **vector images** (PDF/SVG).  
For diagrams, I like <https://app.diagrams.net>. I export as PDF, crop them, and embed them directly in LaTeX.

### **6. Capitalize titles and section names**
This is not always intuitive, especially if your native language does not use title case. Tools like https://capitalizemytitle.com/ can help.

### **7. Keep a consistent style**
Small inconsistencies (capitalization, punctuation, variable naming, plot style, ...) quickly add friction to the reading experience.  
Pick a style and stick to it.

---

## LaTeX Tips

### **1. Fix errors and warnings**
LaTeX is powerful but not magical. If it raises an error or a warning, it is usually trying to tell you something important.  
Always look at the compilation log and fix issues as soon as they appear.

### **2. Split your paper into multiple files**
Use `\input{...}` or `\include{...}` to organize your content.  
I often put sections (and sometimes subsections) in separate files, and I isolate big tables into their own files. Then, I put sections, tables, and images in different directories. This makes it much easier to navigate your paper and make clean modifications.

### **3. Structure your references (labels)**
Use consistent prefixes for labels:
- `sec:` for sections  
- `fig:` for figures  
- `tab:` for tables  
- `ch:` for chapters  

This makes cross-referencing much easier.

### **4. Use the same font in your text and your figures**
It’s a small detail, but it makes your paper look more polished. The LaTeX default (Computer Modern) is perfectly fine.

### **5. Use the proper quotation marks**
Avoid using the default keyboard double quote `"`.  
In LaTeX:  
- Opening quotes: ````  
- Closing quotes: `''`

### **6. Use non-breaking spaces for citations**
Always write `~\cite{...}` and `~\ref{...}` to prevent citations and numbers from drifting to the next line.

### **7. Make your links clickable**
Use:

```latex
\usepackage[backref=page]{hyperref}
```

and/or

```latex
\href{http://...}{link text}
```

It helps readers and reviewers enormously.

### **8. Write clean raw LaTeX**

Your `.tex` files should be readable without compiling.
Avoid breaking sentences in strange places, avoid over-commenting, and try to keep an indentation that reflects structure.
This also makes spell-checking much easier.

---

## Useful Links

* **How to ML Paper — A brief guide**: [https://docs.google.com/document/d/16R1E2ExKUCP5SlXWHr-KzbVDx9DBUclra-EbU8IB-iE/edit](https://docs.google.com/document/d/16R1E2ExKUCP5SlXWHr-KzbVDx9DBUclra-EbU8IB-iE/edit)
* **LaTeX Advice (excellent repo)**: [https://github.com/dspinellis/latex-advice](https://github.com/dspinellis/latex-advice)
* **The Writing Process**: [https://medium.com/@marcotcr/writing-part-1-the-process-6bb92cb522eb](https://medium.com/@marcotcr/writing-part-1-the-process-6bb92cb522eb)
