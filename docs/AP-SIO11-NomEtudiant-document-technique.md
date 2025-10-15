# Dossier Technique et Justificatif de Corrections

> **Important** : ce document doit être exporté en PDF lors de la remise finale du dossier. Le nom du fichier exporté devra suivre la nomenclature&nbsp;: `AP-SIO11-NomEtudiant-document-technique.pdf`.

## 1. Format et organisation des livrables
- Archive ZIP à nommer `AP-SIO11-NomEtudiant-mini-site.zip` contenant l'intégralité du mini-site (HTML, CSS, images, scripts).
- Documents justificatifs et rapports au format PDF (par exemple `AP-SIO11-NomEtudiant-document-technique.pdf`).
- Captures d'écran légendées préparées localement (par exemple dans un dossier `img/screenshots/`) puis insérées lors de l'export PDF, sans les ajouter au dépôt Git.
- Lien vers le dépôt Git (si disponible) à indiquer dans la section «&nbsp;Références&nbsp;».

## 2. Corrections et choix techniques
- Mise en place d'une navigation cohérente et responsive partagée entre toutes les pages.
- Ajout d'un formulaire de démonstration commenté sur la page HTML pour expliciter le rôle de chaque balise.
- Mise en forme homogène du formulaire de contact global dans le footer.
- Création d'un mémento des commandes Linux avec stylisation dédiée.
- Ajout d'une page «&nbsp;Dossier à remettre&nbsp;» détaillant les attentes administratives.

## 3. Captures d'écran à produire
Les captures d'écran doivent être ajoutées lors de la mise en page finale du PDF. Afin d'éviter les erreurs «&nbsp;fichiers binaires non pris en charge&nbsp;» lors de la création d'une pull request, ne versionnez pas les fichiers `.png` ou `.jpg` correspondants dans le dépôt Git. Conservez-les localement et insérez-les au moment de l'export PDF.

| Capture attendue | Légende suggérée | Nom de fichier recommandé |
| --- | --- | --- |
| Formulaire HTML commenté | Fig. 1 – Formulaire de démonstration sur la page HTML. | `html-formulaire.png` |
| Tableau des commandes Linux | Fig. 2 – Tableau des commandes Linux et mise en forme dédiée. | `linux-table.png` |
| Formulaire de contact global | Fig. 3 – Formulaire de contact intégré dans le footer commun. | `footer-contact.png` |

### Balises du tableau Linux
- `<table>` : structure le tableau et regroupe toutes les données tabulaires.
- `<caption>` : fournit un titre accessible décrivant le contenu du tableau.
- `<thead>` et `<tbody>` : séparent l'en-tête des lignes de données pour une lecture plus claire.
- `<tr>` : crée une ligne du tableau.
- `<th>` : cellule d'en-tête apportant du sens aux colonnes pour les lecteurs d'écran.
- `<td>` : cellule de données standard contenant la commande, sa description ou son exemple.

## 4. Explication des balises principales du formulaire
- `<form>` : conteneur du formulaire permettant l'envoi des données.
- `<label>` : associe un texte descriptif à un champ de saisie pour l'accessibilité.
- `<input type="text">` : champ de saisie d'une ligne pour le nom.
- `<input type="email">` : champ de saisie validant le format e-mail.
- `<textarea>` : zone de texte multiligne pour les commentaires détaillés.
- `<button type="submit">` : déclenche l'envoi du formulaire.

## 5. Attributs HTML essentiels du formulaire
- **method** : définit la méthode HTTP utilisée (`GET` ou `POST`). `POST` est privilégié pour l'envoi d'informations privées.
- **action** : URL de destination où les données sont envoyées ; peut pointer vers un script serveur ou rester vide pour tester localement.
- **required** : impose la saisie du champ avant soumission, garantissant des données complètes.
- **name** : identifiant du champ côté serveur permettant de récupérer la valeur envoyée.

## 6. Lier un fichier CSS à un fichier HTML
Utiliser `<link rel="stylesheet" href="chemin/vers/style.css">` dans l'en-tête HTML pour séparer contenu et présentation. Cette méthode facilite la maintenance, favorise la réutilisation des styles sur plusieurs pages et réduit la duplication de code.

## 7. Mise en avant des pages créées
Insérer dans le document PDF un aperçu de chaque page finalisée du mini-site. Reprendre les légendes proposées ci-dessous et conserver les fichiers d'origine en dehors du dépôt Git.

| Page à capturer | Légende suggérée | Nom de fichier recommandé |
| --- | --- | --- |
| Page d'accueil | Fig. 4 – Aperçu de la page d'accueil et de la navigation. | `index-page.png` |
| Page HTML | Fig. 5 – Page HTML avec exemples et formulaire commenté. | `html-page.png` |
| Page CSS | Fig. 6 – Page CSS présentant les bonnes pratiques et liens utiles. | `css-page.png` |
| Page Commandes Linux | Fig. 7 – Page dédiée aux commandes Linux. | `linux-page.png` |
| Page En construction | Fig. 8 – Placeholder pour les sections en cours de réalisation. | `en-construction-page.png` |
| Page Dossier à remettre | Fig. 9 – Nouvelle page détaillant les attentes administratives. | `dossier-remise-page.png` |

## 8. Modèle de mail professionnel pour la remise
```
Objet : Remise du dossier Atelier Professionnel – Nom Prénom – Classe

Bonjour,

Veuillez trouver ci-joint le dossier « Atelier Professionnel – Mini-site SISR » comprenant l'archive du site et le document technique.

Je reste à votre disposition pour tout complément d'information.

Cordialement,
Nom Prénom
Classe – BTS SIO
```

## 9. Références
- Dépôt Git : (ajouter l'URL le cas échéant)
- Support de cours HTML/CSS (indiquer les ressources utilisées)

---
**Rappel** : après vérification, exporter ce document en PDF et le placer dans le dossier final nommé selon la convention imposée.
