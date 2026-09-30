# KickOff

Gestionnaire de championnat de football en console, écrit en Java. Projet fil rouge du module de Programmation Orientée Objet : l'application grossit à chaque séance de cours.

## Structure

```
KickOff/
├── src/          code source Java
├── docs/
│   └── uml/      diagrammes draw.io (.drawio) et exports PNG
├── data/         fichiers CSV de sauvegarde (non versionnés)
└── README.md
```

## Compiler et exécuter

Prérequis : JDK 21 (`java -version` et `javac -version` doivent répondre).

```bash
# compiler tout le code vers le dossier out/
javac -d out $(find src -name "*.java")

# exécuter (remplacer Main par la classe qui contient main)
java -cp out Main
```

Sous Windows PowerShell :

```powershell
javac -d out (Get-ChildItem -Recurse src -Filter *.java).FullName
java -cp out Main
```

## Progression

- [ ] Phase 0 : environnement et syntaxe (calculateur de points et de classement en console)
- [ ] Phase 1 : classes, encapsulation, UML, héritage, polymorphisme (Equipe, Joueur, Attaquant, Gardien)
- [ ] Phase 2 : composition, références, objets immuables (effectif, Score, Match)
- [ ] Phase 3 : classes abstraites et interfaces (Joueur abstrait, Classable, Comparable)
- [ ] Phase 4 : exceptions
- [ ] Phase 5 : collections (Championnat, calendrier, classement)
- [ ] Phase 6 : entrées/sorties, Javadoc, finition

## Conventions

- Classes en `PascalCase`, méthodes et variables en `camelCase`, constantes en `MAJUSCULES`.
- Un fichier = une classe publique.
- Fields `private` par défaut, `@Override` sur chaque redéfinition.
- Un commit par étape, UML avant le code.
