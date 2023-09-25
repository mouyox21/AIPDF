Chatbot avec Intelligence Artificielle pour l'Analyse de Multi-Fichiers PDF
Ce dépôt GitHub contient le code source de l'application Chatbot avec Intelligence Artificielle (IA) que nous avons développée pour l'analyse de plusieurs fichiers PDF. Cette application permet aux utilisateurs d'interagir avec un chatbot alimenté par l'IA pour extraire des informations et effectuer des analyses approfondies sur des fichiers PDF.

Table des Matières
Aperçu
Technologies Utilisées
Installation
Utilisation
Contributions
Licence
Aperçu
Notre application Chatbot avec Intelligence Artificielle a été développée dans le cadre de [insérer le nom de votre projet ou de votre rapport ici]. Elle utilise des modèles de langage avancés et des techniques de traitement de documents pour permettre aux utilisateurs d'extraire des informations pertinentes à partir de fichiers PDF, de poser des questions et d'obtenir des réponses basées sur le contenu des documents.

Technologies Utilisées
L'application repose sur les technologies suivantes :

Streamlit : Une bibliothèque Python pour créer des applications web interactives.
OpenAI GPT-3 : Un modèle de langage avancé utilisé pour la génération de réponses du chatbot.
LangChain : Une bibliothèque de traitement du langage naturel (NLP) utilisée pour diverses tâches de traitement de texte.
Installation
Pour exécuter localement cette application, suivez ces étapes :

Clonez ce dépôt GitHub sur votre machine locale en utilisant la commande suivante :

bash
Copy code
git clone https://github.com/votre-nom/chatbot-analyse-pdf.git
Accédez au répertoire du projet :

bash
Copy code
cd chatbot-analyse-pdf
Installez les dépendances Python nécessaires :

bash
Copy code
pip install -r requirements.txt
Exécutez l'application avec Streamlit :

bash
Copy code
streamlit run app.py
L'application devrait maintenant être accessible localement dans votre navigateur.

Utilisation
[Insérez ici des instructions détaillées sur la façon d'utiliser l'application, en mettant en évidence ses fonctionnalités et ses avantages.]
Contributions
Les contributions à ce projet sont les bienvenues. Si vous souhaitez contribuer, veuillez suivre ces étapes :

Créez une branche pour votre contribution :

bash
Copy code
git checkout -b feature/nouvelle-fonctionnalite
Effectuez vos modifications et ajoutez-les au suivi :

bash
Copy code
git add .
Validez vos modifications :

bash
Copy code
git commit -m "Ajout de la nouvelle fonctionnalité"
Poussez vos modifications vers votre branche :

bash
Copy code
git push origin feature/nouvelle-fonctionnalite
Soumettez une demande d'extraction (pull request) pour vos modifications.

Nous examinerons votre contribution dès que possible.

Licence
Ce projet est sous licence [insérez le nom de la licence ici]. Pour plus de détails, consultez le fichier LICENSE.
# MultiPDF Chat App


## Introduction
------------
The MultiPDF Chat App is a Python application that allows you to chat with multiple PDF documents. You can ask questions about the PDFs using natural language, and the application will provide relevant responses based on the content of the documents. This app utilizes a language model to generate accurate answers to your queries. Please note that the app will only respond to questions related to the loaded PDFs.

## How It Works
------------

![MultiPDF Chat App Diagram](./docs/PDF-LangChain.jpg)

The application follows these steps to provide responses to your questions:

1. PDF Loading: The app reads multiple PDF documents and extracts their text content.

2. Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

3. Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

## Dependencies and Installation
----------------------------
To install the MultiPDF Chat App, please follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Obtain an API key from OpenAI and add it to the `.env` file in the project directory.
```commandline
OPENAI_API_KEY=your_secrit_api_key
```

## Usage
-----
To use the MultiPDF Chat App, follow these steps:

1. Ensure that you have installed the required dependencies and added the OpenAI API key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:
   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Load multiple PDF documents into the app by following the provided instructions.

5. Ask questions in natural language about the loaded PDFs using the chat interface.

## Contributing
------------
This repository is intended for educational purposes and does not accept further contributions. It serves as supporting material for a YouTube tutorial that demonstrates how to build this project. Feel free to utilize and enhance the app based on your own requirements.

## License
-------
The MultiPDF Chat App is released under the [MIT License](https://opensource.org/licenses/MIT).
