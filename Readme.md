# appvuesimple
 Api_card_magic

 # Liens api
 https://api.magicthegathering.io/v1/cards
 
Chaque image à un liens permettant de lire les description de chaque carte.
Elle effectue une requête HTTP vers l'API Magic: The Gathering pour obtenir une liste de cartes et affiche des informations sur une carte sélectionnée. L'utilisateur peut parcourir la liste de cartes en cliquant sur les boutons "Précédent" et "Suivant" ou en entrant un nombre dans le champ de saisie et en appuyant sur Entrée. Le nom et l'image de la carte sont affichés sur la page, et en cliquant sur l'image, l'utilisateur accède à l'URL de l'image de la carte.(Limite à 67 pour l'instant)

L'application a une propriété de données cards qui contient la liste de cartes, une propriété de données CardIndex qui suit l'index de la carte actuellement sélectionnée, une propriété de données apiURL qui contient l'URL de base de l'API Magic: The Gathering et une méthode fetchDataPromise.

La méthode fetchDataPromise effectue une requête HTTP GET vers l'API Magic: The Gathering en utilisant Axios et stocke la liste de cartes dans la propriété de données cards. Elle est appelée lors de la création de l'application et lorsque la propriété de données currentBranch change.
