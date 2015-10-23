#Tuto openClassRoom

Qu'est ce qu'un commit ?

Un commit consiste à sauvegarder par le biais d'un message une modification que l'on a apporté à un fichier (ou dossier...).
C'est à dire que si par exemple vous avez un fichier index.php comportant la ligne :
echo "C'est cool ca";

Que vous le modifier :
echo strtoupper("En majuscule, c'est encore mieux !)";

Cette modification devra être sauvegarde quelque part. C'est la qu'interviendra le commit.
Vous appliqué la commande "git commit -m" suivi d'un message explicite comportant la modification apporté. 
Une fois ceci terminé, le commit est bien visible et permet d'apporter une grande précision sur la modif du fichier. 
De plus chaque commit dispose d'informations intéressante telles que la date d'ajout, ou bien l'email de celui-ci qui l'a crée ainsi qu'un identifiant unique permettant d'accèder à d'autres informations plus poussées.
Bref, vous l'aures compris, le commit est c'est plutôt cool.


A quoi sert la commande git log ?

Etroitement lié aux commits, cette commande va en fait nous permettre d'accèder à la liste de tous les commits réalisés sur le repertoire.
On aura donc accès pour chaque commit, à sa date d'ajout, l'adresse e-mail du créateur, le message du commit, l'identifiant unique du commit.
Cela offre un visuel d'ensemble sur l'avancement d'un projet et ses modifications apportés (d'ou l'importance de réaliser de bons commits bien explicites).


Qu'est-ce qu'une branche ?

Quoi ? Le truc dans les arbres c'est ca ?
Plus serieusement, dans git lorsque l'on crée un repertoire nous somme en fait placés par default sur ce qu'on appelle une branche (la branche master).
C'est donc l'endroit sur lequel on travaille. Et en tant qu'utilisateur on a la possibilité de créer de mutliple branches sur un seul et même projet et de se deplacer sur chacunes d'entre elles, afin de par exemple effectuer des tests sans avoir à affecter notre bracnhe master (branche par default). 
Ca offre donc une flexibilité en terme d'origanisation de travail qui est obligatoire.
Imaginez un projet Git. Par default on part donc avec notre branche master. Seulement, très vite, dans notre équipe, des devs veulent faire des test sur une fonctionnalité en index.php et d'autre devs veulent faire une autre fonctionnalité qui n'a rien à voir mais sur le même fichier.
Vous saisissez ? Sans faire de branche, la, on fonce droit dans le mur et l'enfer abyssal des conflits.
On partira donc sur des branches séparés afin que chacun puisse faire son travail sans avoir à se soucier de conflits.

On aura la branche  :   - master : index.php | style.css
			- fonctionnalité_1 : index.php | style.css
			- fonctionnalité_2 : index.php | style.css

Et la chacun pourra bosser sur l'index.php de sa branche sans avoir à affecter le code de l'autre.

