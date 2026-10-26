# Pràctica 1: Git Flow

**Sistemes de Control de Versions**

Maria Emilia Navalón Vidal · IES L'Estació · Desplegament d'Aplicacions WEB · 2 CFGS DAW Semi

**URL del repositori:** [https://github.com/Miriam-Nav/practica-gitflow](https://github.com/Miriam-Nav/practica-gitflow)

---

## Introducció

Git és un sistema de control de versions distribuït que registra els canvis realitzats en els fitxers d'un projecte, permet tornar a versions anteriors i facilita el treball simultani de diverses persones.

Git Flow és una metodologia de ramificació basada en Git que defineix branques amb funcions concretes: `main` (versions publicades), `develop` (integració del desenvolupament), `feature/*` (cada funcionalitat nova), `release/*` (preparació d'una versió) i `hotfix/*` (correccions urgents sobre una versió publicada).

---

## 1. Usuari 1: creació del repositori i estructura inicial

L'usuari 1 inicialitza git flow amb la configuració per defecte, descarrega el boilerplate HTML5 i prepara l'estructura inicial de la pàgina. Després fa el commit inicial sobre `develop`.

<img width="532" height="310" alt="captura-04" src="https://github.com/user-attachments/assets/a00bf656-d1f3-48df-8742-846d7084774e" />

<img width="835" height="165" alt="captura-05" src="https://github.com/user-attachments/assets/34d58e98-839e-441b-893c-90ec37dbfb51" />

<img width="976" height="911" alt="captura-03" src="https://github.com/user-attachments/assets/2c10543b-23d1-424b-8719-45dd81e59676" />

<img width="812" height="440" alt="img19" src="https://github.com/user-attachments/assets/d13dc3e5-84c0-4aab-af4f-51110eacf4db" />

<img width="809" height="180" alt="captura-06" src="https://github.com/user-attachments/assets/ae1cc29c-ab56-4e34-a21b-3eaf8d761ab8" />


---

## 2. Usuari 2: features contingutHTML i atributsHTML

L'usuari 2 crea dos features, una per cada secció que ha d'implementar. Cada feature es crea amb `git flow feature start`, es confirma amb un commit i es tanca amb `git flow feature finish`, que la fusiona amb `develop` i elimina la branca.

### Feature contingutHTML

<img width="697" height="217" alt="captura-07" src="https://github.com/user-attachments/assets/7ed4270b-05af-460d-87db-58d048ab75d0" />

<img width="732" height="96" alt="captura-08" src="https://github.com/user-attachments/assets/02e93a77-97a3-4d48-b8a7-4526c135952f" />

<img width="735" height="273" alt="captura-10" src="https://github.com/user-attachments/assets/d7ffb7c9-f4de-40b8-9cc5-b1ef684e763e" />

### Feature atributsHTML

<img width="669" height="229" alt="captura-11" src="https://github.com/user-attachments/assets/3fc3bc49-c9b4-4a31-9917-c2229eec0460" />

<img width="734" height="89" alt="captura-12" src="https://github.com/user-attachments/assets/b48f0ea2-9363-42cc-b036-eb937d9217ae" />

<img width="734" height="267" alt="captura-13" src="https://github.com/user-attachments/assets/d19be97d-1603-41fe-a9c1-e6c39343b42e" />

### Resultat index.html

<img width="889" height="249" alt="img31" src="https://github.com/user-attachments/assets/c1e1e77e-3eb6-475c-a46c-4a4e0c6b5e2e" />

<img width="993" height="277" alt="img34" src="https://github.com/user-attachments/assets/df2f73a3-f980-42cb-b718-69361fa50559" />

<img width="733" height="898" alt="captura-14" src="https://github.com/user-attachments/assets/f998493c-386f-47c1-b636-788737d1b16c" />

---

## 3. Usuari 3: feature estilsCSS i release v1.0

L'usuari 3 crea la feature estilsCSS per a la seua secció i, una vegada integrada en `develop`, crea una release amb totes les features i l'etiqueta com a v1.0.

### Feature estilsCSS

<img width="739" height="93" alt="captura-15" src="https://github.com/user-attachments/assets/cb60c840-339c-46d2-ad87-4828cfdff03b" />

<img width="728" height="250" alt="captura-16" src="https://github.com/user-attachments/assets/8d6aff4a-b160-4b6c-98dd-57b911fd3558" />

<img width="912" height="257" alt="img40" src="https://github.com/user-attachments/assets/56f62376-628d-4028-87a1-92205b57df66" />

<img width="761" height="596" alt="img43" src="https://github.com/user-attachments/assets/060223fd-c7ed-4215-a416-45650860f59b" />


### Release v1.0

<img width="642" height="236" alt="captura-17" src="https://github.com/user-attachments/assets/279675d0-bf1e-46a1-a3ee-28895635dee1" />

<img width="734" height="656" alt="captura-18" src="https://github.com/user-attachments/assets/45255ac9-f27e-4475-825d-31016b59f9c8" />

---

## 4. Usuari 1: hotfix milloresV_1_0

L'usuari 1, que s'encarrega de les proves, decideix millorar la secció de contingut creada per l'usuari 2. Per a això crea un hotfix (`hotfix/milloresV_1_0`) amb `git flow hotfix start`, hi fa la millora i el tanca amb `git flow hotfix finish`.

<img width="736" height="94" alt="captura-20" src="https://github.com/user-attachments/assets/2e142456-caf1-40a3-943a-a959d42c2544" />

### Resultat de la millora

A partir d'ara, per a veure una secció cal prémer el seu botó corresponent de la barra de navegació.

<img width="523" height="221" alt="img51" src="https://github.com/user-attachments/assets/36b58c40-98f6-4239-b96a-08a972118d32" />

<img width="818" height="818" alt="captura-27" src="https://github.com/user-attachments/assets/71c95f06-414f-4eb5-b322-fa94d8c1aec1" />

### Tancament del hotfix

El primer intent de `git flow hotfix finish` falla perquè falta el missatge de l'etiqueta. Es torna a executar amb l'opció `-m` i el hotfix es fusiona amb `main` i amb `develop`, queda etiquetat i la branca s'elimina.

<img width="736" height="207" alt="captura-21" src="https://github.com/user-attachments/assets/79038b36-979f-4815-a47c-ee9a8faeef31" />

<img width="737" height="276" alt="captura-22" src="https://github.com/user-attachments/assets/c1271b22-b144-4f4d-a4de-f2e8ec72e6b5" />

### Pujada de les branques i les etiquetes a GitHub

<img width="559" height="391" alt="captura-23" src="https://github.com/user-attachments/assets/0ad9d1e6-9967-4330-a14b-cbe0791fa14c" />

---

## 5. Documentació en gh-pages i projecte de GitHub

La documentació del procés s'inclou en la branca `gh-pages` del repositori, que es publica amb GitHub Pages. També es crea un projecte de GitHub amb les features i el hotfix creats, i es dona accés com a col·laborador al professor.

<img width="912" height="283" alt="img00" src="https://github.com/user-attachments/assets/76b8d2e0-3f9a-4888-9a19-451cd836e656" />

### Branca gh-pages i GitHub Pages

<img width="732" height="380" alt="captura-24" src="https://github.com/user-attachments/assets/9f5a6d8b-8210-4902-8197-b1d0910c5616" />

<img width="967" height="948" alt="captura-25" src="https://github.com/user-attachments/assets/f4374b4c-f651-49c4-bd09-5f8d60a07c4b" />

### Projecte de GitHub

<img width="1623" height="598" alt="captura-26" src="https://github.com/user-attachments/assets/beb35ca8-92ac-48b7-9a8b-cdd6ef52cadc" />

