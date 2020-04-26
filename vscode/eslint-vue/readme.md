# ⚠️ Description 

**Ces configurations sont pour un développement sous Vue.**
- Eslint : .eslintrc.json
- Prettier : .prettierrc



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


---

# .PrettierRC

C'est dans ce fichier qu'on configure les règles de style dans le code.
Par exemple, on définir le reformattage des *"* en *'*.