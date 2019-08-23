---
title: "Grand test: perfomance, accessibilité, bonnes pratiques & SEO"
date: 2019-08-23
description: L'utilisation de Lighthouse en ligne de commande permet de systématiser le travail d'analyse sur les sites web. L'occasion de passer le web protestant romand au crible.
---

Je vous envoie les résultats ainsi, sans autre interprétation.
À vous de regarder où se trouve votre site.
Le tableau est classé par ordre décroissant de performance et comprend les données suivantes:

- domaine testé (page d'accueil uniquement)
- indice de performance
- indice d'accessibilité
- indice de bonnes pratiques
- indice de SEO

Le meilleur résultat possible est 100.
Regardez, comparez, testez!


| Domaine | Perf | A11y | BP | SEO |
|---|---|---|---|---|
| holygames.ch | 99 | 82 | 79 | 100 |
| jeanmarcleresche.ch | 97 | 97 | 79 | 92 |
| ref-fr.ch | 97 | 41 | 86 | 83 |
| eren.ch | 96 | 98 | 93 | 98 |
| dianefriedli.ch | 94 | 100 | 93 | 97 |
| erkw.ch | 94 | 58 | 57 | 64 |
| protestant-edition.ch | 92 | 98 | 79 | 99 |
| dmr.ch | 91 | 40 | 64 | 67 |
| egliserefju.ch | 91 | 93 | 64 | 64 |
| protestinfo.ch | 88 | 77 | 79 | 92 |
| musee-reforme.ch | 86 | 72 | 79 | 83 |
| centredesornetan.ch | 86 | 67 | 57 | 82 |
| jecherchedieu.ch | 83 | 86 | 86 | 97 |
| refbejuso.ch | 82 | 93 | 64 | 85 |
| contactgps.ch | 76 | 75 | 64 | 97 |
| reformes.ch | 76 | 68 | 79 | 80 |
| cine-feuilles.ch | 73 | 71 | 86 | 78 |
| evangile-et-liberte.net | 72 | 49 | 79 | 79 |
| olivierbauer.org | 70 | 87 | 93 | 97 |
| questiondieu.com | 62 | 37 | 71 | 98 |
| cret-berard.ch | 62 | 77 | 71 | 79 |
| painpourleprochain.ch | 61 | 72 | 86 | 89 |
| theologeek.ch | 59 | 87 | 71 | 89 |
| eper.ch | 55 | 74 | 79 | 79 |
| philippegolaz.ch | 53 | 88 | 64 | 98 |
| moser-felix.ch | 52 | 94 | 93 | 95 |
| mediaspro.ch | 51 | 78 | 71 | 92 |
| lire-et-dire.ch | 47 | 60 | 64 | 97 |
| emploi-eglise.ch | 43 | 84 | 79 | 90 |
| vocation.ch | 43 | 80 | 71 | 83 |
| diakonie.ch | 37 | 83 | 79 | 100 |
| ethikos.ch | 33 | 87 | 71 | 96 |
| museeprotestant.org | 30 | 75 | 79 | 88 |
| reforme.net | 27 | 79 | 86 | 97 |
| labokhi.ch | 26 | 92 | 71 | 92 |
| celebrer.ch | 24 | 33 | 71 | 67 |
| regardsprotestants.com | 23 | 77 | 64 | 89 |
| epg.ch | 20 | 69 | 57 | 91 |
| cedresformation.ch | 18 | 94 | 79 | 100 |
| marcpernot.net | 17 | 89 | 86 | 91 |
| lelab.church | 17 | 66 | 57 | 83 |
| oserdieu.ch | 13 | 65 | 64 | 91 |
| eerv.ch | 11 | 69 | 57 | 91 |
| mafemmeestpasteure.ch | 1 | 65 | 57 | 90 |


## Remarques sur les résultats

- Les indices ne sont que des indicateurs techniques: quand ils sont très bons, il n'est pas encore certain que tout va bien. Par exemple, le SEO peut être techniquement bon, mais les contenus textuels mauvais.
- **Quand les indices sont mauvais, c'est très souvent qu'il y a un vrai problème!**
- De nombreux sites pourraient être améliorés facilement en corrigeant des erreurs manifestes, parfois en modifiant seulement quelques fichiers.
- Vous pouvez effectuer vos tests Lighthouse dans le navigateur Chrome. Il vous donnera un bilan complet avec tous les détails.

## Détails techniques

- Le test a été réalisé sur mon ordinateur personnel, le 23 août 2019 à 11h00. Votre connexion Internet sera plus rapide ou plus lente, vous vous situez dans une autre région du monde, etc.
- Les redirections ont été prises en compte avant le test, en utilisant [httpstatus](https://httpstatus.io/). Donc [avec ou sans www](/blog/www/) et [avec ou sans `https`](/blog/https/) selon les réglages du site.
- [Lighthouse](https://developers.google.com/web/tools/lighthouse/) a été utilisé en [ligne de commande](https://www.npmjs.com/package/lighthouse), avec son outil de [traîtement par lots](https://www.npmjs.com/package/lighthouse-batch).
