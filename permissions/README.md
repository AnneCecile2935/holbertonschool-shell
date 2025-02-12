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
10-mirror_permissions : XXXXXXXXXX :  donne les memes autorisations a deux fichiers. ce code doit fonctionner tout le temps, pas que en 664.
11-directories_permissions