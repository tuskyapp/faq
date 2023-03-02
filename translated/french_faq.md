# Foire Aux Questions sur Tusky

## Installer Tusky

### Quelle version de Tusky dois-je utiliser ?

Il existe trois versions du logiciel Tusky.

- La version "mainstream". Sauf indication contraire, il s'agit de la version que vous souhaitez
- Version "Beta". Cette version est prévue pour les testeurs avant chaque version "mainstream"
- Version "Test". Cette version est publiée à chaque modification de Tusky

### Où puis-je trouver Tusky ?

Vous pouvez installer Tusky depuis Google Play ou via F-Droid.

Pour celà :

- Installer [Tusky depuis Google Play](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky)
- Installer [Tusky depuis F-Droid](https://f-droid.org/packages/com.keylesspalace.tusky/)

La version Beta est uniquement disponible sur Google Play. Vous devez vous inscrire au programme Beta.

- S'inscrire à [Tusky Beta sur Google Play](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky)

Les versions de Test sont disponibles sur Google Play et sur F-Droid :

- Installer [Tusky Nightly sur Google Play](https://play.google.com/store/apps/details?id=com.keylesspalace.tusky.test)
- Dans les paramètres F-Droid, sélectionnez "My Apps > Repositories", puis ajoutez un nouveau répertoire avec le lien `https://releases.nailyk.fr/repo/`

### Pourquoi la version de Tusky sur F-Droid n'est pas à jour ?

F-Droid compile Tusky depuis le code source à chaque fois qu'une nouvelle version est disponible. Celà peut prendre plus de temps que pour les nouvelles versions disponibles sur Google Play.

## Gérer mon compte

### Puis-je créer un compte avec Tusky ?

Pas encore, vous devez d'abord créer un compte via un service comme [joinmastodon.org](https://joinmastodon.org/).

Une fois fait, vous pourrez alors vous connecter à ce compte sur Tusky.

### Puis-je supprimer mon compte avec Tusky ?

Vous pouvez vous déconnecter de votre compte avec Tusky. Cependant vous devrez suivre les procédures propres à votre instance pour complètement supprimer votre compte.

### J'essaye de me connecter à mon compte mais je me fais Rick-Rolled. Pourquoi ?

Tusky ne supporte pas l'utilisation de comptes depuis certains [serveurs](https://github.com/tuskyapp/Tusky/blob/develop/app/src/main/res/values/donottranslate.xml#L160) à cause de leur association avec des groupes haineux.

> L'absence d'un serveur de cette list n'implique *pas* une approbation des développeurs de Tusky.

Si celà vous offense, vous restez libre d'utiliser un client Mastodon différent.

## Timelines (fils)

### Pourquoi le compteur de "likes" et de "boosts" différent du client web ?

Ce comportement est lié au fonctionnement de Mastodon. Les likes et les boosts ne sont pas fédérés parfaitement; si les autres et vous êtes sur des serveurs différents il se peut que vous voyez des nombres différents entre Tusky et le site web.

### Comment voir les fils fédérés ?

Depuis votre fil d'accueil :

- Ouvrez les "préférences de compte" (glissez depuis le bord gauche de l'écran ou appuyez sur votre image de profil pour voir l'option)
- Appuyez sur "onglets"
- Appuyez sur le bouton "+" (en bas à droite)
- Choisir "Global" sur ce menu

Vous pouvez ajuster l'ordre des onglets depuis cet écran aussi.

### Comment cacher les republications de postes de mon fil ?

- Ouvrez les "préférences" (glissez depuis le bord gauche de l'écran ou appuyez sur votre image de profil pour voir l'option)
- Appuyez sur la section "Filtres > Onglets"
- Déselectionnez l'option "Afficher les partages"

### Comment cacher les réponses de postes de mon fil ?

- Ouvrez les "préférences" (glissez depuis le bord gauche de l'écran ou appuyez sur votre image de profil pour voir l'option)
- Appuyez sur la section "Filtres > Onglets"
- Déselectionnez l'option "Afficher les réponses"

### Comment puis-je suivre un hashtag ?

- Appuyez sur le hastage dans un poste pour voir l'ensemble des postes avec ce hashtag
- Appuyez sur l'icone "suivre" en haut à droite

### Comment puis-je masquer un hashtag ?

> Cette fonctionnalité est disponible à partir de Tusky 21 (Tusky Nightly inclu). Pour vérifier la version de Tusky que vous utilisez, vous pouvez ouvrir le menu "À propos".

- Appuyez sur le hashtag dans un poste pour voir l'ensemble des postes avec ce hashtag
- Appuyez sur l'icone "masquer" en haut à droite

## Publier

### Comment modifier un poste ?

> Cette fonctionnalité est disponible à partir de Tusky 21 (Tusky Nightly inclu). Pour vérifier la version de Tusky que vous utilisez, vous pouvez ouvrir le menu "À propos".

- Appuyez sur le menu "..." en bas à droite du poste
- Choisissez "Éditer"
- Appuyez sur l'icone "Pouet !" pour publier le poste modifié (qui remplacera alors l'original)

### Comment envoyer un message direct ?

> Important : les messages directs sur Mastodon ne sont pas encryptés et peuvent être lus par les administrateurs de l'instance. Soyez prudents en partageant des informations privées sur Mastodon.

- Créez un nouveau poste
- @-mentionnez l'utilisateur souhaité
- Appuyez sur l'icône "Visibilité" (par défaut elle ressemble à un globe)
- Sélectionnez la visibilité "Direct"

## Notifications

### Pourquoi les notifications sont moins fréquentes sur Tusky ?

Par défaut, Tusky vérifie les nouvelles notifications toutes les 15 minutes environ.

Tusky peut également utiliser [UnifiedPush](https://unifiedpush.org/) pour montrer les notifications en temps réel. Pour celà :

- Installez "ntfy" (depuis le [Google Play](https://play.google.com/store/apps/details?id=io.heckel.ntfy) ou [F-Droid](https://f-droid.org/packages/io.heckel.ntfy))

### Pourquoi Tusky utilise UnifiedPush au lieu des services Google pour les notifications ?

Google Services ne fonctionne pas sur tous les appareils et nous souhaitons donner aux utilisateurs la liberté de choisir leur fournisseur de notifications push.

## Filtres

### Mes filtres sont-ils importés depuis mon instance ?

Oui. Les filtres sont syncronisés dans les deux sens entre Tusky et votre instance.

## Rapporter les bugs et demander de nouvelles fonctionnalités

### Comment puis-je rapporter un bug ?

Si vous pensez avoir identifié un bug dans Tusky, la manière idéale de le rapporter est la suivante :

> Un compte Github est obligatoire pour celà.

1. Vérifiez que personne d'autre n'a signalé ce bug
    1. Ouvrez la [liste des issues ouvertes](https://github.com/tuskyapp/Tusky/issues)
    1. Cherchez dans la liste des issues
    1. Si vous trouvez un signalement de bug existant vous pouvez laisser un commentaire (si vous avez plus d'informations à signaler), ou appuyer sur le bouton "subscribe" pour être notifié des nouveaux commentaires sur ce rapport ou lors de la fermeture de celui-ci.
1. Si il n'y a pas de rapport correspondant, appuyez sur "New issue" pour rapporter un nouveau bug.
    1. Vous serez automatiquement notifié des nouveaux commentaires ou de la fermeture de ce rapport.

La méthode la moins idéale est de publier au sujet de ce bug sur Mastodon en mentionnant le compte officiel de Tusky (`@Tusky@mastodon.social`), ou d'utiliser le hashtag `#Tusky` en croisant les doigts pour quelqu'un le voit.

### Comment demander une nouvelle fonctionnalité ?

Si il y a une fonctionnalité que vous souhaiteriez voir ajoutée à Tusky, la manière idéale de le signaler est la suivante :

> Un compte Github est obligatoire pour celà.

1. Vérifiez que personne d'autre n'a demandé une fonctionnalité similaire
    1. Ouvrez la [liste des issues ouvertes](https://github.com/tuskyapp/Tusky/issues)
    1. Cherchez dans la liste des issues
    1. Si vous trouvez une demande de fonctionnalité existante vous pouvez laisser un commentaire (si vous avez plus d'informations à signaler), ou appuyer sur le bouton "subscribe" pour être notifié des nouveaux commentaires sur ce rapport ou lors de la fermeture de celui-ci.
1. Si il n'y a pas de rapport correspondant, appuyez sur "New issue" pour suggérer une fonctionnalité.
    1. Vous serez automatiquement notifié des nouveaux commentaires ou de la fermeture de ce rapport.

La méthode la moins idéale est de publier au sujet de ce bug sur Mastodon en mentionnant le compte officiel de Tusky (`@Tusky@mastodon.social`), ou d'utiliser le hashtag `#Tusky` en croisant les doigts pour quelqu'un le voit.

## Contribuer à Tusky

### Je veux aider, que puis-je faire ?

Il existe de nombreuses façons d'aider le développement de Tusky.

- Rapporter des bugs et suggérer de nouvelles fonctionnalités
- Apporter des traductions
- Contribuer au code ou à la documentation
- Faire un don

Des rapports de bug et des suggestions de fonctionnalités biens rédigés aident à rendre Tusky meilleur pour tous. Les précédentes sections expliquent comment rapporter un bug ou suggérer une fonctionnalité.

Si vous souhaitez voir Tusky traduit dans une langue que vous parlez, ou que vous appercevez une erreur dans l'une des traductions existantes, vous pouvez contribuer en envoyant une correction. Nous utilisons Weblate pour gérer les traductions; vous pouvez vous inscrire sur [l'instance Weblate de Tusky](https://weblate.tusky.app/) pour soumettre une nouvelle traduction ou améliorer une traduction existante.

Si vous êtes familiers avec le développement Android, vous pouvez également envoyer des modifications de code via Github. Une bonne manière de commencer est de rechercher la liste des issues pour trouver un bug ou une suggestion de fonctionnalité importante pour vous et commencer à discuter la manière dont vous souhaitez résoudre le problème. Après en avoir discuté vous pourrez rédiger le code et soumettre une PR avec le changement.

Les donations financières sont toujours les bienvenues et peuvent être effectuées à travers le [Tusky open collective project](https://opencollective.com/tusky). Vous pourrez vous y inscrire et effectuer une donation ponctuelle ou récurente au projet.

## Comment puis-je contacter les développeurs ?

Dans le salon Matrix [#Tusky](https://matrix.to/#/#Tusky:matrix.org).
