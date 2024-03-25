# Steam Linux post installation

Tutoriel de post-installation de Steam sur Linux, conçu pour vous guider à travers quelques étapes clés afin d'optimiser votre expérience de jeu sur Linux.

## Langue

Changez la langue de l'interface Steam :

<p align="center">
  <img width="850" src="https://github.com/Gaming-Linux-FR/steam-post-install/blob/main/Steam%20langue.png" alt="allowflipping">
</p>

## Proton

Proton est un outil développé par Valve qui permet de jouer à des jeux vidéo conçus pour Windows sur des systèmes d'exploitation Linux. Il agit comme une couche de compatibilité.

Activez Proton pour jouer à des jeux conçus pour Windows sur votre système Linux :

<p align="center">
  <img width="850" src="https://github.com/Gaming-Linux-FR/steam-post-install/blob/main/Steam%20compatibilit%C3%A9.png" alt="allowflipping">
</p>

## Ajout de disque

Ajoutez des emplacements de stockage pour vos jeux en configurant des dossiers supplémentaires de bibliothèque de jeux :

<p align="center">
  <img width="850" src="https://github.com/Gaming-Linux-FR/steam-post-install/blob/main/Steam%20ajout%20de%20disque.png" alt="allowflipping">
</p>

Configuration de l'accès à un second disque si vous utilisez **FLATPAK** :

Si vous souhaitez ajouter un second disque dur ou SSD pour votre bibliothèque de jeux Steam, vous devez accorder à Steam l'accès à ce disque via une commande Flatpak :
              
```bash
flatpak override --user --filesystem=/chemin/vers/votre/Bibliothèque/Steam com.valvesoftware.Steam
```
   
Remplacez `/chemin/vers/votre/Bibliothèque/Steam` par le chemin réel vers votre dossier de bibliothèque Steam sur le second disque.

## Désactiver remote play

Si vous n'utiliser pas la fonctionnalité Remote Play, qui permet de streamer des jeux sur d'autres appareils, vous pouvez facilement la désactiver pour éviter que le service ne tourne en tache de fond :

<p align="center">
  <img width="850" src="https://github.com/Gaming-Linux-FR/steam-post-install/blob/main/D%C3%A9sactiver%20remote%20play.png" alt="allowflipping">
</p>
