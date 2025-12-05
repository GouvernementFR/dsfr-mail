# Template de Mail Gouvernemental - DSFR

Ce repository propose un exemple de template de mail utilisable pour les communications officielles des services gouvernementaux.

## 📄 Description

Le fichier `template-generique.html` est un template d'email non exhaustif, conçu pour les envois de communications officielles des services gouvernementaux français. Il respecte l'identité visuelle et les standards d'accessibilité du Système de Design de l'État Français (DSFR).

>[!NOTE]
>Ce template n'inclut pas le code du DSFR lui-même. Il reprend uniquement son apparence et sa charte graphique. Il ne convient pas pour une utilisation complète du DSFR dans un projet web.

Il est recommandé de consulter la [documentation officielle du DSFR](https://www.systeme-de-design.gouv.fr/) pour toute personnalisation avancée ou intégration spécifique.

## ✨ Caractéristiques principales

### 🎨 Design et Identité visuelle

- **Conformité DSFR** : Respecte le Système de Design de l'État Français
- **Couleurs officielles** : Palette de couleurs conforme au DSFR

### 🌓 Mode sombre adaptatif

- **Support automatique** du mode sombre basé sur les préférences utilisateur
- **Classes CSS dédiées** pour les différents éléments en mode sombre :
  - `.darkmode` : Arrière-plan et texte principal
  - `.darkmode-1` à `.darkmode-6` : Variantes pour différents éléments
  - `.darkmode-button-*` : Styles spécifiques pour les boutons

### 📱 Responsive Design

- **Compatible multi-appareils** : Ordinateurs, tablettes, smartphones
- **Breakpoints adaptatifs** :
  - `@media (max-width: 600px)` : Tablettes
  - `@media (max-width: 480px)` : Smartphones
- **Images responsive** avec classes `.wlkm-resp` et `.img-max`

### 🧩 Structure modulaire

Le template est composé de plusieurs sections modulaires réutilisables :

- **En-tête institutionnel** avec logo Marianne et Nom du service
- **Section titre** avec fond coloré ou non
- **Sections de contenu** alternées (fond blanc/coloré)
- **Blocs texte/image** avec ou sans boutons
- **Blocs image** avec source
- **Zones de texte** et listes à puces
- **Zones de mise en avant** avec fonds colorés
- **Bloc contact** avec informations de contact
- **Boutons d'action** (primaire, secondaire, tertiaire)
- **Bloc avec séparateurs** **avec icônes
- **Cartes d'information** sur 2 colonnes
- **Pied de page** avec liens de désabonnement et mentions légales

### 🎯 Compatibilité clients de messagerie

- **Microsoft Outlook** (toutes versions) : Styles MSO spécifiques
- **Clients web** : Gmail, Yahoo, Outlook.com
- **Applications mobiles** : Support natif iOS/Android
- **Tables HTML** : Structure robuste pour maximum de compatibilité

## 🚀 Utilisation

### 1. Personnalisation du contenu

Le template est structuré en sections de `table` HTML. Pour personnaliser votre email :

- Ajoutez ou supprimez des sections selon la structure souhaitée
- Intégrez vos images en remplaçant les placeholders
- Modifiez le titre, le texte et les liens selon vos besoins

### 2. Images et logos

- Remplacez les images placeholder par vos visuels
- Respectez les dimensions recommandées
- Optimisez pour le web (format WebP recommandé avec fallback)
- Ajoutez des attributs `alt` descriptifs sur les images porteuses d'information

### 3. Couleurs et styles

Les couleurs principales utilisées dans le template sont :

- `#ECECFE` : Fond section titre
- `#F5F5FE` : Fond sections alternées
- `#FFFFFF` : Fond clair
- `#161616` : Texte principal
- `#6b6b6b` : Texte secondaire
- `#000091` : Liens et boutons

L'utilisation de couleurs et styles personnalisés doit respecter les directives du DSFR.

### 4. Configuration du mode sombre

Le mode sombre est activé automatiquement en fonction des préférences utilisateur. La propriété CSS `prefers-color-scheme` est utilisée pour surcharger les classes en mode sombre. C'est au sein de cette media query que les styles spécifiques au mode sombre peuvent être appliqués.

Les classes `.hide-white` et `.hide-black` permettent l'affichage conditionnel :

```html
<!-- Visible en mode clair uniquement -->
<img src="logo-light.png" class="hide-black">

<!-- Visible en mode sombre uniquement -->
<img src="logo-dark.png" class="hide-white">
```

### 5. Classes utilitaires principales

- `.wlkm-mw` : Largeur maximale responsive
- `.wlkm-cl` : Colonne centrée
- `.wlkm-hide` : Masquage sur mobile
- `.darkmode-*` : Variations mode sombre
- `.img-max` : Images responsive

## ⚠️ Recommandations importantes

### Accessibilité

- **Contraste minimal** : Respecter les ratios 4,5:1 pour le texte normal et 3:1 pour le texte large
- **Textes alternatifs** : Renseigner les attributs `alt` des images porteuses d'information
- **Taille des polices** : Minimum 14px pour le contenu principal et minimum 12px pour les textes secondaires
- **DSFR & RGAA** : Suivre les directives officielles pour l'accessibilité numérique

### Compatibilité

- **Clients de messagerie** : Tester sur les principaux clients (Outlook, Gmail, Apple Mail)
- **Inline CSS** : Privilégier les styles inline pour la compatibilité
- **Tables HTML** : Utiliser des tableaux pour la mise en page afin d'assurer une compatibilité maximale

### Conformité légale

- **RGPD** : Inclure les liens de désabonnement obligatoires
- **Mentions légales** : Lien vers la politique de données personnelles
- **Identification** : Mentionner clairement l'expéditeur institutionnel

## 📞 Support

Pour toute question concernant l'utilisation de ce template :

- **Documentation DSFR** : [systeme-de-design.gouv.fr](https://www.systeme-de-design.gouv.fr/)
- **Accessibilité & RGAA** : [accessibilite.numerique.gouv.fr](https://accessibilite.numerique.gouv.fr/)
- **RGPD** : [cnil.fr](https://www.cnil.fr/)

## Contribution

Les contributions à ce projet sont les bienvenues. Veuillez soumettre vos propositions via des pull requests sur le dépôt GitHub.

## Licence et droit d'utilisation

Le contenu de ce projet est placé sous licence MIT License. Voir [LICENSE.md](https://github.com/GouvernementFR/dsfr/blob/main/LICENSE.md).

#### ⚠️ Utilisation interdite en dehors des sites Internet de l'État

>Il est formellement interdit à tout autre acteur d’utiliser le Système de Design de l’État et ce template de mail (les administrations territoriales ou tout autre acteur privé). Le Système de Design de l’État représente l’identité numérique de l’État. En cas d’usage à des fins trompeuses ou frauduleuses, l'État se réserve le droit d’entreprendre les actions nécessaires pour y mettre un terme.

Voir les [conditions générales d'utilisation](https://github.com/GouvernementFR/dsfr/blob/main/doc/legal/cgu.md).

#### ⚠️ Prohibited Use Outside Government Websites

>This Design System is only meant to be used by official French public services' websites and apps. Its main purpose is to make it easy to identify governmental websites for citizens. See terms.

---

**Service d'Information du Gouvernement**
