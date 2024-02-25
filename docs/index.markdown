---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "Genero City - Explications de choix d'architecture"
---

## Avant propos

Le but de ce projet est de construire pas à pas une solution simpliste d'échange de'objets entre
utilisateurs, tout en expliquant les choix d'architecture.

Il ne s'agit **en aucun cas d'une vérité absolue** sur l'architecture logicielle qu'une application
devrait avoir, mais un cheminement de réflexion pour arriver à une solution, répondant au besoin.

Mon objectif est de vous permettre de prendre des bribes de réflexion pour construire votre propre
solution, en fonction de vos besoins.

Gardez en tête qu'**une bonne architecture** - au dela de l'utilité basique de rendre le code
compréhensible, maintenable, et évolutif - **doit être une architecture comprise de l'ensemble de l'
équipe**, et doit être adaptée à l'équipe qui la construit (en termes de connaissances, d'outils, de
méthodes de travail, etc.).

## Introduction

L'article est découpé en plusieurs parties, chacune correspondant à une étape de la construction de
l'applicatition. Dans chaque partie, l'objectif sera clairement défini, et les choix d'architecture
expliqués. Parfois, plusieurs choix d'architecture seront proposés, et les avantages et
inconvénients de chacun seront discutés plus ou moins succinctement.

Il est possible que vous ne soyez pas d'accord avec les choix effectués ou les explications
données, et c'est parfaitement normal. Il n'existe pas de vérité absolue en architecture logicielle,
et chaque choix dépend de nombreux facteurs. Si vous avez des suggestions, des critiques, ou des
questions, n'hésitez pas à me contacter.

Cet article reste une article de réflexion à but pédaogique, et ne prétend pas être une référence en
architecture logicielle.

## Le projet

Afin d'illustrer les choix d'architecture, nous allons construire une application simpliste de don d'objets entre utilisateurs. L'application sera nommée "Genero City".

Elle permettra à des utilisateurs (donneurs) de donner des objets dont ils n'ont plus besoin. Les utilisateurs (adopteurs) pourront voir les objets disponibles, et les demander. Les donneurs pourront accepter ou refuser les demandes.

Les actions effectuées seront logguées à des fins d'audit.

Le projet sera développé en TypeScript, et utilisera un minimum de frameworks et librairies externes, pour se concentrer sur les choix d'architecture.

Les interactions avec l'application se feront via API, il n'y aura pas d'interface graphique.

