```diff
- ATTENTION ! Cette emulateur a été modifié grandement, aucune aide ne sera apporté si vous souhaitez le modifier !
```

## AegnorServeur — Login 1.43.7

Cette émulateur est open source pour tous le monde.  
Merci de pas le vendre, vous avez reçu gratuitement, donnez gratuitement 🤗.

Ce login est désormais **porté pour le client Dofus Retro 1.43.7** (à l'origine 1.34.1).<br>
Il est lié au GitHub game suivant :<br>
👉 [server-1.43.7](https://github.com/jguyet/server-1.43.7) (fork du game Aegnor / Locos)

Ce login est un fork du travail original d'Arwase, lui-même un fork de Locos.

## 🆕 Compatibilité client 1.43.7

Le portage vers le client Dofus Retro 1.43.7 inclut :

- **Transport / handshake** : version client 1.43.7, réponse policy file Flash, parser format `ù` 3-parts (`base64ù<chksum>ù<commande>`), bypass du déchiffrement (encryptPacket désactivé).
- **Character switch** : flow ticket complet via Exchange `WS<accId>;<ticket>#`, intercept du `#S\n<ticket>` côté login, nouveau status `WAIT_SWITCH_TICKET`, envoi Ad/Ac/AH/AlK/AQ.
- **ServerSelected** : encodage UTF-8 (au lieu de ISO-8859-1).
- **Config** : nouveau paramètre `system.server.login.ip` distinct de `system.server.exchange.ip`, permet de bind explicitement le login server sur une IP précise (sinon 0.0.0.0).

## Informations :

Aegnor est un serveur de type EasyLike.
Il propose une experience de jeu legérement modifié afin d'accélerer la progression dans le jeu et ajoute des fonctionnalités non présente initialement comme un système de rareté d'objet etc.
Pour plus d'informations vous pouvez visiter l'ancien discord du serveur qui regorge d'informations à son sujet.
Cette émulateur est basé sur une base d'un émulateur starloco et diverses sources d'emulateurs afin d'en extraire le meilleur.
[@aegnor] https://discord.com/invite/f2cNEZ2cev

## DEBUG :

La liste des debugs est visible sur le discord dans l'onglet patchnote

## REMERCIEMENT :

Je remercie Hydronish de son aide lors du développement du serveur et l'ensemble des donateurs qui m'ont aidé durant le developpement du serveur.  
Je remercie également Locos pour la base de son travail et tous les auteurs qui ont succèdés ou précédés ses modifications pour son émulateur.

👤 Portage client **1.43.7** : **Jiji** ([@jguyet](https://github.com/jguyet))  
👤 Auteur original : Arwase
