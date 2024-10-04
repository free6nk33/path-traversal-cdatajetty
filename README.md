Ce script Bash permet de tester une liste de domaines pour détecter une éventuelle exposition de clés AWS (AKIA keys) en exploitant une vulnérabilité sur les endpoints accessibles via une requête particulière.
Fonctionnalités :

Test sur des domaines multiples : Le script lit un fichier contenant une liste de domaines et envoie une requête à chacun d'eux pour essayer d'extraire des informations sensibles.
Extraction de clés AWS (AKIA) : Il cherche spécifiquement des clés AWS dans la réponse de chaque requête.
Sortie dans un fichier : Les clés AWS trouvées sont enregistrées dans un fichier de sortie spécifié par l'utilisateur.
Vérification des réponses HTTP : Le script vérifie si la requête est réussie et gère les erreurs éventuelles.

Utilisation :

    ./exp.sh <fichier_de_domaines> <fichier_de_sortie>

<fichier_de_domaines> : Fichier contenant une liste de domaines à tester.
<fichier_de_sortie> : Fichier où seront stockées les clés AWS trouvées.
