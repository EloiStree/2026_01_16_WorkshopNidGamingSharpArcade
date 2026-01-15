Bonjour à vous et bienvenue.

Êtes-vous prêts à souffrir 😁.

Devenir développeur de jeux vidéo est magique 🪄
Mais en échange, vous devrez vendre votre âme à l’entropie : <img width="1456" height="610" alt="image" src="https://github.com/user-attachments/assets/db6471da-eee6-470c-9326-25874cb82f56" />

Ma méthode pour enseigner la programmation repose sur le fait de jouer à des jeux vidéo.

Pour cela, j’ai créé deux conventions : **IID** et **S2W**.

* [IID](https://github.com/EloiStree/IID) : index du joueur avec une valeur entière (int) pour une action et la date d’exécution.
* [S2W](https://github.com/EloiStree/2024_08_29_ScratchToWarcraft) : envoyez-moi un entier, je le transforme en code pour simuler des touches.

Il nous faudra un code pour simuler ces touches de clavier :
* [S2W](https://github.com/EloiStree/2024_08_29_ScratchToWarcraft) en Python si on veut faire du software.
  * [XOMI](https://github.com/EloiStree/2022_01_24_XOMI) si vous voulez simuler des manettes avec du software.
* Le [Pico 2W](https://github.com/EloiStree/APIntCodeTournamentHardwarePico2W/tree/main/Pico2W) permet de simuler un clavier, une souris et du MIDI avec du hardware.
  * Vous pouvez trouver une version [ESP32](https://github.com/EloiStree/APIntCodeTournamentHardwareESP32S3/blob/main/WifiToXInputBLE/Wifi_S2W_To_XInput/Wifi_S2W_To_XInput.ino) si vous voulez simuler une manette.

Pour communiquer entre Unity3D et ce code Python, il nous faut du réseau Wi-Fi.
Nous allons utiliser ce que l’on appelle de l’UDP :
[https://github.com/EloiStree/2020_11_29_upm_udp_thread_in_out_gate](https://github.com/EloiStree/2020_11_29_upm_udp_thread_in_out_gate)

Que va-t-on faire :

* Jouer avec les pieds dans Unity grâce à des bornes d’arcade.
* Créer des UnityEvent pour envoyer des entiers dans le but d’avancer.
* Faire une petite boîte à outils pour bouger dans [hordes.io](https://hordes.io).
* Installer S2W pour recevoir nos entiers.
* Pour le faire bouger, il faudra envoyer les messages hors de Unity3D avec de l’UDP.
* Maintenant que l’on sait faire avancer notre personnage :
* On peut le faire bouger, sauter, tirer, se soigner…
* Apprenons le C# et les classes tout en montant de niveau.

Note: S2W ne fonction que avec Firefox pour 
- https://hordes.io
- https://www.firefox.com/

Deuxième exercice : on va apprendre à découper du texte pour faire notre propre langage de programmation 😋.
Nous allons créer un interpréteur.

Pour devenir développeur Unity3D ou Godot version C#, il vous faudra apprendre de nombreux concepts.
Je les ai majoritairement listés ici.

Durant votre apprentissage, je vous invite à les barrer un à un :

* barrer les mots que vous connaissez ;
* double barrer les mots que vous maîtrisez ;
* triple barrer si vous pensez être incollable sur le sujet.


----

### Video

- Long first version of the workshop, part 1: https://youtu.be/n4CXsb6nQG4
  
---

### À voir :

* **La dactylographie**

  * Tous les caractères d’un clavier QWERTY en C#

* **Les bases**

  * C’est quoi :

    * une variable ;
    * une valeur primitive ;
    * une méthode ;
    * un string ;
    * un if, else, while, switch, for ?

* **Les bases avancées**

  * une classe ;
  * une liste et un tableau ;
  * un dictionnaire.



---------

Move in World of Warcraft, C# and Math:   
[<img width="1919" height="1196" alt="image" src="https://github.com/user-attachments/assets/e995b3d9-0cec-4454-be1f-eddfb2f26831" />](https://www.youtube.com/watch?v=QKGy2C7bsUI)    
 



**Note**: Hordes.io n’a pas de version Xbox.  
Donc, pour l’exercice, vous pourriez proposer une façon de jouer au jeu avec une manette.  
Bon, petit problème avec ça : il vous faut du clavier et une simulation de souris.  
Exemple : https://youtu.be/KfbV69KvssA?t=692  
Pour sélectionner les objets sur le sol, je spam-clique le milieu de l’écran avec la souris ;)  
Du temps de JOMI  
