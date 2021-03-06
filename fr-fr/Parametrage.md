# Paramétrage du plugin

Cette étape est la deuxième du processus d'installation du plugin Zigate.


Vous devez donc avoir suivi et terminé l'[étape 1 Installation du plugin](Installation.md)



## Le paramétrage

* Ouvrir __DomoticZ__ dans votre navigateur
* Aller dans le menu __Configuration__ puis __Matériel__

![Domoticz Hardware Menu for Plugin](https://raw.githubusercontent.com/pipiche38/Domoticz-Zigate-Wiki/master/Images/DzMenu.png)

*Cette page est susceptible d'avoir évoluer depuis l'écriture de cette documentation.*



| Id | Short Description    | Full Description |
| -- | -------------------- | ---------------- |
| 1  | Nom                  | Le nom donné à la Zigate. Si vous utiliser plusieurs Zigate, vous aurez besoin de plusieurs instances du matériel Zigate et le nom permettra de les identifiées.
| 2  | Type                 | `Zigate plugin` à sélectionner dans la liste déroulante |
| 3  | Zigate Model         | Choisir entre les différents modèles de Zigate (USB, DIN, PI, Wifi) |
| 4  | IP                   | IP de la Zigate pour le modèle Wifi uniquement. Laisser 0.0.0.0 pour les autres modèles |
| 5  | Port                 | Port de la Zigate pour le modèle Wifi uniquement (défaut 9999). Laisser 9999 pour les autres modèles |
| 6  | Serial Port          | Serial Port sur lequel est branché la Zigate |
| 7  | Initialize ZiGate (Erase Memory) `Erase PDM` | Pour initialiser la Zigate avec les paramètres du plugin. A __activer obligatoirement__ lors de la configuration initiale (ou après (or after an Erase EEPROMO). __ATTENTION:__ L'activation va effacer toutes des informations d'appairage de la Zigate. Will Erase all pairing information on the Zigate. Pour activer, passer à True et redémarrer le plugin |
| 8  | Port for Web Admin| Port pour accéder à l'administration web du plugin (défaut 9440). A modifier en cas d'utilisation de plusieurs instances du plugin. |
| 9  | Verbors and Debuging | Sélection du niveau du log du plugin (Aucun par défaut) |

* Coché __Activé__ pour activer le plugin
* Cliquer sur __Ajouter__

La ligne avec le plugin Zigate est normalement apparue. Cliquer dessus.

* Mettre __Initialize ZiGate (Erase Memory)__ à __False__.
* Décoché __Activé__ pour désactiver le plugin
* Cliquer sur __Modifier__ (ne pas cliquer sur Ajouter car cela dupliquera le plugin)
* Recliquer sur la ligne du plugin Zigate
* Recoché __Activé__ pour réactiver le plugin
* Cliquer sur __Modifier__ pour relancer le plugin

Vérifier les logs que le plugin Zigate s'initialise correctement.

Si tout semble fonctionner normalement, passer à l'[étape 3 Configuration du plugin](Configuration.md)

