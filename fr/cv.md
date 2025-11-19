---
layout: page
title: "Curriculum Vitae"
---

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Julien Romero",
  "jobTitle": "Maître de conférences en Intelligence Artificielle",
  "affiliation": {
    "@type": "Organization",
    "name": "Télécom SudParis",
    "parentOrganization": {
      "@type": "Organization",
      "name": "Institut Polytechnique de Paris"
    }
  },
  "email": "mailto:julien [DOT] romero [AT] telecom-sudparis [DOT] eu",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "Paris",
    "addressCountry": "FR"
  },
  "url": "{{ site.url | default: 'https://julienromero.fr' }}{{ '/fr/cv' | relative_url }}",
  "sameAs": [
    "https://linkedin.com/in/romerojulien",
    "https://github.com/Aunsiels",
    "https://gitlab.com/aunsiels",
    "https://twitter.com/Julien_romero",
    "https://huggingface.co/Aunsiels",
    "https://scholar.google.com/citations?user=nCgiv6YAAAAJ",
    "https://dblp.org/pid/241/9678.html",
    "https://orcid.org/0000-0002-7382-9077",
    "https://www.semanticscholar.org/author/Julien-Romero/119889381",
    "https://www.researchgate.net/profile/Julien_Romero",
    "https://www.wikidata.org/wiki/Q99529363"
  ]
}
</script>

<p>
  Vous pouvez télécharger une version PDF de mon CV ici :
</p>

<ul>
  <li><a href="{{ '/assets/pdf/cv-fr.pdf' | relative_url }}">Télécharger le CV (PDF, français)</a></li>
  <li><a href="{{ '/assets/pdf/cv-en.pdf' | relative_url }}">Download CV (PDF, English)</a></li>
</ul>

---

## Résumé

Chercheur en machine learning / applied scientist avec plus de 9 ans d’expérience en  
**LLMs & NLP**, **apprentissage sur graphes (GNNs)**, **information extraction**  
et **systèmes de recommandation**.  

J’ai co-développé, avec des partenaires industriels, un assistant pour recruteurs et un système de recommandation d’emploi.  
J’ai publié des travaux dépassant l’état de l’art dans des conférences telles que **EMNLP**, **ISWC** et **CIKM**.  
Je suis mainteneur open source de **Pyformlang**.  

Je suis ouvert à des collaborations et opportunités, notamment dans la région parisienne,  
où je peux transformer des méthodes de pointe en produits fiables.

---

## Expérience

### Télécom SudParis — Maître de conférences (ML / IA appliquée)  
*07/2021 – Présent · Paris, France*

- Co-développement avec un partenaire RH d’un assistant pour recruteurs et d’un système de recommandation d’emploi ; intégration dans le CRM client ; amélioration mesurable par rapport aux baselines et réduction du temps de présélection.
- Conception d’un “resume augmenter” inférant et vérifiant des compétences techniques à partir de signaux d’activité publics ; meilleure découverte de compétences latentes et meilleure précision des matches.
- Fine-tuning et évaluation de modèles de langue (Hugging Face Transformers) pour le question-answering temporel et le nettoyage de connaissances ; optimisation des prompts et de l’entraînement pour la latence et le coût.
- Encadrement d’une équipe de 3 doctorants ; gestion de deux partenariats industriels de bout en bout (cadrage → livraison) ; collaboration étroite avec les équipes d’ingénierie et produit.
- Responsable de programmes en IA à Télécom SudParis et à l’Institut Polytechnique de Paris.

---

### Max Planck Institute for Informatics — Chercheur postdoctoral  
*10/2020 – 08/2021 · Saarbrücken, Allemagne*

- Passage à l’échelle de l’extraction d’information sur de grands crawls web ; mise en place de QA sur les triplets extraits.
- Fine-tuning de LLMs pour la découverte et la validation de connaissances ; usage de signaux multimodaux pour la vérification.

---

### Télécom Paris — Doctorant (Ph.D. en Informatique)  
*09/2017 – 09/2020 · France*

- Publications dans des conférences majeures, avec un focus sur l’extraction d’information, le NLP et les méthodes sur graphes.
- Création de **Pyformlang**, une bibliothèque Python de qualité production pour la manipulation de langages formels, devenue la plus utilisée dans sa catégorie.

---

### Haufe-Umantis — Junior Data Scientist  
*01/2017 – 07/2017 · Saint-Gall, Suisse*

- Prototypage de fonctionnalités de people analytics et de systèmes de recommandation dans une suite RH.
- Présentation de solutions à des clients grands comptes (dont Daimler).

---

## Projets sélectionnés

- **Recommandation d’emploi explicable (GNN)**  
  Construction d’un graphe hétérogène à partir de CV, offres d’emploi et signaux comportementaux ; apprentissage d’un modèle de ranking basé sur des GNNs avec explications par chemins ; performances supérieures aux baselines fortes ; déploiement en POC avec un partenaire RH.

- **Génération et nettoyage de connaissances avec des LLMs**  
  Utilisation de modèles de langue pour générer et nettoyer de la connaissance, avec une meilleure précision que la curation manuelle et une réduction de la charge opérationnelle.

- **Séries temporelles financières et signaux exogènes**  
  Intégration de news et de signaux de sentiment dans des modèles de prévision ; amélioration de l’explicabilité et de la robustesse sur des jeux de données de grande taille.

---

## Open source

- **Pyformlang** — Mainteneur principal  
  Environ 53 étoiles GitHub ; ~81k téléchargements (PyPI / pypistats).  
  Largement utilisé pour la manipulation de langages formels en Python ; adopté dans des cours et des travaux de recherche.

---

## Compétences

**ML & Recherche**  
LLMs, NLP, Information Extraction, Graph Neural Networks (GNNs), systèmes de recommandation  

**Frameworks & bibliothèques**  
Python, PyTorch, Hugging Face Transformers, LangChain, vector stores  

**Data & MLOps**  
Airflow, Docker, Spark, Kafka, CI/CD, tests, monitoring, SQL / NoSQL  

**Visualisation**  
matplotlib, Plotly  

**Collaboration**  
Gestion de partenaires, mentorat, encadrement de doctorants et d’étudiants de master

---

## Formation

- **Ph.D. en Informatique** — Télécom Paris  
  *2017 – 2020*

- **M.Sc. en Informatique** — ETH Zürich  
  *2015 – 2017*

- **Diplôme d’ingénieur (Informatique)** — Télécom Paris  
  *2013 – 2015*

---

## Langues

- **Français** — langue maternelle  
- **Anglais** — courant  

---

## Contact

- 📍 Paris, France  
- ✉️ <a href="mailto:julien [DOT] romero [AT] telecom-sudparis [DOT] eu">julien [DOT] romero [AT] telecom-sudparis [DOT] eu</a>  
- LinkedIn : <https://linkedin.com/in/romerojulien>  
- GitHub : <https://github.com/Aunsiels>

