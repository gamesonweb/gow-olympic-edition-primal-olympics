# Primal Olympics
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/primal-olympics-logo.png?raw=true" alt="logo">
</p>

*******
## Sommaire
1. [Trailer du jeu](#trailer-du-jeu)
2. [Lien du jeu](#lien-du-jeu)
3. [Code source](#code-source)
4. [Présentation de l’équipe](#présentation-de-léquipe)
5. [Pourquoi Primal Olympics ?](#pourquoi-primal-olympics-)
6. [Contexte](#contexte)
7. [Description du jeu](#description-du-jeu)
8. [Fonctionnalités](#fonctionnalités)
    - [Personnalisation des personnages](#personnalisation-des-personnages)
    - [Paramètres](#paramètres)
    - [Comment créer une partie](#comment-créer-une-partie)
    - [Comment rejoindre une partie](#comment-rejoindre-une-partie)
    - [Choix des mini-jeux](#choix-des-mini-jeux)
9. [Mini-jeux](#mini-jeux)
    - [Downhill Madness](#downhill-madness)
    - [Trex Track (100m)](#trex-track-100m)
    - [Stellar Storm](#stellar-storm)
    - [Savage Soccer (football)](#savage-soccer-football)
10. [Développement du multijoueur](#développement-du-multijoueur)
    - [Architecture](#architecture)
    - [Prédiction et réconciliation](#prédiction-et-réconciliation)
    - [Interpolation](#interpolation)
11. [Réalisation Assets](#réalisation-assets)
    - [Meshes](#meshes)
    - [Réalisation des Map](#réalisation-des-map)
    - [Animations](#animations)
    - [Sons](#sons)
12. [Problème de connexion à une partie](#probleme-connexion)
13. [Développé avec](#développé-avec)
14. [Logiciels utilisés](#logiciels-utilisés)
15. [Vidéos de développement](#vidéos-de-développement)

*******

<div id='trailer-du-jeu'></div>

## Trailer du jeu

[Trailer](https://youtu.be/yUZOyJOSVew)

<div id='lien-du-jeu'></div>

## Lien du jeu
Jouez au jeu ici : [Primal Olympics](https://doori4n.itch.io/gamesonweb-2024)

<div id='code-source'></div>

## Code source
Trouvez le code source ici : [Code source](https://github.com/Doori4N/primal-olympics/)

<div id='présentation-de-léquipe'></div>

## Présentation de l’équipe
Notre équipe est composée d’étudiants en Master 1 d'informatique, chacun ayant apporté son expertise au développement de notre jeu. **[Quentin Escobar](https://github.com/Moustik06)** a pris en charge la modélisation 3D, créant les cartes, les objets, ainsi que les personnages et leurs tenues, cheveux et barbes. **[Hugo Savasta](https://github.com/HugoSavasta)**  s'est concentré sur le développement des mini-jeux, assurant des expériences variées et captivantes pour les joueurs. **[Dorian Girard](https://github.com/Doori4N/)** a structuré le jeu, conçu l'interface utilisateur (UI) et également conçu des mini-jeux. Ensemble, nous avons uni nos compétences pour créer une aventure immersive et divertissante dans les PRIMAL OLYMPICS.

<div id='pourquoi-primal-olympics-'></div>

## Pourquoi Primal Olympics ?
Lorsque le thème des Jeux Olympiques nous a été proposé, nous avons décidé de l'aborder de manière originale en situant notre jeu à la période de la préhistoire. Nous avons imaginé une édition unique des Primal Olympics, où les participants doivent démontrer leurs capacités physiques et mentales à travers divers mini-jeux. Nous avons conçu quatre mini-jeux, dont certains sont inspirés de vrais sports, tandis que d'autres sont des réinterprétations adaptées à l'époque préhistorique. Cette combinaison de sports authentiques et de concepts fantaisistes nous a permis de créer une expérience de jeu originale.

<div id='contexte'></div>

## Contexte
Nous vous invitons à célébrer la 100ème édition des Primal Olympics, une expérience unique qui vous transporte à l'époque de la préhistoire ! Dans cet univers où les premiers athlètes s'affrontent, vous découvrirez une série de mini-jeux captivants.

<div id='description-du-jeu'></div>

## Description du jeu
Dans notre jeu vous devrez affronter vos adversaires à travers différentes épreuves. A l’issue de chaque épreuve des médailles vous seront attribuées en fonction de votre classement (Médaille d’or, d’argent et de bronze pour les 3 premières positions et aucune médaille pour les joueurs restants). Quand toutes les épreuves auront été jouées, le joueur ayant remporté le plus de médailles sera désigné vainqueur des Primals Olympics. 

Notre jeu est jouable en solo et en multijoueur. Cependant, si vous voulez profiter de la meilleure expérience nous vous conseillons fortement de jouer en multijoueur.

Dans Primal Olympics, vous pouvez jouer au clavier ou à la manette. Si vous n’êtes pas habitué à jouer au clavier nous vous conseillons d’utiliser manette. Avant chaque début de mini jeux, les touches à utiliser vous sont montrées en fonction des contrôles utilisés, ainsi qu’une description de l’épreuve.

<div id='fonctionnalités'></div>

## Fonctionnalités

<div id='personnalisation-des-personnages'></div>

### Personnalisation des personnages
Nous avons mis l’accent sur la personnalisation afin que chaque joueur puisse obtenir une expérience de jeu unique. Le joueur à le choix de son personnage masculin ou féminin, de sa couleur de peau, des ses vêtements, ainsi que de la couleur de ses cheveux. Le jeu offre une multitude de combinaisons possibles pour se différencier des autres joueurs.

<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExdHZybGI3am1qYWxxMzk3cGhlc2tzcHp5d2c3ejJyNXp5ODFseHVnNSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/61nnHZqzLU0YDMgKip/source.gif" alt="perso_custom" width="600">
</p>

<div id='paramètres'></div>

### Paramètres
Le joueur a la possibilité de faire afficher ses FPS (Frames per Second) ou non, il peut également régler le volume de son du jeu pour une expérience plus immersive.

<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExNWMwb2QxejY1cTE2eXh6aDMxYWFmbWhhZGJzNjhxdTA5ZnY1eTNtMiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/syRoIvlsFKczkd93lL/giphy.gif" alt="param" width="600">
</p>

<div id='comment-créer-une-partie'></div>

### Comment créer une partie
- Il suffit de cliquer sur le bouton `Host` dans le menu principal.

<p align="center">
  <img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExNnJzMzM1N3dkemtyN3N4eXh1NHp6Z2x2Mmtmbng0ODk0MXBtNWc3eSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/FFzRSXlEonAOe5DppE/giphy.gif" alt="host" width="600">
</p>

<div id='comment-rejoindre-une-partie'></div>

### Comment rejoindre une partie
- Il suffit de copier le code que l'hôte nous a envoyé !

<p align="center">
  <img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExbTRqbjY5aXN4cndvajcwczRycmZwbXhlMmg3aHgxcmdtYWF1a25hNyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/cK7oZ3vdPWOVQlI9Eo/source.gif" alt="join" width="600">
</p>  

<div id='choix-des-mini-jeux'></div>

### Choix des mini-jeux
- L'hôte a la possibilité de sélectionner les mini-jeux et le nombre de mini-jeux qui seront joués.

<p align="center">
  <img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExZDM3emxoaDFtcTI2MHJzNWhkZ2RzcHRmMmlvazY5cTBneHVvOHdpMCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/smCnfcS9HqBnnsxipE/giphy.gif" alt="choix_game" width="600">
</p>

<div id='mini-jeux'></div>

## Mini-jeux
Notre jeu est constitué de 4 mini-jeux, voici une brève description de chaque jeux :

<div id='downhill-madness'></div>

### Downhill Madness
<p align="left">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/slope-background.png?raw=true" alt="slope-background" width="100">
</p>
Le ou les joueurs se retrouvent en bas d’une montagne et le premier qui arrive à atteindre le sommet de celle-ci sera désigné vainqueur, cependant faites attention la montagne regorge de surprises telles que des énormes bûches et rochers qui dévalent le chemin menant à l'arrivée. Il vous faudra être le plus attentif possible afin de pouvoir franchir tous ces obstacles et foncer vers la victoire.

#### Règles
Les médailles sont distribuées en fonction de l'ordre d'arrivée des joueurs. Le jeu se termine lorsque tous les joueurs ont atteint le sommet de la montagne ou alors lorsqu'ils sont tous tombés.

#### Contrôles
**PC:** `z`, `q`, `s`, `d` pour se déplacer et `space` pour sauter.

**Manette Xbox:** `joystick gauche` pour se déplacer, le bouton `A` pour sauter.

**Manette Playstation:** `joystick gauche` pour se déplacer, le bouton `X` pour sauter.


#### Gameplay
[Downhill Madness](https://youtu.be/n9X7PCBeY4I)

<div id='trex-track-100m'></div>

### Trex Track (100m)
<p align="left">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/track-and-field-background.png?raw=true" alt="track-and-field-background" width="100">
</p>
Aux apparences trompeuses d’un simple 100m, il vous faudra être minutieux sur le timing afin d’échapper au Trex qui n'hésitera pas à vous stopper dans votre quête vers la médaille d’OR…

#### Règles
Les médailles sont distribuées en fonction de l'ordre d'arrivée des joueurs. Le jeu se termine lorsque tous les joueurs ont atteint la ligne d'arrivée ou lorsque le T-Rex les a rattrapé.

#### Contrôles
**PC:** Alterner la touche `q` et `d` pour courir.

**Manette Xbox:** Alterner `lb` et `rb` pour courir.

**Manette Playstation:** Alterner `l1` et `r1` pour courir.

#### Gameplay
[Trex Track](https://youtu.be/fgDxKULAovg)

<div id='stellar-storm'></div>

### Stellar Storm
<p align="left">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/meteorites-background.png?raw=true" alt="meteorite-background" width="100">
</p>
Les joueurs se retrouvent au beau milieu d’une chute de météorites, heureusement ou pas pour eux ils ont tous réussi à se réfugier sur une immense pierre. Seulement il ne peut rester qu’un seul survivant, ils vont devoir essayer de survivre aux coups de poing des adversaires afin de ne pas tomber dans la lave…

#### Règles
Le dernier survivant remporte la médaille d'or. La médaille d'argent et celle de bronze seront attribuées aux joueurs qui seront morts en dernier.

#### Contrôles
**PC:** `z`, `q`, `s`, `d` pour se déplacer et `space` pour donner un coup de poing.

**Manette Xbox:** `joystick gauche` pour se déplacer et le bouton `A` pour donner un coup de poing.

**Manette Playstation:** `joystick gauche` pour se déplacer, le boutton `X` pour donner un coup de poing.

#### Gameplay
[Stellar Storm](https://youtu.be/38aeldfoHnI)

<div id='savage-soccer-football'></div>

### Savage Soccer (football)
<p align="left">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/football-background.png?raw=true" alt="football-background" width="100">
</p>
Rien de mieux qu’un bon match de foot pour se départager, les joueurs ici pourront se tacler, faire des passes et bien évidemment marquer des buts, à la fin du temps réglementaire l’équipe avec le plus de but remporte la victoire.

#### Règles
L'équipe qui gagne remporte la médaille d'or et celle qui perd remporte la médaille de bronze. En cas d'égalité, les deux équipes remportent la médaille d'argent.

#### Contrôles
Pour Joueur PC: `z`, `q`, `s`, `d` pour se déplacer, `shift` pour faire une passe et `space` pour tirer ou sans ballon pour tacler.

Pour Joueur Manette Xbox: `joystick gauche` pour se déplacer, le bouton `A` pour tirer ou tacler sans ballon et le bouton `B` pour faire une passe.

Pour Joueur Manette Playstation: `joystick gauche` pour se déplacer, le bouton `X` pour tirer ou tacler sans ballon et le bouton `O` pour faire une passe.


#### Gameplay
[Savage Soccer](https://youtu.be/fvJbbfjfkiU)

<div id='développement-du-multijoueur'></div>

## Développement du multijoueur
Un des aspects clef de notre jeu est le multijoueur. En effet, nous avons tourné la totalité de nos mini-jeux autour de celui-ci, et c’est pour cela qu’il est préférable de jouer à plusieurs pour profiter d’une meilleure exprérience.

Pour l’intégrer nous avons décidé de ne pas utiliser de framework tel que Colyseus, qui simplifie grandement le développement d’un tel jeu, car nous voulions comprendre le fonctionnement et l’intégration du multijoueur dans un projet.

Nous avons choisi de faire un jeu en peer-to-peer (avec du recul, une architecture client-serveur aurait été plus facile à intégrer) en utilisant la librairie Peer.js. Cette dernière nous a simplifié la communication et la connexion entre peer.

Implémenter le multijoueur a été beaucoup plus long que prévu mais nous avons appris une multitude de concepts qui nous servirons dans le futur.

<div id='architecture'></div>

### Architecture
Notre architecture est la suivante :
- Un joueur est un host qui agit comme un serveur, ce joueur à l’autorité sur tous les autres clients et il se charge de simuler les inputs des clients et ensuite d’envoyer le résultat de ces simulations aux autres clients.
- Les autres clients quant à eux envoient leurs inputs au host et corrigent les erreurs de simulation.

<div id='prédiction-et-réconciliation'></div>

### Prédiction et réconciliation
Lors des phases de test préliminaires du jeu, nous avons constaté qu'il n’était pas jouable pour les joueurs avec une mauvaise connexion (ping > 100ms) car les mouvements n’étaient pas fluides et réactifs, ce qui rendait l’experience assez frustrante.

Nous nous sommes intéressés à la prédiction côté client. Cette technique permet à l'utilisateur de visualiser instantanément l'effet de ses actions, en simulant localement les inputs envoyées au host. Ensuite, pour garantir la cohérence entre l’état du jeu perçu par le joueur et l’état réel du serveur, nous avons implémenter la réconciliation. Ce processus consiste à corriger les prédictions erronées du client en se basant sur les résultats des simulations effectuées sur le serveur.

<div id='interpolation'></div>

### Interpolation
Et enfin, pour les objets dont la prédiction n’est pas nécessaire, comme les IA dans le jeu “Savage Soccer” ou encore les météorites dans le jeu “Stellar Storm”, il a fallu implémenter l’interpolation afin d’assurer une fluidité visuelle entre les updates.

<div id='réalisation-assets'></div>

## Réalisation Assets

<div id='meshes'></div>

### Meshes
Nous avons réalisé l’ensemble des assets à la main à l'exception des corps des personnages ainsi que les arbres. Concernant les corps il n’y avait pas d’armature (squelette pour animer le personnage) ni texture, nous avons donc utilisé [Mixamo](https://www.mixamo.com/#/) qui les a générés tout seul.

- **Modèle Homme:** [Free3D](https://free3d.com/3d-model/male-base-mesh-6682.html)
- **Modèle Femme:** [Sketchfab](https://sketchfab.com/3d-models/female-base-mesh-b6389ae82f044dbe9945c4dad2cd72ae)
- **Arbre:** [Quaternius](https://quaternius.com/packs/ultimatestylizednature.html)

En ce qui concerne  la modélisation 3D nous avons utilisé 2 logiciels en particulier : [Blender](https://www.blender.org/ ) et [Zbrush](https://www.maxon.net/fr/zbrush).

#### Modélisation Femme
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/femme.png?raw=true" alt="Femme" width="600">
</p>

#### Modélisation Homme
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/homme.png?raw=true" alt="Homme" width="600" heigth="50">
</p>

Blender a été utilisé pour construire les scènes en partant de zéro, modéliser les assets ainsi que pour ajouter les animations à nos personnages.

Zbrush a été utilisé pour l’UV unwrapping et la création de certains assets (cheveux du personnage feminin et maps). L’uv unwrapping est une étape nécessaire et souvent difficile qui nous permet d'aplatir en 2D notre modèle 3D pour y ajouter des textures par la suite. Cela a été facilité par l'utilisation de Zbrush.

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/cheveux.png?raw=true" alt="Cheveux" width="600" heigth="100">
</p>


Quant aux textures, nous avons utilisé [Substance 3D Painter](https://www.adobe.com/fr/products/substance3d-painter.html) qui est un logiciel très semblable à PhotoShop mais pour la 3D.

<div id='réalisation-des-map'></div>

### Réalisation des Map

#### Lobby
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/lobby1.png?raw=true" alt="V1" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/lobby2.png?raw=true" alt="V2" width="600" heigth="100">
</p>

#### Downhill Madness
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/downhill1.png?raw=true" alt="V1" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/downhill2.png?raw=true" alt="V2" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/downhill3.png?raw=true" alt="V3" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/downhill4.png?raw=true" alt="V4" width="600" heigth="100">
</p>

#### Trex Track
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/100m1.png?raw=true" alt="V1" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/100m2.png?raw=true" alt="V2" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/100m3.png?raw=true" alt="V3" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/100m4.png?raw=true" alt="V4" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/100m5.png?raw=true" alt="V5" width="600" heigth="100">
</p>

#### Stellar Storm
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/meteorite_1.png?raw=true" alt="V1" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/meteorite_2.png?raw=true" alt="V2" width="600" heigth="100">
</p>

#### Savage Soccer
<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/foot1.png?raw=true" alt="V1" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/foot2.png?raw=true" alt="V2" width="600" heigth="100">
</p>

<p align="center">
  <img src="https://github.com/gamesonweb/gow-olympic-edition-primal-olympics/blob/main/image/foot3.png?raw=true" alt="V3" width="600" heigth="100">
</p>

<div id='animations'></div>

### Animations
- Les animations de nos personnages proviennent du site : [Mixamo](https://www.mixamo.com/#/).

<div id='sons'></div>

### Sons
- [Lobby Music](https://freesound.org/people/Mrthenoronha/sounds/370294/)
- [T-Rex Track Music](https://freesound.org/people/rodincoil/sounds/271383/)
- [T-Rex Steps](https://freesound.org/people/newlocknew/sounds/677414/)
- [T-Rex Roar](https://freesound.org/people/CGEffex/sounds/96223/)
- [Downhill Madness Music](https://youtu.be/8gGWSVHQ-EE)
- [Stellar Storm Music](https://www.youtube.com/watch?v=gbBjjC-KMgE)

<div id='probleme-connexion'></div>

## Problème de connexion à une partie
**Dans le cas où vous n'arrivez pas à rejoindre un ami:**

Cela peut être dû au fait que votre IP n’est pas visible par les autres pair, ou alors que votre pare-feu bloque les ports nécessaire pour les connexions P2P. Pour corriger ce problème, changez de réseau Wi-Fi ou faites un partage de connexion avec votre téléphone. 

<div id='développé-avec'></div>

## Développé avec
- [![Typescript](https://img.shields.io/badge/Typescript-blue?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
- [![Vite](https://img.shields.io/badge/Vite-B73BFE?style=for-the-badge&logo=vite&logoColor=FFD62E)](https://vitejs.dev/)
- [![Babylon.js](https://img.shields.io/badge/Babylon.js-C64A44?style=for-the-badge)](https://www.babylonjs.com/)

<div id='logiciels-utilisés'></div>

## Logiciels utilisés
- [![WebStorm](https://img.shields.io/badge/WebStorm-0099FF?style=for-the-badge&logo=webstorm&logoColor=white)](https://www.jetbrains.com/fr-fr/webstorm/)
- [![VSCode](https://img.shields.io/badge/Visual%20Studio%20Code-0696EA?style=for-the-badge&logo=visualstudiocode&logoColor=white)](https://code.visualstudio.com/)
- [![Blender](https://img.shields.io/badge/Blender-FE8200?style=for-the-badge&logo=blender&logoColor=white)](https://www.blender.org)
- [![ZBrush](https://img.shields.io/badge/ZBrush-red?style=for-the-badge)]([https://www.blender.org](https://www.maxon.net/fr/zbrush))
- [![Adobe](https://img.shields.io/badge/Adobe-F44336?style=for-the-badge&logo=adobe&logoColor=white)](https://www.adobe.com/fr/)

<div id='vidéos-de-développement'></div>

## Vidéos de développement
- [google drive](https://drive.google.com/drive/folders/1hx7jP3G8LzwlBApcsY6VHusVYh8Cht4D)
