# Isa-Web — Site Isabelle, Thérapeute Chartreuse

Site statique one-page pour **Isabelle**, psychopraticienne et thérapeute systémique.  
Déployé sur **Vercel** via GitHub (`Fnarck/isa-web`).

---

## Accès rapide

| Élément | Valeur |
|---------|--------|
| URL principale | https://therapeutechartreuse.fr |
| URL secondaire | https://therapiechartreuse.fr (redirige vers principale) |
| Repo GitHub | https://github.com/Fnarck/isa-web |
| Vercel project | `isa-web` (compte `fnarcks-projects`) |
| Google Search Console | Vérifié sur `therapeutechartreuse.fr` |
| Formulaire de contact | Web3Forms (`2db2cbbd-932e-4642-becd-9e4546409512`) → `contact@therapeutechartreuse.fr` |

---

## Stack

- HTML statique + CSS vanilla (thèmes : blanc / sauge / lin)
- Assets dans `assets/` (images JPG/PNG)
- Déploiement continu : `git push main` → Vercel déploie automatiquement

---

## Structure des fichiers

```
index.html                          # Site complet (one-page)
assets/
  isabelle-about.jpg                # Photo section "Qui suis-je"
  image-000.jpg                     # Photo hero
  image-001.jpg                     # Photo cabinet
  image-002.png / image-003.png     # Illustrations
  image-004.jpg                     # Photo parent-enfant
  photo-couple.jpg                  # Photo thérapie couple
sitemap.xml                         # Sitemap Google
robots.txt                          # Ouvert à tous crawlers + déclaration sitemap
llms.txt                            # Fiche synthèse pour crawlers IA (Perplexity, ChatGPT…)
vercel.json                         # Config Vercel + redirects 301
googled62d852b54ba370c.html         # Fichier de vérification Google Search Console
```

---

## Ce qui a été fait (mai 2026)

### Contenu & Design
- Site one-page complet : Hero, Mon Approche, Mes Accompagnements, Qui suis-je, Tarifs & Contact
- 3 thèmes de couleur (blanc / sauge / lin) switchables en live
- Photo Isabelle mise à jour dans la section "Qui suis-je" (mai 2026)
- Ligne de spécialités ajoutée sous le titre hero : *Thérapie de couple · Thérapie familiale*
- Formulaire de contact Web3Forms (envoi vers `contact@therapeutechartreuse.fr`)

### SEO technique
- `<title>` géolocalisé, `<meta description>` complète
- Open Graph (Facebook/LinkedIn) + Twitter Card avec image
- Schema.org JSON-LD (`HealthAndBeautyBusiness`) : adresse, géo, tarifs, services, `sameAs`
- Canonical pointant sur `https://therapeutechartreuse.fr`
- `sitemap.xml` soumis dans Google Search Console (1 URL, statut : succès)
- `robots.txt` ouvert à tous les crawlers y compris IA
- `llms.txt` créé pour visibilité dans les moteurs IA
- Redirect 301 `therapiechartreuse.fr` → `therapeutechartreuse.fr` (via `vercel.json`)
- URLs visibles en texte dans le footer (indexation textuelle par Google)
- Google Search Console vérifié + sitemap soumis (12 mai 2026)

---

## Recommandations SEO — Actions restant à faire par Isabelle

### Priorité 1 — Google Business Profile ⭐
**Gratuit — Impact maximal sur la recherche locale**

Crée une fiche sur [business.google.com](https://business.google.com) :
- Nom : *Isabelle – Thérapeute Chartreuse*
- Adresse : Saint-Étienne-de-Crossey, Isère
- Téléphone, horaires, site web : `https://therapeutechartreuse.fr`
- Demander à des patients/proches de laisser un avis Google

→ Apparaître dans Google Maps et le bloc local "résultats à proximité".

### Priorité 2 — Annuaires spécialisés (backlinks gratuits)

Inscription gratuite sur ces annuaires, avec lien vers `https://therapeutechartreuse.fr` :

| Annuaire | URL |
|----------|-----|
| Pages Jaunes | pagesjaunes.fr |
| Annuaire Thérapeutes | annuaire-therapeutes.com |
| Thérapeutes.com | therapeutes.com |
| Synapse-fr | synapse-fr.com |

### Priorité 3 — Bing Webmaster Tools
Même démarche que Google Search Console, pour couvrir Bing et DuckDuckGo.  
→ [bing.com/webmasters](https://bing.com/webmasters)

### Sur Doctolib
- **Pour** : visibilité locale immédiate, agenda en ligne, patients habitués à la plateforme
- **Contre** : ~130–160 €/mois, éligibilité du titre "psychopraticienne" à vérifier au préalable
- **Décision** : à évaluer selon le rythme de remplissage du cabinet et le réseau de prescripteurs existant

---

## Workflow de mise à jour

```bash
# 1. Modifier index.html (ou autre fichier)
# 2. Commit + push → Vercel déploie automatiquement
cd /Users/franck/.gemini/antigravity/scratch/Isa-Web
git add <fichier>
git commit -m "feat(scope): description en anglais"
git push
```

> ⚠️ Toujours vérifier le déploiement sur https://therapeutechartreuse.fr après le push.

---

## Historique des versions principales

| Commit | Description |
|--------|-------------|
| `0c964bb` | Fichier vérification Google Search Console |
| `751ae7a` | Redirect 301, llms.txt, sameAs, URLs footer |
| `8ada013` | Spécialités ajoutées dans le hero |
| `94c5c9f` | Nouvelle photo Isabelle (section Qui suis-je) |
| `dba9f63` | SEO complet : robots, sitemap, OG, JSON-LD |
| `e2513a0` | Activation Web3Forms |
| `a251bca` | Switch domaine → therapeutechartreuse.fr |
| `c42e118` | Initialisation du projet |
