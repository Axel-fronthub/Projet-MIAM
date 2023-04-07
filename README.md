# Projet-MIAM



Ce projet permet à l'utilisateur de rechercher et de sélectionner des plats à partir d'un fichier JSON. Les plats sélectionnés sont ajoutés à un conteneur avec un bouton pour les supprimer. Le projet utilise une fonction de saisie semi-automatique pour suggérer des plats en fonction du texte saisi par l'utilisateur.



Fonctionnalités :



Le projet contient les fonctionnalités suivantes :

Récupérer les plats à partir d'un fichier JSON (plats.json) et les stocker dans un tableau.

Filtrer les plats en fonction d'un terme de recherche.

Afficher les suggestions de plats en fonction du terme de recherche dans une liste déroulante.

Ajouter la suggestion sélectionnée à un conteneur et créer un élément de formulaire caché pour stocker la valeur de la suggestion sélectionnée pour l'envoyer au serveur.

Supprimer la suggestion sélectionnée du conteneur et du tableau des plats en cliquant sur le bouton de suppression.



Fonctions principales :



getPlats(): Récupère les plats à partir du fichier plats.json et retourne un tableau d'objets contenant les données des plats.

filterPlats(plats, searchTerm): Filtre les plats en fonction d'un terme de recherche et retourne un tableau de plats qui contiennent le terme de recherche dans leur nom.

addSelectedSuggestion(suggestion, container, inputId): Ajoute la suggestion sélectionnée au conteneur, crée un élément de formulaire caché pour stocker la valeur de la suggestion sélectionnée, et ajoute un bouton pour supprimer la suggestion sélectionnée.

displaySuggestions(suggestions, datalistElement, inputElement, selectedContainer): Affiche les suggestions dans la liste déroulante et ajoute un écouteur d'événements pour détecter lorsque l'utilisateur sélectionne un plat.

setupAutocomplete(inputElement): Configure la saisie semi-automatique pour un champ texte donné.



Utilisation :



Incluez le code JavaScript dans votre fichier HTML.

Ajoutez des champs texte avec des identifiants uniques et des éléments de liste déroulante et de conteneur associés.

Appelez la fonction setupAutocomplete() pour chaque champ texte pour configurer la saisie semi-automatique.



