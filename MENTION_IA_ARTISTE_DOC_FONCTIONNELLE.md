# 🎨 Mention IA sur la Biographie d'Artiste
## Documentation Fonctionnelle - Version Non-Technique

---

## 🎯 En une phrase

**Quand une biographie d'artiste a été créée avec l'aide de l'intelligence artificielle, on l'indique clairement à l'utilisateur avec une mention "© Contenu généré par IA ✨" et un lien vers la source originale (Wikipédia).**

---

## ❓ Pourquoi cette fonctionnalité ?

### Transparence et confiance
- Les utilisateurs ont le droit de savoir quand un contenu a été créé par une IA
- Cela respecte les bonnes pratiques et potentiellement les futures réglementations
- Cela renforce la crédibilité de pass Culture

### Traçabilité des sources
- Le lien vers Wikipédia permet à l'utilisateur d'accéder à la source originale
- L'utilisateur peut vérifier ou approfondir les informations

---

## 📖 Scénario d'utilisation complet

### Situation de départ
**Julie, 19 ans, utilise l'application pass Culture. Elle cherche des concerts et tombe sur un artiste qu'elle ne connaît pas.**

### 📱 Étape 1 : Découverte de la page artiste
Julie clique sur le nom de l'artiste. Elle arrive sur sa page et voit :
- Une photo de l'artiste
- Son nom
- Les **premières lignes** de sa biographie (environ 250 caractères)
- Un bouton **"Voir plus"**

> 💡 **À ce stade** : Julie ne voit **PAS** encore la mention IA. L'interface reste simple et épurée.

---

### 📱 Étape 2 : Lecture de la biographie complète
Julie veut en savoir plus. Elle clique sur **"Voir plus"**.

**La biographie s'agrandit** et révèle le texte complet.

**C'est maintenant qu'apparaît** :
- 📝 La mention : **"© Contenu généré par IA ✨"**
- 🔗 Un lien cliquable : **"Source : Wikipédia"**

---

### 📱 Étape 3 : Accès à la source (optionnel)
Si Julie le souhaite, elle peut cliquer sur **"Source : Wikipédia"**.
→ Elle est redirigée vers la page Wikipédia de l'artiste dans son navigateur.

---

## 📊 Tableau récapitulatif : Quand la mention apparaît-elle ?

| **État de la biographie** | **Mention IA visible ?** | **Pourquoi ?** |
|---|---|---|
| 🔒 **Biographie courte** (moins de 250 caractères) | ❌ **Non** | Pas de bouton "Voir plus", donc pas besoin de mention |
| 📖 **Biographie longue, pas encore étendue** | ❌ **Non** | L'utilisateur n'a pas encore demandé à voir le contenu complet |
| ✅ **Biographie étendue + générée par IA + source Wikipedia** | ✅ **Oui** | Toutes les conditions sont réunies |
| ⚠️ **Biographie étendue + générée par IA MAIS pas de source** | ❌ **Non** | Sécurité : on affiche la mention seulement si on peut fournir la source |
| ⚠️ **Biographie étendue + écrite manuellement (pas d'IA)** | ❌ **Non** | Pas d'IA = pas de mention |

---

## 🔍 Les règles métier détaillées

### Règle 1 : La mention n'apparaît que sur demande
**Pourquoi ?**
- Éviter de surcharger visuellement la page artiste
- Laisser l'utilisateur découvrir l'artiste sans distraction
- La mention n'est utile que pour ceux qui lisent la biographie complète

**Conséquence :**
- Si l'utilisateur ne clique jamais sur "Voir plus", il ne verra jamais la mention
- C'est un choix assumé pour privilégier l'expérience utilisateur

---

### Règle 2 : La mention n'apparaît que si on a une source fiable
**Pourquoi ?**
- Une mention sans source serait incomplète
- Wikipédia est la source utilisée pour générer la biographie
- Le lien permet à l'utilisateur de vérifier l'information

**Conséquence :**
- Si un artiste a une biographie IA mais pas de page Wikipédia, la mention ne s'affichera pas
- C'est une garantie de qualité

---

### Règle 3 : Toutes les biographies ne sont pas générées par IA
**Deux types de biographies coexistent :**
1. **Biographies manuelles** : Écrites par l'équipe pass Culture ou récupérées d'autres sources
   → Pas de mention IA
2. **Biographies IA** : Générées automatiquement depuis Wikipédia
   → Mention IA affichée

**Comment faire la différence techniquement ?**
C'est automatique : le système sait quelle source a été utilisée et affiche la mention en conséquence.

---

## 🎨 Exemple concret : Le cas d'Avril Lavigne

### Ce que voit l'utilisateur

**État initial (biographie courte) :**
```
Avril Lavigne

Avril Ramona Lavigne, née le 27 septembre 1984 à
Belleville en Ontario, est une auteure-compositrice-
interprète et actrice canadienne...

[Voir plus]
```

**Après clic sur "Voir plus" :**
```
Avril Lavigne

Avril Ramona Lavigne, née le 27 septembre 1984 à
Belleville en Ontario, est une auteure-compositrice-
interprète et actrice canadienne. Elle est
considérée comme l'une des artistes les plus
influentes du rock alternatif et du pop punk des
années 2000...

[texte complet de la biographie]

© Contenu généré par IA ✨
Source : Wikipédia
```

---

## 💼 Pour les Product Managers / Product Owners

### Ce qu'il faut savoir pour piloter cette fonctionnalité

#### 📈 Métriques à suivre
- **Taux d'expansion de biographie** : Combien d'utilisateurs cliquent sur "Voir plus" ?
- **Taux de clic sur le lien Wikipédia** : Les utilisateurs sont-ils intéressés par la source ?
- **Proportion d'artistes avec biographie IA vs manuelle** : Quel est le taux de couverture ?

#### 🎛️ Levier d'activation
Aucun ! Cette fonctionnalité est toujours active pour tous les utilisateurs.

> **Note :** La doc originale mentionne un feature flag `WIP_ARTIST_PAGE`, mais il n'a pas été trouvé dans le code actuel. Si la page artiste est derrière un flag, c'est pour activer/désactiver toute la page, pas spécifiquement la mention IA.

#### 🔄 Évolutions possibles
1. **Personnaliser le texte de la mention** : Actuellement "© Contenu généré par IA ✨", mais pourrait être adapté
2. **Ajouter d'autres sources** : Pour l'instant uniquement Wikipédia
3. **Afficher la mention plus tôt** : Actuellement cachée jusqu'au clic sur "Voir plus"
4. **Ajouter une modal explicative** : Expliquer comment l'IA a généré la biographie

---

## 🧪 Cas d'usage à tester (QA)

### ✅ Cas nominal
1. Accéder à la page d'un artiste avec biographie IA et source Wikipedia
2. Cliquer sur "Voir plus"
3. ✅ Vérifier que la mention "© Contenu généré par IA ✨" apparaît
4. ✅ Vérifier que le lien "Source : Wikipédia" est cliquable
5. Cliquer sur le lien
6. ✅ Vérifier l'ouverture de la page Wikipédia correcte

### ⚠️ Cas limites

**Cas 1 : Biographie courte (< 250 caractères)**
- Pas de bouton "Voir plus"
- Pas de mention IA affichée (même si générée par IA)
- ⚠️ **Point d'attention** : L'utilisateur ne saura pas que c'est de l'IA

**Cas 2 : Biographie IA sans source Wikipedia**
- Bouton "Voir plus" présent
- Après clic, pas de mention IA
- Comportement normal : on n'affiche pas de mention sans source

**Cas 3 : Biographie manuelle**
- Bouton "Voir plus" présent
- Après clic, pas de mention IA
- Comportement normal : pas d'IA utilisée

**Cas 4 : Artiste sans biographie**
- Aucun texte de biographie affiché
- Pas de bouton "Voir plus"
- Pas de mention IA

---

## 📱 Spécificités d'affichage

### Texte exact de la mention
```
© Contenu généré par IA ✨
```
> ⚠️ Inclut un emoji sparkle (✨) pour rendre la mention plus visible et moins "légale"

### Format du lien source
```
Source : Wikipédia
```
> Cliquable, ouvre le navigateur externe

### Emplacement
- En bas de la biographie complète
- Après le dernier paragraphe de texte
- Séparé visuellement du contenu

---

## 🔐 Considérations légales et éthiques

### Conformité RGPD
✅ Pas de données personnelles collectées spécifiquement pour cette fonctionnalité

### Transparence algorithmique
✅ Respect des bonnes pratiques : on indique clairement l'usage d'IA

### Attribution de source
✅ Lien direct vers Wikipédia, respect de la source originale

### Droit d'auteur
✅ Wikipédia utilise une licence libre (CC BY-SA), réutilisation possible avec attribution

---

## 📞 Questions fréquentes (FAQ étendue)

### 1. Pourquoi la mention n'apparaît-elle pas tout de suite ?
**Réponse courte :** Pour ne pas surcharger l'interface et gêner la lecture.

**Réponse longue :**
- La majorité des utilisateurs ne lisent que les premières lignes
- Afficher la mention dès le début créerait une "pollution visuelle"
- Seuls les utilisateurs vraiment intéressés par la biographie complète voient la mention
- C'est un compromis entre transparence et expérience utilisateur

---

### 2. Que se passe-t-il si je clique sur "Source : Wikipédia" ?
**Réponse :**
- Ouverture d'un navigateur externe (Chrome, Safari, etc.)
- Redirection vers la page Wikipédia de l'artiste dans la langue de l'utilisateur
- L'utilisateur peut consulter la source complète, avec plus de détails
- Il peut ensuite revenir à l'application pass Culture

---

### 3. Comment sait-on qu'une biographie a été générée par IA ?
**Réponse pour les non-tech :**
Lorsque l'équipe technique crée une biographie avec l'aide de l'IA, elle est "marquée" dans la base de données. L'application sait alors qu'elle doit afficher la mention.

**Réponse avec détails :**
- La base de données contient deux champs différents : `biography` (IA) et `description` (manuel)
- Si le champ `biography` est rempli, la mention IA s'affiche
- Sinon, on utilise le champ `description` sans mention

---

### 4. Tous les artistes ont-ils une biographie ?
**Non.** Il y a plusieurs cas :
- 🟢 **Artistes avec biographie IA** : Les plus connus, présents sur Wikipédia
- 🟡 **Artistes avec biographie manuelle** : Ajoutée par l'équipe pass Culture
- 🔴 **Artistes sans biographie** : Artistes émergents ou peu documentés

---

### 5. Peut-on désactiver l'IA pour certains artistes ?
**Oui.** Si une biographie manuelle est préférée (par exemple pour un partenariat), on peut :
- Supprimer la biographie IA
- La remplacer par une description manuelle
- La mention IA disparaîtra automatiquement

---

### 6. Que se passe-t-il si Wikipédia modifie la page de l'artiste ?
**Aujourd'hui :** La biographie dans pass Culture n'est pas mise à jour automatiquement. Elle est générée une fois puis stockée.

**Dans le futur :** Possible mise en place d'une synchronisation périodique pour garder les biographies à jour.

---

### 7. L'IA traduit-elle automatiquement les biographies ?
**Bonne question !** Cela dépend de l'implémentation :
- Si l'utilisateur est en français, on génère depuis Wikipédia FR
- Si l'utilisateur est dans une autre langue, il faut soit :
  - Générer depuis Wikipédia dans sa langue
  - Traduire la biographie française
  - Ne rien afficher si pas disponible

> ⚠️ **Point à clarifier avec l'équipe technique**

---

### 8. Pourquoi ne pas mettre la mention IA partout (offres, lieux, etc.) ?
**Réponse stratégique :**
Pour l'instant, on commence par les biographies d'artistes car :
- C'est un contenu éditorial long
- L'IA apporte une vraie valeur (génération de texte)
- Les utilisateurs s'attendent à une source pour ce type de contenu

Pour les autres contenus (descriptions d'offres courtes, etc.), l'IA n'est peut-être pas utilisée, ou différemment.

---

## 🚀 Résumé pour décideurs (Executive Summary)

### En 3 points clés

1. **Transparence** : On informe les utilisateurs quand une biographie est générée par IA
2. **Traçabilité** : On fournit un lien direct vers la source (Wikipédia)
3. **UX optimale** : La mention n'apparaît que quand l'utilisateur lit la biographie complète

### Bénéfices business

| Bénéfice | Impact |
|---|---|
| **Conformité réglementaire** | Anticipe les futures obligations légales sur l'IA |
| **Confiance utilisateur** | Renforce la crédibilité de pass Culture |
| **Gain de temps** | Génération automatique de centaines de biographies |
| **Qualité du contenu** | Source fiable (Wikipédia) et vérifiable |

### Risques et mitigation

| Risque | Mitigation |
|---|---|
| **"L'IA c'est de la triche"** | La mention et la source montrent la transparence |
| **Contenu obsolète** | Prévoir une mise à jour périodique |
| **Biographies trop courtes** | La mention ne s'affiche pas = pas de problème |
| **Pas de source Wikipedia** | La mention ne s'affiche pas = sécurité |

---

## 📚 Annexes pour aller plus loin

### Glossaire rapide

- **Biographie tronquée** : Texte raccourci à ~250 caractères avec "..."
- **Biographie étendue** : Texte complet visible après clic sur "Voir plus"
- **Feature flag** : Interrupteur pour activer/désactiver une fonctionnalité
- **API** : Le "serveur" qui fournit les données à l'application mobile

---

### Schéma de décision : La mention s'affiche-t-elle ?

```
Utilisateur accède à la page artiste
         ↓
La biographie existe-t-elle ?
    ↓ Non → Rien à afficher
    ↓ Oui
         ↓
La biographie est-elle longue (>250 caractères) ?
    ↓ Non → Pas de bouton "Voir plus" → Mention jamais affichée
    ↓ Oui → Bouton "Voir plus" visible
         ↓
L'utilisateur clique-t-il sur "Voir plus" ?
    ↓ Non → Mention jamais affichée
    ↓ Oui → Biographie étendue
         ↓
La biographie a-t-elle été générée par IA ?
    ↓ Non → Pas de mention (biographie manuelle)
    ↓ Oui
         ↓
Une source Wikipedia existe-t-elle ?
    ↓ Non → Pas de mention (sécurité)
    ↓ Oui → ✅ AFFICHAGE DE LA MENTION IA
```

---

## 📝 Notes finales

### Version du document
- **Date de création** : Janvier 2026
- **Auteur** : Documentation fonctionnelle pass Culture
- **Public cible** : Product Managers, Business Analysts, QA, parties prenantes non-techniques

### Points de contact
Pour toute question sur cette fonctionnalité :
- **Fonctionnel** : Équipe Product
- **Technique** : Équipe Dev Backend (API) et Mobile
- **Analytique** : Équipe Data

---

**🎉 Fin de la documentation fonctionnelle**

> *Cette documentation explique COMMENT fonctionne la mention IA pour les utilisateurs et les équipes métier. Pour la documentation technique (code, API, architecture), se référer à la documentation développeur.*
