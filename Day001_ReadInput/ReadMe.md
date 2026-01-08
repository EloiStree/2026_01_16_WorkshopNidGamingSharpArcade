
# Allons lire des boutons d’arcade et changer la couleur de la scène Unity3D

Unity utilise un **Input Action System**.
Le game designer crée une description de ce que le joueur peut faire et du type de primitive attendue.
Le développeur n’a plus qu’à la glisser dans son script.

**Manuel** : ajouter la documentation Unity sur l’Input System.

Utilisons la librairie **Tick** que j’ai créée pour nous faciliter cela :
[https://github.com/EloiStree/OpenUPM_TickCollection](https://github.com/EloiStree/OpenUPM_TickCollection)

Et regardons comment le code de `TickMono_InputButton` fonctionne :
[https://github.com/EloiStree/OpenUPM_TickCollection/blob/main/Runtime/TickMono_InputButton.cs](https://github.com/EloiStree/OpenUPM_TickCollection/blob/main/Runtime/TickMono_InputButton.cs)

Maintenant que l’on peut déposer une Input Action et l’associer à un UnityEvent,
relions l’événement à un script qui changerait aléatoirement la couleur de la caméra.

```cs
Ajouter un code ici
```

---

# Associons un bouton à l’envoi de messages réseau avec UDP

Laissez-moi vous expliquer.

En informatique, et en réseaux plus particulièrement, on peut utiliser le fait de lier **n chiffres** à une action ou à une série d’actions.

J’ai créé une convention qui, lorsqu’elle reçoit un chiffre, se débrouille pour exécuter le code selon la plateforme :
[https://github.com/EloiStree/2024_08_29_ScratchToWarcraft](https://github.com/EloiStree/2024_08_29_ScratchToWarcraft)

J’appelle ces conventions **S2W** et **IID**, pour *Scratch To Warcraft* et *Index Integer Date*.

Dans le cadre du **IID (Index Integer Date)** :
[https://github.com/EloiStree/IID](https://github.com/EloiStree/IID)

* **Index** = l’identifiant du joueur
* **Integer** = valeur codée à utiliser pour l’action
* **Date** = information sur quand l’exécuter sur la destination

Par exemple :

* 1027 = Appuyer sur espace
* 2027 = Relâcher espace
* 4042 = Coller le caractère `*`
* 1300 = Presser le bouton A de la manette Xbox
* 2300 = Relâcher le bouton A de la manette Xbox

Pour envoyer ces nombres, nous allons utiliser un relay UDP qui visera une addresse IP
C est des numeros qui represente votre ordinateur sur le Wifi 
127.0.0.1, c est votre ordinateur
192.186.1.1 c est generalement votre routeur internet

Vision votre oridnateur personnel pour le moment.

Vous avez :
* 5 boutons d’arcade
* un board arcade DIY
* un Raspberry Pi Pico 2W

Créons un personnage sur **Hordes.io** via Firefox :
[https://hordes.io](https://hordes.io)

A la place de changer de couleur avec notre scene, contactons:  
- https://github.com/EloiStree/2020_11_29_upm_udp_thread_in_out_gate 


# N’aurait-on pas pu utiliser une interface graphique ?

Si, on aurait pu utiliser les **UnityEvent** des **Unity Button**.
Comme le bouton Unity n’a qu’un événement *Down* et pas *Up*, on doit y ajouter un petit script pour détecter le *Down* et le *Up*.

{Ajouter les détails}

Essayons de faire une petite interface de debug pour jouer à **Hordes.io** depuis notre interface 2D sous Unity3D.

Notez qu’avec une vitesse de rotation fixe, vous pouvez demander à votre personnage de tourner d’une rotation plus ou moins précise.

# C est quoi le truc vert (le Pico 2W)


Le pico est ce que lon appelle un micro controller.
Il est utiliser dans le projet de IOT et utilisant de l electronique.

Mais la puce permet aussi de simuler des claviers et des souris.

Changeons  la cible de notre relay UDP.


