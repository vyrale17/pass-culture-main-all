# Descriptions des activités professionnelles - Pass Culture

## Descriptions adaptées pour le public jeune

Ces descriptions courtes et compréhensibles peuvent être utilisées dans le frontend pour aider les jeunes à comprendre le type d'activité de chaque lieu culturel.

---

### ART_GALLERY (Galerie d'art)
**Description courte :** Des expositions d'œuvres d'art contemporain, peintures, sculptures et photos que tu peux venir découvrir.

**Exemples :** Galeries d'art, espaces d'exposition

---

### ART_SCHOOL (Conservatoire ou école d'arts)
**Description courte :** Un lieu pour apprendre et pratiquer les arts : musique, danse, théâtre, dessin, peinture...

**Exemples :** Conservatoires, écoles de musique, écoles de danse, ateliers artistiques

---

### ARTS_CENTRE (Centre d'arts)
**Description courte :** Un espace dédié à la création artistique avec des expos, des ateliers et des rencontres avec des artistes.

**Exemples :** Centres d'art contemporain, friches artistiques

---

### BOOKSTORE (Librairie)
**Description courte :** Ton point de vente de livres préféré : romans, BD, mangas, essais... et parfois des rencontres d'auteurs !

**Exemples :** Librairies indépendantes, librairies BD/mangas

---

### CINEMA (Cinéma)
**Description courte :** La salle où tu viens regarder les derniers films, classiques ou avant-première sur grand écran.

**Exemples :** Multiplexes, cinémas indépendants, cinémas d'art et d'essai

---

### COMMUNITY_CENTRE (Centre socio-culturel)
**Description courte :** Un lieu de vie de quartier qui propose des activités culturelles, sportives et des événements pour tous.

**Exemples :** Maisons de quartier, MJC (Maisons des Jeunes et de la Culture)

---

### CREATIVE_ARTS_STORE (Magasin d'arts créatifs)
**Description courte :** Le paradis des créatifs : matériel de dessin, peinture, loisirs créatifs et tout pour tes projets DIY.

**Exemples :** Magasins de fournitures artistiques, boutiques de loisirs créatifs

---

### CULTURAL_CENTRE (Centre culturel pluridisciplinaire)
**Description courte :** Un lieu qui mélange tout : spectacles, concerts, expos, cinéma, ateliers... Il y en a pour tous les goûts !

**Exemples :** Scènes nationales, centres culturels municipaux, Maisons de la Culture

---

### DISTRIBUTION_STORE (Magasin de distribution de produits culturels)
**Description courte :** Un grand magasin où tu trouves livres, musique, films, jeux vidéo et produits culturels divers.

**Exemples :** Fnac, grandes surfaces culturelles

---

### FESTIVAL (Festival)
**Description courte :** Un événement culturel temporaire : concerts, spectacles, projections... concentrés sur quelques jours !

**Exemples :** Festivals de musique, festivals de cinéma, festivals de théâtre

---

### GAMES_CENTRE (Espace ludique) [ARCHIVÉ]
**Description courte :** Un lieu pour jouer : jeux vidéo, jeux de société, escape games... Solo ou entre potes !

**Exemples :** Salles d'arcade, bars à jeux, escape games

**Note :** Cette catégorie est archivée et n'est plus utilisée pour les nouvelles structures.

---

### HERITAGE_SITE (Site patrimonial, historique ou touristique)
**Description courte :** Des monuments, châteaux, sites historiques ou naturels à visiter pour découvrir l'histoire et le patrimoine.

**Exemples :** Châteaux, monuments historiques, sites archéologiques, parcs naturels

---

### LIBRARY (Bibliothèque ou médiathèque)
**Description courte :** Un espace pour emprunter des livres, BD, magazines, films, musique... et parfois assister à des événements gratuits.

**Exemples :** Bibliothèques municipales, médiathèques

---

### MUSEUM (Musée)
**Description courte :** Des collections permanentes et des expositions temporaires pour explorer l'art, l'histoire, les sciences...

**Exemples :** Musées d'art, musées d'histoire, musées de sciences

---

### MUSIC_INSTRUMENT_STORE (Magasin d'instruments de musique)
**Description courte :** Le magasin spécialisé pour acheter, louer ou réparer ton instrument de musique préféré.

**Exemples :** Magasins d'instruments, lutherie

---

### OTHER (Autre)
**Description courte :** Un lieu culturel qui ne rentre pas dans les autres catégories mais qui propose des activités culturelles.

---

### PERFORMANCE_HALL (Salle de spectacles)
**Description courte :** Une salle pour assister à des concerts, pièces de théâtre, spectacles de danse, one-man-shows...

**Exemples :** Salles de concert, théâtres, Zéniths, salles de spectacle

---

### RECORD_STORE (Disquaire)
**Description courte :** La boutique spécialisée en musique : vinyles, CD, merchandising... et de bons conseils pour découvrir de nouveaux sons !

**Exemples :** Disquaires indépendants, magasins de vinyles

---

### SCIENCE_CENTRE (Centre de culture scientifique, technique et industrielle)
**Description courte :** Un lieu pour explorer les sciences et les technologies de façon interactive et ludique : expos, ateliers, planétarium...

**Exemples :** Cité des Sciences, planétariums, centres de culture scientifique

---

### TOURIST_INFORMATION_CENTRE (Office de tourisme)
**Description courte :** Le point info pour découvrir les activités culturelles et touristiques de ta région.

**Exemples :** Offices de tourisme, syndicats d'initiative

---

## Format pour intégration frontend

### TypeScript / JSON

```typescript
export const VenueActivityDescriptions = {
  ART_GALLERY: "Des expositions d'œuvres d'art contemporain, peintures, sculptures et photos que tu peux venir découvrir.",
  ART_SCHOOL: "Un lieu pour apprendre et pratiquer les arts : musique, danse, théâtre, dessin, peinture...",
  ARTS_CENTRE: "Un espace dédié à la création artistique avec des expos, des ateliers et des rencontres avec des artistes.",
  BOOKSTORE: "Ton point de vente de livres préféré : romans, BD, mangas, essais... et parfois des rencontres d'auteurs !",
  CINEMA: "La salle où tu viens regarder les derniers films, classiques ou avant-première sur grand écran.",
  COMMUNITY_CENTRE: "Un lieu de vie de quartier qui propose des activités culturelles, sportives et des événements pour tous.",
  CREATIVE_ARTS_STORE: "Le paradis des créatifs : matériel de dessin, peinture, loisirs créatifs et tout pour tes projets DIY.",
  CULTURAL_CENTRE: "Un lieu qui mélange tout : spectacles, concerts, expos, cinéma, ateliers... Il y en a pour tous les goûts !",
  DISTRIBUTION_STORE: "Un grand magasin où tu trouves livres, musique, films, jeux vidéo et produits culturels divers.",
  FESTIVAL: "Un événement culturel temporaire : concerts, spectacles, projections... concentrés sur quelques jours !",
  GAMES_CENTRE: "Un lieu pour jouer : jeux vidéo, jeux de société, escape games... Solo ou entre potes !",
  HERITAGE_SITE: "Des monuments, châteaux, sites historiques ou naturels à visiter pour découvrir l'histoire et le patrimoine.",
  LIBRARY: "Un espace pour emprunter des livres, BD, magazines, films, musique... et parfois assister à des événements gratuits.",
  MUSEUM: "Des collections permanentes et des expositions temporaires pour explorer l'art, l'histoire, les sciences...",
  MUSIC_INSTRUMENT_STORE: "Le magasin spécialisé pour acheter, louer ou réparer ton instrument de musique préféré.",
  OTHER: "Un lieu culturel qui ne rentre pas dans les autres catégories mais qui propose des activités culturelles.",
  PERFORMANCE_HALL: "Une salle pour assister à des concerts, pièces de théâtre, spectacles de danse, one-man-shows...",
  RECORD_STORE: "La boutique spécialisée en musique : vinyles, CD, merchandising... et de bons conseils pour découvrir de nouveaux sons !",
  SCIENCE_CENTRE: "Un lieu pour explorer les sciences et les technologies de façon interactive et ludique : expos, ateliers, planétarium...",
  TOURIST_INFORMATION_CENTRE: "Le point info pour découvrir les activités culturelles et touristiques de ta région.",
}
```

### Python / API

```python
VENUE_ACTIVITY_DESCRIPTIONS = {
    Activity.ART_GALLERY: "Des expositions d'œuvres d'art contemporain, peintures, sculptures et photos que tu peux venir découvrir.",
    Activity.ART_SCHOOL: "Un lieu pour apprendre et pratiquer les arts : musique, danse, théâtre, dessin, peinture...",
    Activity.ARTS_CENTRE: "Un espace dédié à la création artistique avec des expos, des ateliers et des rencontres avec des artistes.",
    Activity.BOOKSTORE: "Ton point de vente de livres préféré : romans, BD, mangas, essais... et parfois des rencontres d'auteurs !",
    Activity.CINEMA: "La salle où tu viens regarder les derniers films, classiques ou avant-première sur grand écran.",
    Activity.COMMUNITY_CENTRE: "Un lieu de vie de quartier qui propose des activités culturelles, sportives et des événements pour tous.",
    Activity.CREATIVE_ARTS_STORE: "Le paradis des créatifs : matériel de dessin, peinture, loisirs créatifs et tout pour tes projets DIY.",
    Activity.CULTURAL_CENTRE: "Un lieu qui mélange tout : spectacles, concerts, expos, cinéma, ateliers... Il y en a pour tous les goûts !",
    Activity.DISTRIBUTION_STORE: "Un grand magasin où tu trouves livres, musique, films, jeux vidéo et produits culturels divers.",
    Activity.FESTIVAL: "Un événement culturel temporaire : concerts, spectacles, projections... concentrés sur quelques jours !",
    Activity.GAMES_CENTRE: "Un lieu pour jouer : jeux vidéo, jeux de société, escape games... Solo ou entre potes !",
    Activity.HERITAGE_SITE: "Des monuments, châteaux, sites historiques ou naturels à visiter pour découvrir l'histoire et le patrimoine.",
    Activity.LIBRARY: "Un espace pour emprunter des livres, BD, magazines, films, musique... et parfois assister à des événements gratuits.",
    Activity.MUSEUM: "Des collections permanentes et des expositions temporaires pour explorer l'art, l'histoire, les sciences...",
    Activity.MUSIC_INSTRUMENT_STORE: "Le magasin spécialisé pour acheter, louer ou réparer ton instrument de musique préféré.",
    Activity.OTHER: "Un lieu culturel qui ne rentre pas dans les autres catégories mais qui propose des activités culturelles.",
    Activity.PERFORMANCE_HALL: "Une salle pour assister à des concerts, pièces de théâtre, spectacles de danse, one-man-shows...",
    Activity.RECORD_STORE: "La boutique spécialisée en musique : vinyles, CD, merchandising... et de bons conseils pour découvrir de nouveaux sons !",
    Activity.SCIENCE_CENTRE: "Un lieu pour explorer les sciences et les technologies de façon interactive et ludique : expos, ateliers, planétarium...",
    Activity.TOURIST_INFORMATION_CENTRE: "Le point info pour découvrir les activités culturelles et touristiques de ta région.",
}
```

---

## Notes d'utilisation

- **Ton** : Utilisation du tutoiement pour parler directement aux jeunes
- **Vocabulaire** : Simple, accessible, parfois un peu informel (DIY, potes, sons...)
- **Longueur** : 1-2 phrases maximum pour rester concis
- **Exemples** : Ajout de références concrètes que les jeunes connaissent (BD, mangas, vinyles, escape games...)
- **Émojis** : Non inclus dans les descriptions mais peuvent être ajoutés selon la charte graphique

## Suggestions d'amélioration

Ces descriptions peuvent être :
- Testées auprès d'un panel de jeunes utilisateurs
- Ajustées selon le ton de marque du Pass Culture
- Traduites en versions plus courtes pour les tooltips
- Enrichies avec des exemples locaux selon la géolocalisation
