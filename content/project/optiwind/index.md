---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Optiwind"
summary: "[Projet Européen OPTIWIND - HORIZON 2020, consortium Clean Sky 2:](https://cordis.europa.eu/project/id/785300/fr) Optimized cockpit windshield for large diameter business aircraft"
authors: ["Nicolas Cellier"]
tags: ["résolution d'EDP", "simulation"]
categories: []
date:

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

lang: fr
---

{{< video src="hs_ratio.m4v" controls="yes" >}}

Ce projet à pour objectif une meilleure compréhension de l'écoulement des
gouttelettes d'eau sur les pare-brises d'avion. Il est nécessaire de chauffer
les pare-brises pour en éviter le gel (ce qui impliquerait une perte de
visibilité et impacterait les caractéristiques aérodynamiques de l'aéronef), ce
qui implique une consommation énergétique non négligeable.

Le dimensionnement de l'appareil de chauffe est piloté par des réglementations
relativement anciennes qui ne sont pas forcément adapté aux appareils modernes.
Il est possible que ces réglementations surestiment la puissance nécessaire à
l'évaporation des gouttelettes ruisselant sur le pare-brise.

Il est alors nécessaire d'acquérir à la fois des données expérimentales sur
l'écoulement et les outils de modélisation permettant une compréhension plus
fine des phénomènes physiques sous-jacents.

Ce projet est en cours et a mené à une première publication sur les méthodes de
modélisations [^Bresh2020].

Ce même modèle a été utilisé et étendu pour modéliser l'écoulement de
gouttelettes sur un domaine périodique, grâce à un solveur écrit en Julia. Celui
ci peut tourner sur GPU permettant des résolutions rapides ne nécessitant pas
de cluster de calculs.

{{< video src="20_dropplets_fine.mp4" controls="yes" >}}

[^Bresh2020]: [Augmented skew-symmetric system for shallow-water system with
  surface tension allowing large gradient of density]({{< ref
  "/publication/bresch-2020-augmented" >}} "Augmented skew-symmetric system for
  shallow-water system with surface tension allowing large gradient of density")
