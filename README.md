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
    <td rowspan="6"><img width="200" src="/screenshot/screenshot.png"></td>
  </tr>
  <tr>
    <td>Motherboard</td>
    <td>Asus Prime Z790M-PLUS</td>
  </tr>
  <tr>
    <td>Audio</td>
    <td>ALC887</td>
  </tr>
  <tr>
    <td>GPU</td>
    <td>Sapphire Radeon Pulse RX 6800XT 11GB</td>
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
    <td>Corsair 32G DDR5 (16G * 2) 7000Mhz CL34 (CMK32GX5M2X7000C34)</td>
  </tr>
  <tr>
    <td>Wireless &amp; Bluetooth</td>
    <td>None</td>
  </tr>
</table>

## Step 1 - Installer Windows 
1. installer Windows 10
2. 

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

### Imprimante

- Canon PIXMA MP 499
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

Google Chrome



