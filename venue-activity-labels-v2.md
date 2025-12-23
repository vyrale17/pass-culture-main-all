# Labels courts des activités professionnelles - V2

## Propositions finales avec recommandations

| Code | Label actuel | Proposition V2 | Statut | Recommandation |
|------|--------------|----------------|--------|----------------|
| **ART_SCHOOL** | École d'arts | **Cours d'art** / Atelier / Atelier créatif | À définir | ✅ **Cours d'art** - Plus court et clair pour les jeunes |
| **BOOKSTORE** | Librairie | Librairie | ✅ Validé | - |
| **PERFORMANCE_HALL** | Salle de spectacles | Salle de spectacle | ✅ Validé | - |
| **CREATIVE_ARTS_STORE** | Magasin d'arts créatifs | Magasin arts créatifs / **Magasin d'arts créatifs** | À définir | ✅ **Magasin d'arts créatifs** - Grammaticalement correct avec "d'" |
| **DISTRIBUTION_STORE** | Magasin culturel | Magasin culturel | ✅ Validé | - |
| **CULTURAL_CENTRE** | Centre culturel | Centre culturel | ✅ Validé | - |
| **FESTIVAL** | Festival | Festival | ✅ Validé | - |
| **GAMES_CENTRE** | Jeux vidéo | - | À définir | ✅ **Ludothèque** - Plus adapté (inclut jeux de société + jeux vidéo) |
| **LIBRARY** | Bibliothèque | **Bibliothèque** / Bibliothèque et médiathèque | À définir | ✅ **Bibliothèque** - Plus court, "médiathèque" implicite |
| **MUSEUM** | Musée | Musée | ✅ Validé | - |
| **MUSIC_INSTRUMENT_STORE** | Instruments de musique | Magasin d'instruments | ✅ Validé | - |
| **CINEMA** | Cinéma | Cinéma | ✅ Validé | - |
| **OTHER** | Autre | Autre lieu | ✅ Validé | - |
| **HERITAGE_SITE** | Patrimoine | Site patrimonial | ✅ Validé | - |
| **RECORD_STORE** | Disquaire | Disquaire | ✅ Validé | - |
| **SCIENCE_CENTRE** | Culture scientifique | Centre scientifique | ✅ Validé | - |
| **ART_GALLERY** | Galerie d'art | **Galerie d'art** | À définir | ✅ **Galerie d'art** - Parfait tel quel |
| **ARTS_CENTRE** | Centre d'arts | - | - | ✅ **Centre d'arts** - OK tel quel |
| **COMMUNITY_CENTRE** | Centre socio-culturel | - | - | ✅ **Centre socio-culturel** - OK tel quel |
| **TOURIST_INFORMATION_CENTRE** | Office de tourisme | - | - | ✅ **Office de tourisme** - OK tel quel |

---

## Détails des recommandations pour les "À définir"

### 1. ART_SCHOOL - Cours d'art ✅

**Options :**
- ❌ "Atelier" → Trop vague, peut être confondu avec un atelier ponctuel
- ❌ "Atelier créatif" → Similaire à "Magasin d'arts créatifs", risque de confusion
- ✅ **"Cours d'art"** → Clair, court, explicite (conservatoire, école de musique, danse, etc.)

**Argument :** Les jeunes comprennent immédiatement qu'il s'agit d'un lieu où on apprend (cours).

---

### 2. CREATIVE_ARTS_STORE - Magasin d'arts créatifs ✅

**Options :**
- ❌ "Magasin arts créatifs" → Manque l'article "d'" pour être grammaticalement correct
- ✅ **"Magasin d'arts créatifs"** → Correct et complet

**Argument :** Respecte les règles grammaticales françaises tout en restant court.

---

### 3. GAMES_CENTRE - Ludothèque ✅

**Options :**
- ❌ "Jeux vidéo" → Trop restrictif, exclut les jeux de société
- ❌ "Espace ludique" → Trop formel
- ✅ **"Ludothèque"** → Terme établi, reconnu, couvre tous types de jeux

**Argument :** "Ludothèque" est un terme familier pour les jeunes et inclut naturellement jeux de société, jeux vidéo, escape games, etc.

**Note :** Cette catégorie est archivée, donc moins prioritaire.

---

### 4. LIBRARY - Bibliothèque ✅

**Options :**
- ✅ **"Bibliothèque"** → Simple, universel, court
- ❌ "Bibliothèque et médiathèque" → Trop long, "médiathèque" est implicite aujourd'hui

**Argument :** Le terme "bibliothèque" englobe déjà les médiathèques dans l'usage courant des jeunes. Plus court = meilleur.

---

### 5. ART_GALLERY - Galerie d'art ✅

**Option :**
- ✅ **"Galerie d'art"** → Parfait tel quel, clair et court

**Argument :** Terme standard, pas besoin de modifier.

---

## Liste finale proposée (tous les codes)

| Code | Label V2 final recommandé |
|------|---------------------------|
| ART_GALLERY | Galerie d'art |
| ART_SCHOOL | Cours d'art |
| ARTS_CENTRE | Centre d'arts |
| BOOKSTORE | Librairie |
| CINEMA | Cinéma |
| COMMUNITY_CENTRE | Centre socio-culturel |
| CREATIVE_ARTS_STORE | Magasin d'arts créatifs |
| CULTURAL_CENTRE | Centre culturel |
| DISTRIBUTION_STORE | Magasin culturel |
| FESTIVAL | Festival |
| GAMES_CENTRE | Ludothèque |
| HERITAGE_SITE | Site patrimonial |
| LIBRARY | Bibliothèque |
| MUSEUM | Musée |
| MUSIC_INSTRUMENT_STORE | Magasin d'instruments |
| OTHER | Autre lieu |
| PERFORMANCE_HALL | Salle de spectacle |
| RECORD_STORE | Disquaire |
| SCIENCE_CENTRE | Centre scientifique |
| TOURIST_INFORMATION_CENTRE | Office de tourisme |

---

## Format TypeScript - V2

```typescript
export const VenueActivityLabelsV2 = {
  ART_GALLERY: 'Galerie d'art',
  ART_SCHOOL: 'Cours d'art',
  ARTS_CENTRE: 'Centre d'arts',
  BOOKSTORE: 'Librairie',
  CINEMA: 'Cinéma',
  COMMUNITY_CENTRE: 'Centre socio-culturel',
  CREATIVE_ARTS_STORE: 'Magasin d'arts créatifs',
  CULTURAL_CENTRE: 'Centre culturel',
  DISTRIBUTION_STORE: 'Magasin culturel',
  FESTIVAL: 'Festival',
  GAMES_CENTRE: 'Ludothèque',
  HERITAGE_SITE: 'Site patrimonial',
  LIBRARY: 'Bibliothèque',
  MUSEUM: 'Musée',
  MUSIC_INSTRUMENT_STORE: 'Magasin d'instruments',
  OTHER: 'Autre lieu',
  PERFORMANCE_HALL: 'Salle de spectacle',
  RECORD_STORE: 'Disquaire',
  SCIENCE_CENTRE: 'Centre scientifique',
  TOURIST_INFORMATION_CENTRE: 'Office de tourisme',
}
```

---

## Changements par rapport à V1

| Code | V1 | V2 | Changement |
|------|----|----|------------|
| ART_SCHOOL | École d'arts | Cours d'art | Simplifié |
| GAMES_CENTRE | Jeux vidéo | Ludothèque | Plus inclusif |
| PERFORMANCE_HALL | Salle de spectacles | Salle de spectacle | Singulier |

Tous les autres labels restent identiques ou quasi-identiques.
