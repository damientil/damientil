## APT

### Rechercher les mises à jour disponibles
Télécharge les informations des paquets à partir des sources configurées
Se base sur les sources définies dans /etc/apt/source.list
```
apt update
```
Meme comportement pour `apt-get update`
### Installer les mises à jour identifiée
Mets à jour les paquets installés sans en supprimer. Quelques différences de comportement :
`apt-get upgrade` : N'installe pas de nouveaux paquets
`apt upgrade` : Installe de nouveau paquets pour satisfaire des dépendances si nécessaire
```
apt upgrade
```
### Voir la liste des paquets aynt des résidus de configuration
```
sudo apt list ~c
```
### Purger tous les résidus de configuration.
```
sudo apt purge ~c
```
