# Le PowerShell  
_______________________  
  
## Histoire rapide  
  
Le **Powershell** est un interpreteur de commande Windows qui a pour but de pouvoir gérer des objet. Ca a été  mis en place par Microsoft en 2006 pour la premiere fois et est toujours disponible sous Win10.  
________________________
  
## Commande de base  
  
### Naviger dans votre ordinateur  
  
**ls** : Vous permet d'afficher les éllement dans le fichier ou vous vous trouvez.  
  
![exemple](https://github.com/Arata34/PowerShell/blob/master/Exemple_ls.PNG)  
  
**cd "Nom d'un fichier"** : Vous permet de rentrer dans le fichier de votre choix.  
  
**cd ..** : Vous fait revenir au fichier d'avant.  
  
### Gestion de fichier  
  
**New-Item -Path . -Name "Nom fichier" -ItemType "type"** : Commande asser complexe servent à créé toute  
                                                            sorte de chose.  
   
**New-Item -Path . -Name "Exemple" -ItemType "directory"** : Cette commande vas créé un dossier nommé Exemple  
                                                             dans le fichier au vous vous trouvez.  
  
**New-Item -Path . -Name "Exemple.txt" -ItemType "file"** : Comme la présédente a la difference près que  
                                                            celle la vas créé un fichier text.  
  
![Exemple New-Item](https://github.com/Arata34/PowerShell/blob/master/Exemple_New-Item.PNG)  
  
**Important** : Vous pouvez chnager le dossier ou sera créé le fichier en changeant le "." par le chemain de votre choix. Exemple :  New-Item -Path "D:\_Documents" -Name "Exemple.txt" -ItemType "file". 
  
**rm nom_de_l'éllément** : Cela vas suprimer l'éllément choisie (attention il n'y a pas de confirmation).  
  
**Nom_du_fichier** : Entrer le nom d'un fichier dans l'interpreteur l'ouvira si possible.
  
___________________________  
  
## Création de Script  
  
Pour créer des script Powershell je conseil d'utiliser **Powershell ISE**, l'outil est tres simple d'utilisation et est installer de base sur votre machine.

![PowerShell_ISE](https://github.com/Arata34/PowerShell/blob/master/PowerShell_ise.PNG)  
  
### Les Variables  
  
**$Nom_variable = valeur** : Cette syntaxe vas déclarer la variable et lui assigner un type.
                             Pour forcer le type de la variable vous pouvez le rajouter entre crochet avant le nom de la variable. Exemple : [string]$Exemple = "Exemple".
  
**Type de variable** : ![Variable](https://github.com/Arata34/PowerShell/blob/master/variable.PNG)  
  
**Les opérateur** : les opérateur fonctionelle sont : +, -, *, /. Exemple $result = $V_1 + $V_2.
  
________________________  
  
### Les Conditions  
  
**If (condition) {}** : La structure des condition est très simple et pertmet de verifier tout ce que l'ont   
                        souhaite.

**For (etat de base; condition; variation) {}** : Les boucle for pertmet de repeter une portion de scripte 
                                                  un nombre de fois que l'ont veux.
  
**Do {}Until(condition)** : Une boucle Do Until vas permettre de répéter un morceaux de scripte un nombre de
                            fois indéterminer.
  
## Les Opperateur de condition
  
En PowerShell les condition utilise des opperateur different qu'il faut connaitre.  
  
**-eq** : Vas verrifier l'égaliter entre deux variable ou autre. Exemple : if (5 -ep $age) {}
  
**-ne** : Comme le precedant mais vérifier une inégaliter.  

**-gt/-lt/-ge/-le** : gt est pour plus grand que, lt pour plus petit que, ge pour plus grand ou égale, le pour 
                      plus petit ou égale.

**-like** : Va permettre de comparer deux chaine de charactere. Exemple if ($value -like 'Exemple') {} 
            A noté qu'il est possible de rechercher juste une petite suite de charactere.
            Exemple : if ($value -like '*Exp\*')  
  
### Les fonction
  
Le PowerShell utilise un systeme très simple. En PowerShell utilise des prefix suivit de l'élément choisie pour interagire avec.

**Add-** : Ajoute un élément du type choisie.
  
**Get-** : Recupere un élément du type choisie.
  
**Read-** : Lis un élément du type choisie.
  
**New-** : Permet de créer un objet ou une classe.
