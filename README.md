# Rééquilibrage des stations de vélos partagés
Dans une ville comme Nancy, les systèmes de vélos en libre-service sont largement utilisés pour des trajets urbains courts. Cependant, la gestion des stocks de vélos entre les différentes stations est cruciale pour offrir un service de qualité.

# Contexte du projet
En tant que futur développeur en IA, vous allez concevoir et développer une interface interactive qui intègre les données des stations de vélos partagés de Nancy via l'API de JCDecaux.
Vous allez utiliser les données d'OpenStreetMap avec OSMnx pour représenter les stations sur une carte interactive avec Folium et optimiser le chemin entre stations avec NetworkX.
L'application permettra de visualiser les stations surchargées ou sous-alimentées et indiquera aux utilisateurs à déplacer les vélos en fonction des besoins

# jcDecauxApi
API Python pour interagir avec le service de vélos en libre-service de JCDecaux.

## Table des matières

- [Installation](#installation)
- [Utilisation](#utilisation)
- [Fonctionnalités](#fonctionnalités)
- [Contribuer](#contribuer)
- [Licence](#licence)

## Installation

1. Clonez le repository :
    ```sh
    git clone https://github.com/votre-utilisateur/jcDecauxApi.git
    ```
2. Accédez au répertoire du projet :
    ```sh
    cd jcDecauxApi
    ```
3. Créez un environnement virtuel :
    ```sh
    python -m venv venv
    ```
4. Activez l'environnement virtuel :
    - Sur Windows :
        ```sh
        venv\Scripts\activate
        ```
    - Sur macOS/Linux :
        ```sh
        source venv/bin/activate
        ```
5. Installez les dépendances :
    ```sh
    pip install -r requirements.txt
    ```

## Utilisation

1. Obtenez une clé API JCDecaux à partir du site officiel [JCDecaux Developers](https://developer.jcdecaux.com/#/opendata/vls?page=getstarted).

2. Configurez la clé API dans le fichier de configuration ou via une variable d'environnement :
    ```sh
    export JCDECAUX_API_KEY="votre_clé_api"
    ```

3. Pour exécuter le projet, lancez le script principal :
    ```sh
    python main.py
    ```

4. Accédez à l'application via votre navigateur à l'adresse :
5. http://localhost:5000 

## Fonctionnalités

- Récupération des informations des stations de vélos.
- Vérification de la disponibilité des vélos et des places libres.
- Localisation des stations sur une carte.

## Contribuer

Les contributions sont les bienvenues ! Veuillez suivre les étapes suivantes pour contribuer :

1. Forkez le repository.
2. Créez une nouvelle branche :
    ```sh
    git checkout -b feature/nom-de-la-fonctionnalité
    ```
3. Faites vos modifications et committez-les :
    ```sh
    git commit -m "Ajout de la fonctionnalité X"
    ```
4. Pushez vers la branche :
    ```sh
    git push origin feature/nom-de-la-fonctionnalité
    ```
5. Ouvrez une Pull Request.