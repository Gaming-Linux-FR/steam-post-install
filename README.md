# Steam Linux post installation

Tutoriel de post-installation de Steam sur Linux, conçu pour vous guider à travers quelques étapes clés afin d'optimiser votre expérience de jeu sur Linux.

<br>

# Table des Matières

1. [Changer la Langue](#changer-la-langue)
2. [Proton](#proton)
3. [Ajout de Disque](#ajout-de-disque)
4. [Steam Input](#steam-input)
5. [Désactiver Remote Play](#désactiver-remote-play)
6. [Trouver le chemin d'installation de vos jeux](#trouver-le-chemin-dinstallation-de-vos-jeux)
7. [Astuce pour améliorer la vitesse de téléchargement](#user-content-astuce-pour-améliorer-la-vitesse-de-téléchargement)

<br>

## Changer la Langue

Changez la langue de l'interface Steam :

<p align="center">
  <img width="850" src="https://codeberg.org/Gaming-Linux-FR/steam-post-install/raw/branch/main/Steam%20langue.png" alt="langue">
</p>

<br>

## Proton

Proton est un outil développé par Valve qui permet de jouer à des jeux vidéo conçus pour Windows sur des systèmes d'exploitation Linux. Il agit comme une couche de compatibilité.

Activez Proton pour jouer à des jeux conçus pour Windows sur votre système Linux :

<p align="center">
  <img width="850" src="https://codeberg.org/Gaming-Linux-FR/steam-post-install/raw/branch/main/Steam%20compatibilit%C3%A9.png" alt="compatibilité">
</p>

<br>

## Ajout de disque

Ajoutez des emplacements de stockage pour vos jeux en configurant des dossiers supplémentaires de bibliothèque de jeux :

<p align="center">
  <img width="850" src="https://codeberg.org/Gaming-Linux-FR/steam-post-install/raw/branch/main/Steam%20ajout%20de%20disque.png" alt="ajout-disque">
</p>

Si Steam **flatpak** : [Ajout disques secondaires Steam Flatpak](https://codeberg.org/Gaming-Linux-FR/glf-astuces#acc%C3%A8der-%C3%A0-un-disque-secondaire-avec-une-application-flatpak)

<br>

## Steam input

Steam input peut grandement améliorer le support de votre manette sur Linux.

<p align="center">
  <img width="850" src="https://codeberg.org/Gaming-Linux-FR/steam-post-install/raw/branch/main/steam%20input.png" alt="manettes">
</p>

<br>

## Désactiver remote play

Si vous n'utilisez pas la fonctionnalité Remote Play, qui permet de streamer des jeux sur d'autres appareils, vous pouvez facilement la désactiver pour éviter que le service ne tourne en tache de fond :

<p align="center">
  <img width="850" src="https://codeberg.org/Gaming-Linux-FR/steam-post-install/raw/branch/main/D%C3%A9sactiver%20remote%20play.png" alt="désactiver-remote-play">
</p>

## Trouver le chemin d'installation de vos jeux

Si par exemple vous voulez moder vos jeux, sur Linux les chemins d'installation de vos jeux ne sont pas les mêmes que sur Windows, mais pas de tracas, plutôt que de chercher faites clic droit sur le jeu, propriété et dans l'onglet `Fichiers Installés` vous pourrez cliquer sur `parcourir` et vous vous retrouvez directement dans le dossier d'installation du jeu.

<p align="center">
  <img width="850" src="https://codeberg.org/Gaming-Linux-FR/steam-post-install/raw/branch/main/steam-fichiers.png" alt="steam-fichiers">
</p>

## Astuce pour améliorer la vitesse de téléchargement

Si vous constatez que vos téléchargements sur Steam sont plus longs que ce que vous pouvez voir ailleurs, alors vous pouvez tenter de désactiver le HTTP2.

Pour cela, copiez collez les linges suivantes dans un terminal : 

Steam natif :

```
echo "@nClientDownloadEnableHTTP2PlatformLinux 0" >> ~/.steam/steam/steam_dev.cfg
echo "@fDownloadRateImprovementToAddAnotherConnection 1.0" >> ~/.steam/steam/steam_dev.cfg
```

Steam Flatpak :

```
echo "@nClientDownloadEnableHTTP2PlatformLinux 0" >> ~/.var/app/com.valvesoftware.Steam/.steam/steam/steam_dev.cfg
echo "@fDownloadRateImprovementToAddAnotherConnection 1.0" >> ~/.var/app/com.valvesoftware.Steam/.steam/steam/steam_dev.cfg
```

