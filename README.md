# Hackintosh
Ma configuration pour mon Hackintosh en Dual Boot avec Sonoma 14.3.1 / Windows 11

<table>
<tr>
  <th>Type</th>
  <th>Name</th>
  <th></th>
</tr>
  <tr>
    <td>CPU</td>
    <td>Intel Core I7 14700KF</td>
    <td rowspan="8"><img src="https://github.com/percolouco/Hackintosh/assets/57752243/fc7842bc-4bbb-4bca-a335-65eebf48e5eb"></td>
  </tr>
  <tr>
    <td>Motherboard</td>
    <td>Asus Prime Z790M-PLUS</td>
  </tr>
  <tr>
    <td>Chipset Audio</td>
    <td>Realtek ALC897</td>
  </tr>
  <tr>
    <td>Chipset LAN</td>
    <td>Intel I219-V</td>
  </tr>
  <tr>
    <td>GPU</td>
    <td>Sapphire Radeon Pulse RX 6800XT 16Go</td>
  </tr>
  <tr>
    <td>SSD</td>
    <td>
      Crucial P3 Plus 2To
      <br>
      PNY XLR8 CS3030 1To
    </td>
  </tr>
  <tr>
    <td>RAM</td>
    <td>Corsair 32Go DDR5 (2 * 16Go) 7000Mhz CL34 (CMK32GX5M2X7000C34)</td>
  </tr>
  <tr>
    <td>Wireless &amp; Bluetooth</td>
    <td>None</td>
  </tr>
</table>

## Step 1 - Installer Windows 

> [!WARNING]
> Faire l'image avec balenaEtcher va faire bugguer l'installation de Windows 10

1. Créer l'image ISO Windows 10 avec Rufus
2. Installer Windows 10
3. Mettre la clé CD pour activer windows 10
4. Faire les MAJ Windows update et redémarrer le PC autant que nécessaire
> [!WARNING]
>  Lancer l'application pour la mise à niveau vers Windows 11 en administrateur
5. aller sur [https://www.microsoft.com/fr-fr/software-download/windows11](https://www.microsoft.com/fr-fr/software-download/windows11) pour télécharger ce qu'il faut pour mettre à niveau windows 10 vers Windows 11



Windows est prêt à fonctionner.

## Step 2 - Installer macOS
### Step 2.1 - Créer la clé bootable

Créer une clé bootable avec l'image `Olarila Sonoma 14.3.1.raw` avec [balena Ecther](https://etcher.balena.io/)

### Step 2.2 - Créer le dossier EFI

à remplir

### Step 2.3 - Transférer le dossier EFI dans la clé bootable

Pour ouvrir la partition EFI de la clé de boot : 
1. Lancer l'invit de commande
2. Taper `Diskpart`
3. Taper `list disk`
4. Taper `select disk X` X étant le disque à selectionner
5. Taper `list partition X` X étant la partition à selectionner
6. Taper `assign letter=X` X étant la lettre du lecteur que l'on souhaite lui attribuer

## Step 3 - Application à installer sur macOS

[Aggrégateur d'installation comme Ninite](https://macapps.link/en/)

## Step 4 - Drivers pour Windows

### Drivers de la CM

> [!WARNING]
> Penser à update le BIOS

[Asus Prime Z790M-PLUS ](https://www.asus.com/motherboards-components/motherboards/prime/prime-z790m-plus/)

### Carte graphique

Sapphire PULSE AMD Radeon™ RX 6800 XT 

[AMD Software: Adrenalin Edition](https://www.amd.com/en/support)

### Imprimante

> [!WARNING]
> Prendre les drivers pour Windows 10
- [Canon PIXMA MP 499](https://www.canon-europe.com/support/consumer/products/printers/pixma/mp-series/pixma-mp499.html?type=drivers&detailId=tcm:13-988844&os=Windows%2010%20(64-bit)&language=fr&productTcmUri=tcm:13-780631)

> [Canon MP Navigator EX 4.0](https://www.canon.fr/support/consumer_products/software/mp-navigator-ex.html)
> 
> [Canon IJ Network Tool](https://www.canon.fr/support/consumer_products/software/ij-network-tool.html)

## Step 5 - Application à installer sur Windows

[Ninite](https://ninite.com/7zip-chrome-discord-filezilla-firefox-greenshot-notepadplusplus-putty-steam-thunderbird-vlc-vscode-zoom/)

> Firefox
>
> Google Chrome
>
> 7-zip
>
> Zoom
>
> Discord
>
> Thunderbird
>
> VLC
>
> Greenshot
>
> Notepad++
>
> [!NOTE]
> transférer le dossier ici une fois installé %appdata%\notepad++
> 
> Filezilla
> 
> Putty
> 
> Steam
> 
> Visual Studio Code


Liste des plugins à rajouter à Visuel Studio Code

Alpine.js IntelliSense
Auto Close Tag
C/C++
Compare Folders
ESLint
Liquid
PlatformIO IDE
Pomodoro Timer
Prettier - Code formatter
Pylance
Python
Python debugger
Shopify Liquid
Tailwind CSS IntelliSense
Todo Tree
Turbo Console log

[Ultimaker Cura](https://ultimaker.com/software/ultimaker-cura/#downloads)  

[Fusion 360](https://www.autodesk.com/products/fusion-360/overview)

[DS4Windows](https://ds4-windows.com/download/ryochan7-ds4windows/)

[Binance]

[Github Desktop](https://desktop.github.com/)

[Slack](https://slack.com/intl/fr-fr/downloads/windows)

[WhatsApp](https://www.whatsapp.com/download)

[Microsoft Teams](https://www.microsoft.com/en-us/microsoft-teams/download-app)

Photoshop

## Step 6 - Feature à update

Modification du menu contextuel pour retrouver celui d'avant 

![image](https://github.com/percolouco/Hackintosh/assets/57752243/e0f49d8e-997a-4f56-8a9c-61872062d50e)

1. Lancer le terminal de commande en Administrateur
2. taper dans le cmd `reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f `
3. redémarrer








