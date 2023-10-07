# Application de Chat MultiPDF

## Introduction
------------
L'application de Chat MultiPDF est une application Python qui vous permet de discuter avec plusieurs documents PDF. Vous pouvez poser des questions sur les PDF en utilisant un langage naturel, et l'application fournira des réponses pertinentes en fonction du contenu des documents. Cette application utilise un modèle de langage pour générer des réponses précises à vos questions. Veuillez noter que l'application ne répondra qu'aux questions liées aux PDF chargés.

## Comment Ça Marche
------------

![Schéma de l'Application de Chat MultiPDF](./docs/PDF-LangChain.jpg)

L'application suit ces étapes pour fournir des réponses à vos questions :

1. Chargement des PDF : L'application lit plusieurs documents PDF et extrait leur contenu textuel.

2. Fragmentation du Texte : Le texte extrait est divisé en petits fragments qui peuvent être traités efficacement.

3. Modèle de Langage : L'application utilise un modèle de langage pour générer des représentations vectorielles (embeddings) des fragments de texte.

4. Recherche de Similarités : Lorsque vous posez une question, l'application la compare avec les fragments de texte et identifie les plus similaires sémantiquement.

5. Génération de Réponses : Les fragments sélectionnés sont transmis au modèle de langage, qui génère une réponse en fonction du contenu pertinent des PDFs.

## Dépendances et Installation
----------------------------
Pour installer l'Application de Chat MultiPDF, suivez ces étapes :

1. Clonez le dépôt sur votre machine locale.

2. Installez les dépendances requises en exécutant la commande suivante :
   ```
   pip install -r requirements.txt
   ```

3. Obtenez une clé d'API d'OpenAI et ajoutez-la au fichier `.env` dans le répertoire du projet.
```commandline
OPENAI_API_KEY=your_secrit_api_key
```

## Utilisation
-----
Pour utiliser l'Application de Chat MultiPDF, suivez ces étapes :

1. Assurez-vous d'avoir installé les dépendances requises et ajouté la clé d'API d'OpenAI dans le fichier `.env`.

2. Exécutez le fichier `main.py` en utilisant la CLI de Streamlit. Exécutez la commande suivante :
   ```
   streamlit run test1.py
   ```

3. L'application s'ouvrira dans votre navigateur par défaut, affichant l'interface utilisateur.

4. Chargez plusieurs documents PDF dans l'application en suivant les instructions fournies.

5. Posez des questions en langage naturel sur les PDF chargés en utilisant l'interface de chat.

## Contribution
------------
Ce dépôt est destiné à des fins éducatives et n'accepte pas d'autres contributions. Il sert de matériel de soutien pour un tutoriel YouTube qui montre comment construire ce projet. N'hésitez pas à utiliser et à améliorer l'application en fonction de vos propres besoins.

## Licence
-------
L'Application de Chat MultiPDF est publiée sous la [Licence MIT](https://opensource.org/licenses/MIT).




------------------
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
   streamlit run test1.py
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
