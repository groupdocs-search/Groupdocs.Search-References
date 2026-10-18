---
title: "GroupDocs.Search.Common"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "L'espace de noms fournit les classes communes de la bibliothèque."
type: docs
weight: 20
url: /fr/net/groupdocs.search.common/
---
L'espace de noms fournit les classes communes de la bibliothèque.

## Classes

| Classe | Description |
| --- | --- |
| [AttributeChangeBatch](./attributechangebatch) | Représente un conteneur pour les modifications d'attributs. |
| [Cancellation](./cancellation) | Représente un objet permettant de demander l'annulation d'une opération. |
| [ChunkSearchToken](./chunksearchtoken) | Représente un jeton pour la poursuite de la recherche par morceaux (recherche par pages). |
| [CustomExtractorCollection](./customextractorcollection) | Contient une collection d'extracteurs personnalisés. Si la collection contient un extracteur pour une extension de fichier prise en charge par les extracteurs intégrés, alors cet extracteur sera utilisé à la place de celui intégré. |
| [Document](./document) | Représente la classe de base pour les documents ajoutés à un index depuis le système de fichiers, un flux ou une structure. Contient des méthodes statiques pour créer des documents à partir de différents types de sources. |
| [DocumentField](./documentfield) | Représente les données d'un champ de document. |
| [DocumentImage](./documentimage) | Représente les données d'image d'un document. |
| [Encodings](./encodings) | Contient les noms des encodages possibles. |
| [ExtractedData](./extracteddata) | Représente les données récupérées d'un document et préparées pour l'indexation. |
| [ExtractedItemInfo](./extractediteminfo) | Représente les informations d'un élément de conteneur. |
| [ExtractorSettings](./extractorsettings) | Contient les paramètres de l'extracteur de données de document. |
| [FileLogger](./filelogger) | Représente un journal qui enregistre les événements et les erreurs dans un fichier local. |
| [FileOutputAdapter](./fileoutputadapter) | Représente un adaptateur de sortie qui collecte la sortie dans un fichier. |
| [FragmentContainer](./fragmentcontainer) | Représente un conteneur pour les fragments de texte avec les termes trouvés mis en évidence d'un champ de document. |
| [ImageFrame](./imageframe) | Représente une trame d'image. |
| [IndexInfo](./indexinfo) | Contient les informations de base sur un index. |
| [IndexingReport](./indexingreport) | Représente des informations détaillées sur une opération d'indexation. |
| [Notification](./notification) | La classe de base pour toutes les notifications à l'index. Cette classe contient également des méthodes pour créer des objets de notification. |
| [OutputAdapter](./outputadapter) | Représente la classe de base d'un adaptateur de sortie utilisé pour collecter une sortie sous une forme généralisée. Les adaptateurs actuellement disponibles sont [`FileOutputAdapter`](../groupdocs.search.common/fileoutputadapter), [`StreamOutputAdapter`](../groupdocs.search.common/streamoutputadapter), [`StructureOutputAdapter`](../groupdocs.search.common/structureoutputadapter) et [`StringOutputAdapter`](../groupdocs.search.common/stringoutputadapter). |
| [ResultBuilderFactory](./resultbuilderfactory) | Représente la classe de base d'une fabrique de constructeurs de résultats. |
| [SearchImage](./searchimage) | Représente une image à rechercher. |
| [SearchReport](./searchreport) | Représente des informations détaillées sur une opération de recherche. |
| [StreamOutputAdapter](./streamoutputadapter) | Représente un adaptateur de sortie qui collecte la sortie dans un flux. |
| [StringOutputAdapter](./stringoutputadapter) | Représente un adaptateur de sortie qui collecte la sortie sous forme de chaîne. |
| [StructureOutputAdapter](./structureoutputadapter) | Représente un adaptateur de sortie qui collecte la sortie sous forme d'une structure contenant chaque champ séparément. |
| [WordPattern](./wordpattern) | Représente un modèle de mot à utiliser dans la recherche de caractères génériques de mots. |
## Interfaces

| Interface | Description |
| --- | --- |
| [IContainerItemExtractor](./icontaineritemextractor) | Fournit des méthodes pour extraire des éléments des documents conteneurs. |
| [IDocumentLoader](./idocumentloader) | Définit l'interface du chargeur de documents utilisée pour charger des documents paresseux. |
| [IFieldExtractor](./ifieldextractor) | Fournit des méthodes pour extraire des champs d'un document. |
| [ILogger](./ilogger) | Définit l'interface d'un journaliseur utilisé pour consigner les événements et les erreurs dans un index. |
| [IWordSplitter](./iwordsplitter) | Définit une méthode pour diviser le texte en mots individuels. |
## Énumération

| Énumération | Description |
| --- | --- |
| [DocumentSourceKind](./documentsourcekind) | Définit les types de sources de documents. |
| [DocumentStatus](./documentstatus) | Représente l'état de traitement d'un document. |
| [IndexStatus](./indexstatus) | Spécifie l'état d'un index. |
| [VersionUpdateResult](./versionupdateresult) | Représente le résultat d'une opération de mise à jour de version d'index. |

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
