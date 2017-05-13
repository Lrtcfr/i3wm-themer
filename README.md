<h1>i3wm-themer</h1>
<ul>
  Ma collection de thèmes pour i3wm.

  ![](https://github.com/unix121/i3wm-themer/blob/master/workflow/workflow1.gif?raw=true)
</ul>

<h1>Prérequis :</h1>
<ul>
  <li> i3-wm (peut être i3-gaps pour certaines sections) sur votre distribution GNU/Linux préférée.</li>
  <li> <a href="https://github.com/jaagr/polybar">Polybar</a> (pour la pluparts des thèmes)</li>
  <li> <a href="https://davedavenport.github.io/rofi/">Rofi</a> (pour la pluparts des thèmes)</li>
  <li> <a href="https://wiki.archlinux.org/index.php/nitrogen">Nitrogen</a> (Pour le fond d'écran, peut aussi être fait manuellement)</li>
  <li> Les thèmes de Firefox peuvent être installés en utilisant l'extension Firefox "Stylish"</li>
  <li> La pluparts des thèmes et icônes GTK ont été créés en utilisant <a href="https://github.com/actionless/oomox">oomox</a></li>
</ul>

<ul>
  Tous les changments nécéssaire de vos fichiers de configuration peuvent être trouvés dans le répertoire /emplated_themes/{THEME}/
  Copiez ce que vous voulez de n'importe quelle configuration dans le répertoire /themes/{THEME}/ Vous pouvez trouver mes fichiers de     configuration, mais je ne recommande pas pas de les copier directement, car ils contiennent mes propres raccourcis clavier et des       paramètres spécifique. Mais à la place, vous pouvez utiliser le script d'installation pour appliquer les différentes parties de ma
  configuration à la votre.
</ul>

<h3>Prérequis basique (pour le script)</h3>
<ul>
Ce script est encore en cours de développement, vous devez donc mettre votre configuration au bon endroit.
<li> Les fichiers de configuration i3 doivent être placés dans le répertoire :

      ~/.i3/config ou ~/.config/i3/config  

</li><li>Les fichiers de configuration de Polybar doivent être placés dans le répertoire :

      ~/.config/polybar/config

</li><li>Les fichiers de configuration de Compton doivent être placés dans le répertoire :

      ~/.config/compton.conf

</li><li>.Xresources doit être placé dans le répertoire :

      ~/.Xresources ou ~/.extend.Xresources

</li><li>Les fichiers de configuration de Dmenu doivent être placés dans le répertoire :

      ~/.dmenurc
</li>
<li>Vous devrez peut être effectuer quelques changements vous-même, après l'exécution du script, car il est encore en développement peut parfois avoir des comportements non désirés.
</li>
<li>Pour les problèmes communs, regardez la section issues du dépot.</li>
</ul>

<h1>Utilisation du script</h1>
<ul>
Le script réécrira seulement les parties de votre configuration utilisés par le thème. Pour appliquer un thème, veuillez effectuer les commandes suivantes :
</ul>
<ul>

  <li> git clone https://github.com/unix121/i3wm-themer</li>
  <li> cd i3wm-themer/scripts/</li>
  <li> Premièrement, sauvegarder votre configuration actuelle, au cas vous vous voudriez y revenir :
  
      ./i3wmthemer -b {BACKUP_NAME}

La sauvegarde est enregistrée dans le repertoire i3wmthemer/backups/ Le répertoire de sauvegarde contiendra les fichiers de configuration mentionnés dans la section [Prérequis basique]. Si quelque chose se passe mal, vous pouvez les copier-coller à leurs place originale, afin de retrouver votre configuration précédente.
  </li>

  <li> Now run the script in configuration mode to apply some of the basic changes for the theme:

      ./i3wmthemer -c

  This will add the lines that are in /templates/ directory to your i3 and polybar configuration files.

  DO NOT GO FURTHER IF THOSE CHANGES ARE NOT APPLIED CORRECTLY

  After that step you should have something like <a href="https://github.com/unix121/i3wm-themer/blob/master/templates/.i3/config">
  this</a> added to your i3 configuration file and something like <a href="https://github.com/unix121/i3wm-themer/blob/master/templates/.config/polybar/config">this</a> added under [colors] tag in
  your polybar configuration file.

  If those changes are not applied then you might have to copy them manually.

  Run this script only the first time you use this script just to setup your files.
  You don't need to run it every time you want to apply a theme, only the first time.
  </li>
  <li> Now apply the theme you want:

    ./i3wmthemer -t {THEME}

{THEME} should be the name of the theme you want to apply.

Example on how to apply the "Forest" theme:

    ./i3wmthemer -t Forest
 </li>
 <li> If you want to go back to a backup you can run the script like that:

    ./i3wmthemer -t ../backups/{BACKUP_NAME}

{BACKUP_NAME} should be the same as the one given in the backup step above.
  </li>
 <li> After you run the script you might have to manually set the wallpaper
which is located in the {THEME} directory and also use your
appearance manager to apply the Icons and the GTK Themes.</li>
  <li> NOTE: If you notice any bugs on the script feel free to contact me and I will address them</li>
</ul>

<ul>
<h3>Disclaimer</h3>
The ways mentioned above overwrite some parts of your files, use them with caution. I am not responsible if anything happens to your computer. Normally if you follow the instructions step by step everything should be just fine, but unexpected things sometimes happen. The author is not responsible for any damage done.
Also the script is still under development so any feedback/help would be much appreciated.
</ul>

</ul>

<h1>Themes</h1>

<ul>
  <li><h2>Clouds</h2>
    <img src="http://i.imgur.com/QAORpDM.png">
  <li><h2>Sky</h2>
    <img src="http://i.imgur.com/mFbVgTf.png">
    <a href="http://imgur.com/a/p2ziB">(More can be found here)</a></li>
  <li><h2>Forest</h2>
    <img src="http://i.imgur.com/1WafFRk.png">
    <a href="http://imgur.com/a/SuKKf">(More can be found here)</a></li>
  <li><h2>Water</h2>
    <img src="http://i.imgur.com/z3rliuz.png">
    <a href="http://imgur.com/a/PVCKq">(More can be found here)</a></li>
  <li><h2>Fire</h2>
    <img src="http://i.imgur.com/8U5DmFY.png">
    <a href="http://imgur.com/a/pYqEl">(More can be found here)</a></li>
  <li><h2>Ice</h2>
    <img src="http://i.imgur.com/3a1J77j.png">
    <a href="http://imgur.com/a/0FMYq">(More can be found here)</a></li>
  <li><h2>Space</h2>
    <img src="https://i.imgur.com/eLkyvc0.png">
    <a href="http://imgur.com/a/0hmbl">(More can be found here)</a></li>
  <li><h2>Nature</h2>
    <img src="http://i.imgur.com/1B7IA96.png">
    <a href="http://imgur.com/a/PuXie">(More can be found here)</a></li>
  <li><h2>Subway</h2>
    <img src="http://i.imgur.com/M5ZH9Dh.png">
    <a href="http://imgur.com/a/1aO8E">(More can be found here)</a></li>
  <li><h2>Colors</h2>
    <img src="http://i.imgur.com/ZUEzkiT.png">
    <a href="http://imgur.com/a/ub0Jl">(More can be found here)</a></li>
  <li><h2>Minimal</h2>
    <img src="http://i.imgur.com/aaosiZ2.png">
    <a href="http://imgur.com/gallery/bZHDF">(More can be found here)</a></li>
  <li><h2>Grayscale</h2>
    <img src="http://i.imgur.com/K0uT5ua.png">
    <a href="http://imgur.com/gallery/1TYFd">(More can be found here)</a></li>
  <li><h2>Sea</h2>(Cannot be set via the script yet)
    <img src="http://i.imgur.com/yapFCCe.png">
    <a href="http://imgur.com/a/3BsTW">(More can be found here)</a></li>
</ul>

<ul>

<h3>Note</h3>

If you are the original artist of any of the photos/pictures
featured in those themes, please feel free to contact me,
so that you can get credited.

e-mail: unix121@protonmail.com
</ul>
