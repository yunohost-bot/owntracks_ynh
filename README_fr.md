# OwnTracks pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/owntracks.svg)](https://dash.yunohost.org/appci/app/owntracks) ![](https://ci-apps.yunohost.org/ci/badges/owntracks.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/owntracks.maintain.svg)  
[![Installer OwnTracks avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=owntracks)

*[Read this readme in english.](./README.md)*
*[Lire ce readme en français.](./README_fr.md)*

> *Ce package vous permet d'installer OwnTracks rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

Gérez votre historique de géolocalisation

**Version incluse :** 0.1~ynh10



## Captures d'écran

![](./doc/screenshots/screenshot.png)

## Avertissements / informations importantes

## Caractéristiques

- [Fonctionnalités d'OwnTracks pour une API HTTP](http://owntracks.org/booklet/tech/http/), limité aux [fonctionnalités implémentées par l'enregistreur PHP](https://github.com/tomyvi/php-owntracks-recorder#features). Notamment, pas de fonction Amis. L'[enregistreur PHP en amont a été modifié](https://github.com/tituspijean/php-owntracks-recorder) pour supprimer une dépendance PHP encombrante.
- Multi-utilisateur : chaque utilisateur YunoHost peut se connecter via l'authentification HTTP de base, et n'a accès qu'à ses données.

## Installation

- Installez l'application sur votre serveur YunoHost
- Installez l'application mobile sur votre appareil, consultez le [site Web d'OwnTracks](http://owntracks.org)
- Configurez votre application mobile :
  - Autorisez-le à accéder à votre emplacement
  - Préférence > Connexion
    - Mode : `http privé`
    - Hébergeur : `https://DOMAIN/PATH/record.php`
    - Identification
       - Authentification: `enabled`
       - Nom d'utilisateur/mot de passe : vos identifiants YNH
       - ID de l'appareil : comme vous le souhaitez
   - Reportez-vous à la [documentation d'OwnTracks](http://owntracks.org/booklet) pour les autres paramètres

## Documentations et ressources

* Site officiel de l'app : https://owntracks.org/
* Dépôt de code officiel de l'app : https://github.com/tomyvi/php-owntracks-recorder
* Documentation YunoHost pour cette app : https://yunohost.org/app_owntracks
* Signaler un bug : https://github.com/YunoHost-Apps/owntracks_ynh/issues

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/owntracks_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/owntracks_ynh/tree/testing --debug
ou
sudo yunohost app upgrade owntracks -u https://github.com/YunoHost-Apps/owntracks_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** https://yunohost.org/packaging_apps