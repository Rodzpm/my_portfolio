# Workshop : Développement d'un Site Portfolio avec Vue.js

Cet atelier vous guidera à travers toutes les étapes, de l'installation à la mise en ligne de votre propre site portfolio.

## Objectif

Le but de cet atelier est de vous accompagner dans la création d'un site portfolio interactif en utilisant Vue.js. À la fin de cet atelier, vous aurez un site portfolio de base que vous pourrez personnaliser selon vos préférences.

## Prérequis

Assurez-vous d'avoir les éléments suivants installés sur votre machine :
- [Node.js](https://nodejs.org/) (avec npm)

## 1. Installation

Vérifiez que node.js a bien été installé:

```bash
node -v
```

Créez le projet Vue.js

```bash
npm create vue@latest
```

Précisez le nom de votre projet et mettez à "non" tous les ajouts proposés (après si vous connaissez et souhaitez allez plus loin...)

Déplacez vous dans le dossier correspondant au projet et installez les dépendances

```
cd [your_beautiful_portfolio_name]
npm install
```
Vous pouvez lancez le projet et voir votre magnifique portfolio (même si il y est vide pour l'instant)

```
npm run dev
```

## 2. Commencer un Projet avec Vue.js

Nous utilisons Vue.js comme framework pour ce workshop. Vous pouvez en apprendre plus sur Vue.js [ici](https://vuejs.org/).

Dans le dossier `src`, vous allez retrouver `App.vue`, qui est le composant principal de votre application Vue.js. Ce fichier se compose des sections suivantes :

### Template (`<template>`)

Contient le code HTML de votre composant. Utilisez la syntaxe Vue.js pour définir la structure de votre page.

```html
<template>
  <div>
    <Header />
    <main>
      <!-- Contenu principal de votre page -->
    </main>
    <Footer />
  </div>
</template>
```

### Script (<script>)
Contient la logique JavaScript de votre composant. Définissez les méthodes, les données et les hooks de cycle de vie du composant, et importez d'autres composants ou bibliothèques nécessaires.

```html
<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Header,
    Footer
  },
  data() {
    return {
      // Données spécifiques au composant
    }
  },
  methods: {
    // Méthodes spécifiques au composant
  }
}
</script>
```

### Style (<style>)
Contient les styles CSS spécifiques au composant. Utilisez du CSS classique ou des préprocesseurs comme Sass ou Less.

```html
<style>
/* Styles spécifiques au composant */
</style>
```

C'est dans App.vue que vous organisez la mise en page générale de votre application et intégrez les différentes parties de votre portfolio. Créez d'autres composants dans le dossier components pour organiser votre code de manière modulaire et réutilisable.

Je vous conseille vivement d'aller vous renseigner auprès de la [Documentation Vue.js](https://vuejs.org/guide/introduction.html).

## 4. Déploiement sur Vercel

Nous allons déployer votre site portfolio sur Vercel, une plateforme de déploiement simple et rapide.

1. Créez un compte sur [Vercel](https://vercel.com/).
2. Ajoutez votre projet sur Vercel.
3. Configurez les paramètres de déploiement, et n'oubliez pas de définir les variables d'environnement si nécessaire.
4. Votre site sera automatiquement déployé à chaque push sur la branche principale (main/master).

## Et après ?

- Personnalisez davantage votre site portfolio en ajoutant des projets personnels, des blogs, etc.
- Explorez des fonctionnalités avancées de Vue.js pour améliorer votre site.
- Partagez votre travail et demandez de l'aide sur le canal de communication dédié.

## Ressources Complémentaires

- [Documentation Vue.js](https://vuejs.org/guide/introduction.html)
- [Vercel Documentation](https://nodejs.org/docs/latest/api/)
