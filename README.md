# Ollama & Qlik Sense Advanced Analytics

Ce projet vise à exploiter la puissance des modèles de langage via [Ollama](https://ollama.com/) pour réaliser de l’**advanced analytics** avec [Qlik Sense Client Managed](https://help.qlik.com/fr-FR/sense/February2023/Content/Sense_Helpsites/Client-Managed.htm).

Il permet d'automatiser des analyses avancées, de générer des insights ou des recommandations, et d’enrichir vos applications Qlik Sense avec des résultats provenant de modèles IA.

## Fonctionnalités principales

- **Intégration Ollama** : Utilisez des modèles de langage (LLM) localement pour le traitement, l’analyse ou la génération de texte.
- **Advanced Analytics avec Qlik Sense** : Connectez vos applications Qlik Sense Client Managed à des scripts Python pour enrichir vos visualisations avec des analyses statistiques, du NLP, du scoring, etc.
- **Automatisation** : Exécutez des workflows d’analyse avancée en interaction avec vos données Qlik Sense.

## Cas d’usage

- Génération automatique de commentaires ou d’explications à partir de vos dashboards Qlik Sense.
- Détection d’anomalies ou prédictions basées sur vos jeux de données Qlik.
- Enrichissement des visualisations avec des scores ou des clusters calculés en Python.
- Chatbot analytique intégré à Qlik Sense.

## Prérequis

- Python 3.8 ou supérieur
- [pip](https://pip.pypa.io/en/stable/)
- Qlik Sense Client Managed (accès développeur ou API)
- [Ollama installé sur votre machine](https://ollama.com/download)

## Installation

### 1. Clonez le dépôt

```bash
git clone https://github.com/votre-utilisateur/ollama-qlik-advanced-analytics.git
cd ollama-qlik-advanced-analytics
```

### 2. Créez et activez un environnement virtuel

Sous Linux/macOS :

```bash
python3 -m venv venv
source venv/bin/activate
```

Sous Windows :

```bat
python -m venv venv
venv\Scripts\activate
```

### 3. Installez les dépendances Python

```bash
pip install -r requirements.txt
```

## Exemple d’utilisation

### 1. Lancer Ollama

Assurez-vous qu’Ollama est lancé sur votre machine.

### 2. Exécuter un script d’analytics avancé

```bash
python scripts/qlik_advanced_analytics.py --app "NomApplication" --sheet "NomFeuille" --model llama2
```

Ce script :
- Récupère des données de Qlik Sense via l’API REST,
- Exécute une analyse avancée avec un LLM Ollama,
- Retourne les résultats ou les insère dans Qlik Sense.

> **Astuce :** Consultez le dossier `scripts/` pour des exemples de scripts d’intégration Qlik Sense.

### 3. Intégration avec Qlik Sense

Pour utiliser les résultats dans Qlik Sense :
- Utilisez l’Advanced Analytics Connector (Python SSE) ou l’API REST.
- Consommez les résultats dans vos visualisations ou extensions.

## Documentation

- [Ollama - Documentation](https://ollama.com/docs)
- [Qlik - Advanced Analytics Integration](https://help.qlik.com/fr-FR/sense/February2023/Subsystems/Hub/Content/Sense_Hub/AdvancedAnalytics/aa-python-connector.htm)
- [Qlik - API REST](https://help.qlik.com/fr-FR/sense-developer/February2023/Subsystems/RepositoryServiceAPI/Content/Sense_RepositoryServiceAPI/RepositoryServiceAPI-Connect-REST.htm)

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.
