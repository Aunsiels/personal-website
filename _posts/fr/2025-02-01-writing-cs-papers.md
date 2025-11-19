---
layout: post
title: "Écrire un article en informatique : quelques conseils"
lang: fr
categories: [fr, blog]
tags: [écriture, doctorat, recherche]
---

Écrire un article scientifique n’est jamais simple — et encore moins en informatique, où l’on mélange théorie, code, maths, systèmes et narration.  
Au fil des années, j’ai noté une série de conseils pratiques qui permettent de garder un article **clair**, **lisible** et **bien structuré**.  
Cet article est encore en évolution, mais j’espère qu’il sera utile aux étudiants, doctorants et collègues.

## Conseils généraux

### **1. Ne plagiez pas — citez vos sources**
Cela semble évident, mais il faut le rappeler : **ne réutilisez jamais du texte sans citation**.  
Si vous reprenez une phrase, mettez-la entre guillemets. Si vous reprenez une idée, citez la source. Les outils de détection sont aujourd’hui très performants.

### **2. Traquez les fautes et les formulations étranges**
Les fautes de grammaire, les tournures maladroites et les phrases ambiguës ralentissent la lecture — et peuvent modifier le sens.  
Je ne suis pas anglophone natif, donc j’utilise toujours un assistant d’écriture (Grammarly, LanguageTool…).  
Ils corrigent les erreurs évidentes, mais il faut toujours **relire manuellement** à la fin.

### **3. Utilisez un anglais simple**
La majorité des chercheurs ne sont pas natifs. Des phrases simples sont souvent plus claires et plus agréables à lire.

### **4. Illustrez avec des exemples**
Les exemples sont l’outil le plus efficace pour expliquer un concept complexe.  
Ils fonctionnent partout : introduction, motivation, résultats expérimentaux, limitations…  
J’aime particulièrement montrer **de vrais outputs de système**, beaucoup plus parlants que des tableaux abstraits.

### **5. Utilisez des figures lisibles et haute résolution**
Évitez les images pixelisées ou les textes minuscules.  
Privilégiez les **images vectorielles** (PDF/SVG).  
Pour les schémas, j’utilise <https://app.diagrams.net>, exporté en PDF.

### **6. Mettez les titres et sections en capitalisation correcte**
Ce n’est pas intuitif dans toutes les langues. Des outils comme https://capitalizemytitle.com/ peuvent aider.

### **7. Gardez un style cohérent**
Choisissez un style et tenez-vous-y (capitalisation, ponctuation, notation mathématique, style des figures…).

---

## Conseils LaTeX

### **1. Corrigez les erreurs et avertissements**
LaTeX n’est pas magique : s’il signale une erreur, c’est qu’il y a un problème réel.  
Lisez et corrigez les messages du compilateur immédiatement.

### **2. Séparez votre article en plusieurs fichiers**
Utilisez `\input{...}` ou `\include{...}`.  
Je mets souvent les sections (et parfois les sous-sections) dans des fichiers séparés, ainsi que les grandes tables.  
Cela rend la navigation et les modifications beaucoup plus faciles.

### **3. Structurez vos labels**
Utilisez des préfixes cohérents :
- `sec:`  
- `fig:`  
- `tab:`  
- `ch:`  

### **4. Conservez la même police dans le texte et les figures**
Un détail, mais cela donne un article beaucoup plus propre.  
La police par défaut de LaTeX (Computer Modern) est très bien.

### **5. Utilisez les guillemets LaTeX**
En LaTeX :  
- Ouverture : ````  
- Fermeture : `''`

### **6. Utilisez les espaces insécables pour les citations**
Toujours écrire `~\cite{...}` et `~\ref{...}` pour éviter que les citations flottent en début de ligne.

### **7. Rendez les liens cliquables**
Avec :

```latex
\usepackage[backref=page]{hyperref}
`````

ou

```latex
\href{http://...}{texte du lien}
```

### **8. Gardez un LaTeX brut propre**

Le `.tex` doit être lisible **sans compiler**.
Évitez les coupures étranges, les commentaires sauvages et les indentations incohérentes.
Cela facilite aussi l’usage d’un correcteur orthographique.

---

## Liens utiles

* **How to ML Paper** : [https://docs.google.com/document/d/16R1E2ExKUCP5SlXWHr-KzbVDx9DBUclra-EbU8IB-iE/edit](https://docs.google.com/document/d/16R1E2ExKUCP5SlXWHr-KzbVDx9DBUclra-EbU8IB-iE/edit)
* **LaTeX Advice** : [https://github.com/dspinellis/latex-advice](https://github.com/dspinellis/latex-advice)
* **The Writing Process** : [https://medium.com/@marcotcr/writing-part-1-the-process-6bb92cb522eb](https://medium.com/@marcotcr/writing-part-1-the-process-6bb92cb522eb)

