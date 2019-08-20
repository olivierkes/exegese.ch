---
title: https (ou non), qu'en font les protestants romands?
date: 2019-08-20
description: Google veut nous faire croire que https est nécessaire à tout site web pour son référencement, pour la sécurité des internautes et pour une question d'image...
---



## À quoi sert `https`?

`https` est à la mode.
Avec `https`, un site web serait sécurisé, bien référencé et donnerait une belle image. 
Qu'en penser?

Le protocole `https` sécurise la connexion entre le serveur et l'ordinateur ou le smartphone de l'utilisateur.
Ce qui signifie que personne ne peut lire les informations qui transitent sur le réseau.
Pourtant, la sécurisation de la connexion ne suffit pas à faire un site sûr, notamment s'il est mal mis à jour ou mal codé.

Avec `https`, il est certain que la page reçue est parfaitement identique à la page envoyée.
Ce qui signifie que les différents fournisseurs d'accès ne peuvent pas envoyer de contenus, notamment des publicités, à l'insu du créateur du site.

Enfin, `https` donne une bonne image du site consulté. 
Il paraît (ou est) sûr, il est raisonnablement maintenu à jour, le prestataire technique a des compétences actuelles, etc.

## Pressions vs utilité

Malgré ses avantages, `https` est aussi adopté de plus en plus en raisons de pressions exercées.
Plus parfois pour ces pressions que pour une réelle utilité sécuritaire.

Les sites `https` seraient mieux référencés par Google.
C'est possible, mais pas évident.
Pourtant, dès que le roi des moteurs de recherche menace, les webmasters suivent.

Les navigateurs récents indiquent visuellement si un site n'est pas en `https`.
Ce qui signifie qu'un tel site, même s'il ne fait rien transiter de confidentiel par le réseau, passe pour peu sûr.
Il est alors plus simple de changer la configuration de son site que d'expliquer que, par choix, il reste en simple http.

Enfin, l'image de compétence, de sécurité joue à plein.
En passant mon site en `https`, je montre ma compétence technique à mes utilisateurs et à mes mandataires.
Même si, dans certains cas, c'est peu utile.

Certaines voix critique s'élèvent contre le `https` partout.
C'est par exemple le cas de l'expert Karl Dubost qui trouve que nous basculons vers un [système inutilement complexe](http://www.la-grange.net/2018/02/09/chimere-https).
Une critique à lire avant d'installer à tout prix `https`.

Voici un rapide état des lieux protestant romand, qui pourra vous inciter (ou non) à passer à `https`.

## Sites sans `https`


Le sites suivant fonctionnent sans `https`:

- centredesornetan.ch
- cret-berard.ch
- egliserefju.ch
- emploi-eglise.ch
- epg.ch
- erkw.ch
- ethikos.ch
- holygames.ch
- lelab.church
- lire-et-dire.ch
- mafemmeestpasteure.ch
- refbejuso.ch
- vocation.ch

## Sites avec `https`

### Fonctionnent avec et sans


Sans `hsts`, ce qui signifie que ces sites peuvent être consultés indéfiniment en `http` ou `https` (pourrait être modifié pour imposer `https`):

- contactgps.ch
- marcpernot.net
- mediaspro.ch

Les sites suivants envoient l'entête `hsts`, ce qui signifie que s'ils sont consultés une seule fois en `https`, ils le seront toujours par la suite avec ce navigateur (devrait être modifié pour imposer `https`):

- jeanmarcleresche.ch
- philippegolaz.ch
- theologeek.ch


### `https` imposé

La grande majorité impose l'utilisation de `https`, quel que soit le moyen utilisé:

- cedresformation.ch
- celebrer.ch
- cine-feuilles.ch
- diaconie.ch
- dianefriedli.ch
- dmr.ch
- eerv.ch
- eper.ch
- eren.ch
- evangile-et-liberte.net
- jecherchedieu.ch
- labokhi.ch
- moser-felix.ch
- musee-reforme.ch
- museeprotestant.org
- olivierbauer.org
- painpourleprochain.ch
- protestant-edition.ch
- protestinfo.ch
- questiondieu.com
- ref-fr.ch
- reforme.net
- reformes.ch
- regardsprotestants.com

## Problèmes `https`

Ca fonctionne, mais...

- marcpernot.net: lorsque le site est utilisé en `https`, une erreur est signalée parce qu'un fichier au moins est en `http` (pas très grave, le site est prévu pour http)
- oserdieu.ch: le site impose `https`, mais une erreur est signalée car des éléments sont en `http` (plus embêtant...)

## Remarques pratiques

NB: 
Je ne suis pas un spécialiste de sécurité informatique.
C'est une discipline à part entière et je vous invite à contacter des spécialistes pour des configurations avancées.
Attention au passage en `https`, puis à l'entête `hsts`, puis au *preload* `hsts`; ces trois manipulations peuvent rendre votre site inaccessible.

1. Si votre site fonctionne en `http` et `https` sans erreurs durant un certain temps, il me semble logique de forcer la redirection vers `https`.
2. La redirection vers `https` est facile à mettre en oeuvre (mais pas sans risques): changement d'adresse du site dans WordPress, extensions diverses ou redirection `.htaccess`. Chez [Infomaniak](https://www.infomaniak.com/fr/support/faq/1961/rediriger-tous-les-visiteurs-sur-le-site-avec-https-ssl), c'est bien documenté.
3. Lorsque le site envoie l'entête `hsts` et qu'il est consulté en `https`, il est compliqué pour le navigateur qui effectué la visite de revenir en arrière. Encore une fois, [Infomaniak](https://www.infomaniak.com/fr/support/faq/2133/desactiver-ou-personnaliser-le-hsts-dun-site-webhebergement) documente bien.
4. Si le site fonctionne bien avec `https` et `hsts`, il est possible de passer en *preload*. Ce qui signifie que le site est d'office chargé en `https`, sans redirection. C'est gravé dans le navigateur! C'est [hstspreload](https://hstspreload.org/?domain=exegese.ch) est l'outil qui permet d'activer la chose, comme c'est le cas d'exegese.ch.

Je reçois volontiers vos questions et remarques par [mail](/contact/).