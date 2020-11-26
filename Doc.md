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
