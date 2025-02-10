0-current_working_directory : pwd pour afficher le repertoire courant
1-listit : ls pour afficher la liste des fichiers du repertoire courant
2-bring_me_home : cd pour ramener au repertoire origine
3-listfiles :(ls -l) pour afficher la liste detaillee des fichiers
4-listmorefiles : (ls -la) pour afficher la liste des fichiers et les fichiers caches
5-listfilesdigitonly : (ls -lna) pour afficher la liste de tous les fichiers et ID utilisateur
6-firstdirectory : $mkdir /tmp/my_first_directory : pour creer un repertoire a un ednroit precis
7-movethatfile : $(mv /tmp/betty /tmp/my_first_directory : pour deplacer un fichier d un dossier dans un autre dossier
8-firstdelete : $(rm /tmp/my_first_directory/betty) : supprimer un fichier dans un sous dossier et dossier
9-firstdirdeletion : $(rmdir /tmp/my_first_directory) : supprimer un repertoire dans un autre repertoire
10-back : cd -  pour revenir au repertoire ou on etait precedemment
11-lists : (ls -la . .. /boot) : afficher la liste des fichiers dans le repertoire en cours + fichier caches + fichier repertoire parent + fichiers dans repertoire specifique
12-file_type : file /tmp/iamafile afficher le type de fichier dans un repertoire specifique
13-symbolic_link : ln -s /bin/ls __ls__ pour creer un lien symbolique vers une adresse specifique
14-copy_html : cp -u *html ../ pour copier tous les fichiers qui ont une extension dans le repertoire parent
15-lets_move : mv [A-Z]* /tmp/u pour deplacer tous les fichiers dont la premiere lettre est une majuscule dans un dossier specifique
16-clean_emacs : rm *~ pour supprimer tous les fichiers qui ont un ~
17-tree : mkdir -p welcome/to/school : pour creer en une seule commande plusieurs repertoire imbriques les uns dans les autres 