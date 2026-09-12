========================================
6GEI311 - Architecture des logiciels
Laboratoire 1 - ReadMe
Nom de l'etudiant : THOROUM_DJASRA_WILSON
Date : 11 septembre 2026
========================================

--- RESUME DE CE QUI A ETE APPRIS ---

Ce laboratoire m'a permis de me familiariser avec les bases de la gestion de
version avec Git et GitHub dans un contexte de collaboration en equipe.
J'ai appris a :
- Creer, cloner et synchroniser un repository distant avec un repository local.
- Creer et utiliser des branches pour isoler le travail d'un collaborateur
  sans affecter la branche principale.
- Fusionner (merge) les modifications d'un collaborateur dans la branche
  principale apres validation.
- Visualiser l'historique complet d'un repository (git log) pour suivre
  l'evolution du code et identifier les contributions de chaque membre.
- Diagnostiquer et corriger des situations problematiques : rendre un projet
  local accessible via GitHub, et revenir a une version fonctionnelle apres
  l'introduction d'une erreur, tout en conservant les changements valides
  effectues apres l'erreur.
- Rediger une issue claire et exploitable pour signaler un probleme a un
  collaborateur.

--- GIT CHEAT-SHEET ---

Initialisation / connexion
  git init                        Initialise un repository local
  git clone <url>                 Clone un repository distant
  git clone -b <branche> <url>    Clone une branche specifique
  git remote add origin <url>     Lie un repo local a un repo distant
  git remote -v                   Affiche les remotes configures

Travail quotidien
  git status                      Affiche l'etat des fichiers
  git add <fichier>                Ajoute un fichier a la zone de staging
  git add .                       Ajoute tous les fichiers modifies
  git commit -m "message"         Cree un commit avec un message descriptif
  git push origin <branche>       Envoie les commits locaux vers le distant
  git pull origin <branche>       Recupere et fusionne les changements distants
  git fetch                       Recupere les changements distants sans fusionner

Branches
  git branch                      Liste les branches locales
  git branch -m <nom>             Renomme la branche courante
  git checkout <branche>          Change de branche
  git checkout -b <branche>       Cree une branche et bascule dessus
  git merge <branche>             Fusionne une branche dans la branche courante
  git branch -d <branche>         Supprime une branche locale

Historique / retour en arriere
  git log --oneline               Affiche l'historique des commits
  git log --all --graph --decorate --oneline
                                   Affiche l'historique de toutes les branches
  git revert <commit>             Annule un commit en creant un nouveau commit
  git reset --hard <commit>       Ramene la branche a un commit precis

--- RETOUR D'EXPERIENCE : DESCRIPTION ET LECTURE D'UNE ISSUE ---

Une bonne description d'issue doit contenir :
- Un titre clair et concis resumant le probleme.
- Le contexte : ou se trouve le probleme (fichier, branche, commit concerne).
- Le comportement observe vs le comportement attendu.
- Les etapes pour reproduire le probleme, si applicable.
- Le numero ou hash du commit ayant introduit le probleme, s'il est connu.

Lors de la lecture d'une issue, il est important de verifier qu'on dispose de
toutes ces informations avant de commencer a investiguer. Une issue bien
ecrite permet de gagner beaucoup de temps et evite les allers-retours
inutiles entre les membres de l'equipe.
