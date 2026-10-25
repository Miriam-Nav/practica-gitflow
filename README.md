# Pràctica 1: Git Flow - Sistemes de Control de Versions

**Alumna:** Maria Emilia Navalón Vidal  
**Institut:** IES L’Estació  
**Mòdul:** Desplegament d'Aplicacions WEB (2 CFGS DAW Semi)  
**URL del repositori:** https://github.com/Miriam-Nav/practica-gitflow  

---

## Introducció teòrica

**Git** és un sistema de control de versions distribuït que registra els canvis realitzats en els fitxers d'un projecte, permet tornar a versions anteriors i facilita el treball simultani de diverses persones.

**Git Flow** és una metodologia de ramificació basada en Git que defineix branques amb funcions concretes: `main` (versions publicades), `develop` (integració del desenvolupament), `feature/*` (cada funcionalitat nova), `release/*` (preparació d'una versió) i `hotfix/*` (correccions urgents sobre una versió publicada).

S'utilitza en aquest projecte perquè ordena el treball d'un equip de tres persones: cada usuari desenvolupa la seua part en una branca pròpia, les versions s'etiqueten de forma controlada i les correccions urgents no interrompen el desenvolupament.

---

## Desenvolupament de la pràctica

### 1. Usuari 1: Creació del repositori i estructura inicial
L'usuari 1 clona el repositori creat a GitHub, inicialitza git flow amb la configuració per defecte (branques main i develop), descarrega el boilerplate HTML5 i prepara l'estructura inicial de la pàgina (capçalera, barra de navegació amb Home i footer). Després fa el commit inicial sobre develop.

[Inserta aquí la captura: git push de les branques main i develop a GitHub]

### 2. Usuari 2: Features contingutHTML i atributsHTML
L'usuari 2 crea dues features, una per cada secció que ha d'implementar. Cada feature es crea amb `git flow feature start`, es confirma amb un commit i es tanca amb `git flow feature finish`, que la fusiona amb develop i elimina la branca.

**Feature contingutHTML:**
[Inserta aquí la captura: feature contingut HTML]

**Feature atributsHTML:**
[Inserta aquí la captura: feature atributs HTML]

### 3. Usuari 3: Feature estilsCSS i release v1.0
L'usuari 3 crea la feature `estilsCSS` per a la seua secció i, una vegada integrada en develop, crea una release amb totes les features i l'etiqueta com a `v1.0` (`git flow release start` i `git flow release finish`, que fusiona la release amb main i amb develop).

**Feature estilsCSS:**
[Inserta aquí la captura: git flow feature start estilsCSS]

**Release v1.0:**
[Inserta aquí la captura: etiqueta v1.0 creada (git tag) i pujada a GitHub]

### 4. Usuari 1: Hotfix milloresV_1_0
L'usuari 1, que s'encarrega de les proves, decideix millorar la secció de contingut creada per l'usuari 2. Per a això crea un hotfix (`hotfix/milloresV_1_0`) amb `git flow hotfix start`, hi fa la millora i el tanca amb `git flow hotfix finish`.

[Inserta aquí la captura: git flow hotfix start milloresV_1_0]
[Inserta aquí la captura: commit de la millora]
[Inserta aquí la captura: git flow hotfix finish milloresV_1_0]

### 5. Documentació en gh-pages i projecte de GitHub
La documentació del procés s'inclou en la branca `gh-pages` del repositori (GitHub Pages). A més, es crea un projecte de GitHub on es dona accés com a col·laborador a l'usuari `antoni-gimenez`, amb les features i el hotfix creats.

[Inserta aquí la captura: col·laborador antoni-gimenez afegit al projecte]
[Inserta aquí la captura: features i hotfix com a elements del projecte]
[Inserta aquí la captura: documentació publicada en gh-pages (GitHub Pages)]