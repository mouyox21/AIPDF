# PDF Profiler - Développement d'un Assistant IA pour l'Analyse des Documents PDF

## Introduction
------------
   PDF Profiler est une puissante application Python qui vous permet d'analyser et d'explorer des fichiers PDF de manière approfondie. Vous pouvez extraire des informations pertinentes, générer des statistiques, et même poser des questions en langage naturel sur les PDF chargés. Cette application repose sur un modèle de langage avancé pour vous fournir des réponses précises. Veuillez noter que l'application répondra uniquement aux questions liées aux PDFs que vous avez chargés.

## Fonctionnement
------------

![Schéma de Fonctionnement de PDF Profiler](./docs/PDF-LangChain.jpg)

PDF Profiler suit un processus en plusieurs étapes pour vous offrir une analyse complète de vos fichiers PDF :

1. **Chargement des PDF :** L'application lit et analyse vos fichiers PDF, extrayant leur contenu textuel.

2. **Extraction des Données :** Les données essentielles des PDFs sont extraites et organisées de manière structurée.

3. **Statistiques et Profilage :** PDF Profiler génère des statistiques et des profils détaillés des PDFs chargés, vous permettant de mieux comprendre leur contenu.

4. **Modèle de Langage :** L'application utilise un modèle de langage avancé pour répondre à vos questions et fournir des informations pertinentes.

5. **Réponses aux Questions :** Posez des questions en langage naturel sur les PDFs et obtenez des réponses basées sur leur contenu.

## Dépendances et Installation
----------------------------
Pour installer et utiliser PDF Profiler, suivez ces étapes simples :

1. **Clonez le Répertoire :** Commencez par cloner ce répertoire sur votre machine locale.

2. **Installez les Dépendances :** Installez les dépendances requises en exécutant la commande suivante :
   ```
   pip install -r requirements.txt
   ```

3. **Obtenez une Clé d'API OpenAI :** Vous devez obtenir une clé d'API auprès d'OpenAI et l'ajouter au fichier `.env` dans le répertoire du projet. Voici comment cela doit être fait :
```commandline
OPENAI_API_KEY=your_secret_api_key
```

## Utilisation
-----
Pour utiliser PDF Profiler efficacement, suivez ces étapes :

1. **Configuration :** Assurez-vous d'avoir installé les dépendances requises et ajouté la clé d'API d'OpenAI dans le fichier `.env`.

2. **Lancement de l'Application :** Exécutez le fichier `main.py` en utilisant la CLI de Streamlit. Vous pouvez le faire avec la commande suivante :
   ```
   streamlit run main.py
   ```

3. **Interface Conviviale :** L'application s'ouvrira automatiquement dans votre navigateur par défaut, vous présentant une interface utilisateur conviviale.

4. **Chargement des Documents PDF :** Importez vos fichiers PDF dans l'application en suivant les instructions fournies.

5. **Exploration des PDF :** Utilisez PDF Profiler pour extraire des informations, générer des statistiques et poser des questions sur les PDFs chargés.

## Contributions
------------
Ce dépôt est principalement destiné à des fins éducatives et ne prend pas en charge les contributions externes. Il sert de matériel de support pour un tutoriel YouTube qui explique comment construire ce projet. Néanmoins, n'hésitez pas à utiliser et à personnaliser l'application en fonction de vos besoins particuliers.

## Licence
-------
PDF Profiler est publié sous la [Licence MIT](https://opensource.org/licenses/MIT).
