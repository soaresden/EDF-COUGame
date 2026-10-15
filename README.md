<h1 align="center">🌬️ Pile Poil — le chantier du large</h1>

<p align="center">🇬🇧 <a href="README.en.md">English version</a></p>

<p align="center"><b>Hissez les 64 éoliennes du parc éolien en mer du Calvados, pièce par pièce, au bout d'une grue qui balance.</b><br>
Plus vous avancez vers le large, plus les éléments se déchaînent.</p>

<p align="center"><a href="https://soaresden.github.io/EDF-COUGame/"><b>▶ Jouer dans le navigateur</b></a> · ordinateur, tablette et téléphone · français / anglais</p>

<p align="center"><img src="docs/neige.jpg" width="820" alt="Une éolienne en construction sous la neige : PARFAIT ×6"></p>

---

## 🎮 Le jeu

Vous partez de la base de **Ouistreham** et vous hissez les éoliennes du parc, de **G01** à **A10**. Chacune sort de la mer et doit atteindre **174,5 m** en bout de pale : pièce de transition, tronçons de mât, puis nacelle et rotor.

- La grue balance la pièce au bout de son câble : **touchez l'écran** ou appuyez sur **Espace** pour la lâcher.
- Pile au-dessus de la précédente : **PARFAIT**. Les parfaits enchaînés font monter le combo et calment le balancement de la tour.
- Surveillez la **verticalité** : une tour trop penchée bascule.
- **Trois pièces à la mer** et le chantier de cette éolienne s'arrête.

Toutes les éoliennes sont ouvertes dès le départ : choisissez sur la carte celle que vous voulez construire. Chaque éolienne raccordée s'allume sur la carte du parc, avec un « Le saviez-vous ? » sur le vrai chantier.

## 🌩️ Des niveaux tous différents

Chaque éolienne a sa propre combinaison d'éléments, et leur nombre grimpe au fil du parc. Avant d'appareiller, la carte affiche le **niveau de difficulté** (une jauge à 5 crans) et les **éléments** qui vous attendent.

| Éoliennes | Difficulté | Éléments en même temps |
|---|---|---|
| 1 à 6 | 🟢 Calme | aucun, ou presque |
| 7 à 18 | 🟢 Agité | 1 |
| 19 à 34 | 🟡 Gros temps | 2 |
| 35 à 50 | 🟠 Tempête | 3 (la nuit amène toujours son orage) |
| 51 à 63 | 🔴 Déchaînement | 4 |
| **A10**, la dernière | 🔥 **Les éléments se déchaînent !** | tous, de nuit |

| Élément | Ce qu'il fait |
|---|---|
| 🌙 Nuit | on y voit beaucoup moins, seules les lumières du chantier éclairent |
| ⚡ Orage | nuit d'encre, éclairs qui aveuglent, pluie |
| 🌁 Brouillard | la brume couvre la mer et monte avec la tour, jusqu'au point de pose |
| ❄️ Neige | flocons poussés par le vent, pièces glissantes : le PARFAIT est plus serré |
| 💨 Rafales | une rafale annoncée pousse la pièce d'un coup |
| 🌊 Houle | la mer se creuse et la tour balance davantage |
| 🐦 Goélands | ils se posent sur la pièce et la font balancer davantage… KIAAA ! |

Le nombre de tronçons de mât, la vitesse du balancier et le vent augmentent aussi d'une éolienne à l'autre.

<p align="center"><img src="docs/dechaine.jpg" width="820" alt="La dernière éolienne : nuit, orage, brouillard, neige, rafales, houle et goélands"></p>

## ⚓ 64 navires du Débarquement

Comme sur le vrai parc, chaque éolienne porte le nom d'un navire du Débarquement et de la bataille de Normandie, avec son drapeau : la carte, le bandeau de départ, le tableau de bord et l'écran de fin l'affichent. Les rangées suivent la logique du parc : transports de matériel et de carburant (G), transports de troupes (F), frégates, monitors et dragueurs de mines (E), cuirassés (D), croiseurs (C), destroyers (B), et en première ligne face à la côte les navires emblématiques (A), comme le *Satterlee* de la pointe du Hoc, *La Combattante* qui ramène de Gaulle ou la barge du commando Kieffer.

La liste vient de la carte [« 64 navires mis à l'honneur »](https://www.parc-eolien-en-mer-du-calvados.fr/2023/04/12/lhistoire-au-coeur-du-parc-64-navires-mis-a-lhonneur/) du parc, établie par un groupe de travail d'historiens ; F07 porte le nom du Liberty ship *Jeremiah O'Brien*, comme annoncé par le parc en 2024.

## 🌊 Le vrai parc

Les chiffres du jeu sont ceux du **parc éolien en mer du Calvados** : 64 éoliennes de 7 MW (448 MW), entre 10 et 16 km au large de Courseulles-sur-Mer, sur environ 43,5 km². L'implantation de la carte suit le plan du parc, avec ses câbles regroupés en lignes jusqu'à la sous-station en mer.

## 🛠️ Technique

- Un seul fichier, [`index.html`](index.html) : HTML, CSS et JavaScript sans bibliothèque, dessin sur `<canvas>`, sons générés par Web Audio.
- La progression (éoliennes en service, scores, étoiles) est gardée dans le navigateur (`localStorage`).
- Français et anglais, avec le bouton 🇬🇧 EN / 🇫🇷 FR (le choix est mémorisé).
- Mouvements réduits respectés (`prefers-reduced-motion`).

Pour y jouer hors ligne, il suffit de télécharger `index.html` et de l'ouvrir.

---

<sub>Jeu fait par <a href="https://github.com/soaresden">soaresden</a>. Les logos du parc éolien en mer du Calvados et d'EDF power solutions appartiennent à leurs propriétaires.</sub>
