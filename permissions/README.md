0-iam_betty : su betty fait passer de l'utilisateur actuel  un utilisateur betty
1-who_am_i : whoami imprime le nom de l'utilisateur effectif de l'utilisateur actuel
2-groups : groups: imprime tous les groupes dont l'utilisateur actuel fait partie
3-new_owner: $sudo chown betty hello : change le proprietaire du fichier en utilisateur betty
4-empty : touch hello : cree un fichier vide
5-execute : chmod u+x hello : ajoute l'execution au proprietaire pour un fichier
6-multiple_permissions : chmod ug+x,o+r hello : ajoute les autorisations differentes au proprietaire, groupe et autres utilisateurs
7-everybody : chmod ugo+x hello : ajoute l'autorisation d'execution a tous les utilisateurs d'un fichier
8-James_Bond : chmod 007 hello : supprime toutes les autorisations au proprietaire et groupe, ajoute l'autorisation de lecture aux autres utilisateurs
9-John_Doe : chmod 753 hello : donne toutes les autorisations au proprietaire, execution et lecture au groupe et ecriture, execution aux autres utilisateurs
10-mirror_permissions : chmod -R +X . :  donne les memes autorisations a deux fichiers. ce code doit fonctionner tout le temps, pas que en 664. le X au lieu de x permet d'agir que sur les repertoires et sous repertoires. Le "." dit qu'on agit que sur le repertoire courant
11-directories_permissions : chown -R ugo-x /permissions : ajoute l autorisation a tous les utilisateurs en execution sur les sous repertoires d un repertoire sans modifier les autorisations sur les fichiers
12-directory_permissions : mkdir -m 751 my_dir : creer un repertoire et ses autorisations "-m 751 " permet de definir les auto du repertoire au moment de sa creation
13-change-group : chgrp school hello : changer le proprietaire du groupe du fichier hello par school (il faut bien creer le groupe avant)
14-change_owner_and_group : chown -R vincent:staff . : chown pour changer de proprietaire / -R pour changer que sur les repertoires vincent (propriteraire) staff (groupe) <<<<<<changer le proprietaire et le groupe pour le repertoire courant .
15-symbolic_link_permissions : chown -R vincent:staff _hello :creer le lien symbolic avant (ls -n hello _hello) et changer le proprietaire et le groupe
16-if_only : chown --from=guillaume:staff vincent:staff hello : changer le proprietaire si on connait le prorpietaire precedent (ancien proprietaire:groupe) (nouveau proprietaire:groupe)