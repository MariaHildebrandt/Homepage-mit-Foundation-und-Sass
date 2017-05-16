# Website für Cloud Anbieter
Website für Cloud-Storage- und Backup Anbieter, Sceenshots vorhanden

## Verwendet
- [Foundation](http://foundation.zurb.com/)
- [Sass](http://foundation.zurb.com/sites/docs/v/5.5.3/sass.html)
- [Font Awesome](http://fontawesome.io/)
- [NodeJS](https://nodejs.org/en/) 
- [Lizenzfreie Bilder von Pexels.com](https://nodejs.org/en/) 
- [Google Fonts](https://fonts.google.com/)

## Voraussetzungen

- [NodeJS](https://nodejs.org/en/) 
- [Git](https://git-scm.com/)


## Manual Setup

1.Download mit Git:

```bash
git clone https://github.com/MariaHildebrandt/Website-fuer-Cloud-Anbieter projectname
```
2.Ordner in command line öffnen und dependencies installieren:

```bash
cd projectname
npm install
bower install
```

3. `npm start` 
- um Sass compiler zu starten
- 'projectname' auf Default-Port: 3000 bzw: http://127.0.0.1:3000/

## Screenshots

#### Vollansicht:
<p>
  <a href="https://postimg.org/image/c0a70uyan/">Home</a>,
  <a href="https://postimg.org/image/97gzgtxy7/">Features</a>,
  <a href="https://postimg.org/image/6stpa5733/">Modelle</a>
</p>


#### Vorschau:
<p align="left">
  <img src="https://s19.postimg.org/wkf0zce1v/home.png"/  width="280">
  <img src="https://s19.postimg.org/72wmfqwbn/features.png"/  width="280">
  <img src="https://s19.postimg.org/jk7vgngv7/modelle.png"/  width="280">
</p>


## How to recreate environment
- 1.install Node.js from node homepage by downloading and opening the msi file
- 2.create new folder for your project. open this folder vith git bash
- 3. install foundation with command: "npm install --global foundation-cli"  or whatever command is advised in the documentation on the homepage
- 4.once the installation has finished (about 3 min) command: "foundation new" and chose what you want to build. this will create a new folder in your project folder with the title you chose
- 5. download and install atom (code editor). in atom goto datei->settings. search for atom-live-server and install (by jas-chen). then you can go to packges->live-server and open in a port of you like
- 6.Open folder "hosting" (thats the name of the folder that you created with the command foundation new) and start server with packages->atom-live-> start server. This will open a Welcome to Foundation website in your standard browser
- 7.in git bash cd hosting (leads you into folder hosting) and then: foundation watch
- this will compile all foundation css files into one file and include the stylesheet reference into index.html 
- this will also reload the welcome to foundation website. now the site contains css design
- 8.Install FontAwesome
- download font-aweseom.zip from homepage
- entpacke gesamten font folder in den hauptpfad (selbe ebene wie ordner css, index.html)
- entpacke aus css\fon.aweseome.min.css und hinterlege die datei im scss folder
- benenne die datei in "_bezeichnung.scss" um
- in app.scss schreibe @import 'bezeichnung';
- schliesslich mit strg+c beende den laufenen foundation watch im git bash und starte foundation watch neu. 
- nun sollten die icons zu sehen sein

### notes on how to use SASS
- you can create a new css stylesheet by creating a new file in scss and call it : "_custom.scss"
- in app.scss write : @import 'custom';
- this will include the custom stylesheet into css/app.css

- in  _settings.scss you can change
- $topbar-padding: 1.5rem; to whatever you like (about ~line 610)
- in line 49 define own variables vor css
- can look like this: 
```bash
@import 'util/util';

//custom variables
$primary: #0f74a0;
$secondary: #9bc33f;

$global-font-size: 100%;
$global-width: rem-calc(1200);
$global-lineheight: 1.5;
$foundation-palette: (
  primary: $primary,
  secondary: $secondary,
  success: #3adb76,
  warning: #ffae00,
  alert: #cc4b37,
);
```

- and you can use costum variables in _costum.scss
```bash
.top-nav{
  width:100%;
  background:$dark-gray;
  padding: 0;
  margin: 0;
}
```


