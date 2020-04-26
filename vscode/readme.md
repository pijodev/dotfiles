# Description

Le contenu de ces fichiers sont à coller dans :   
- le fichier de settings.json de VSCode
- .eslintrc.json du projet 
- .prettierrc du projet

Pour trouver le setting.json dans VSCode, on peut par exemple :

- ctrl+,
- cliquer en haut à droite sur l'icône pour afficher en mode JSON


# Utilité

Cela permet notamment de configurer :   
- les extensions ou les thèmes
- les configurations du Linter
- les configurations du formatteurs Prettier

**Les plugins Eslint et Prettier doivent être installés.**

---

# .EslintRC.JSON

## Membres principaux

### 1. Extends
Eslint récupère étend sa config à ces sources là

### 2. Plugins
Eslint utilise les plugins suivants 

### 3. ParserOptions
J'utilise l'attribut : 
```json
"parserOptions": {
    "sourceType": "module" 
},
```
Pour éviter l'erreur : *"import" est un mot-clé réservé*


### 4. Rules
Mes règles perso qui écrasent celles de la config définie dans Eslint.
*RULES se place en dernier dans le JSON.*

### 5. Validate 
Valide le lint sur les langages définis.
Je ne sais pas encore très bien à quoi ça sert.
Ne peut plus être défini dans le settings.json du VSCode.

### 6. AutoFixOnSave
Ne peut plus être défini dans le settings.json du VSCode.


---

# .PrettierRC

C'est dans ce fichier qu'on configure les règles de style dans le code.
Par exemple, on définir le reformattage des *"* en *'*.