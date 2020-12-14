# unDEV

<h1 align="center">Hey there! 👋</h1>
<h3 align="center">That's my personal unRAID edit! You can use it, but this repo is new... So don't be mad if some files are missing.</h3>

- 🔭 Soon there will be an installation guid for you!

🛠️ Installation

Recommended way:

Install using the bash script and the plugin CA User Scripts

Add a new user script by clicking Add new script

Give it a name and click OK

Click or hover over the gear icon and click Edit Script

Paste the contents of the bash script: custom_login.sh

Below the shebang(#!/bin/bash) are the variables you need to change for the different themes.

The default values are the ones below

TYPE="retro-terminal"
THEME="green.css"
DOMAIN="gilbn.github.io"
ADD_JS="true"
JS="custom_text_header.js"
DISABLE_THEME="false"

Available theme colors.

See screenshots at the bottom.

amber.css
red.css
green.css
blue.css
white.css
custom.css

Set the values to what you like, and click Save Changes

To have the script applied at every boot, set the schedule to At Startup of Array

Now just click Run Script and it will print some text in the window.

Thats it.. logout and have a look at your new theme :)
Javascript:

You can also inject an animated <pre> tag with javascript for that ultimate alien feel 👽

Set ADD_JSto "true" to enable or "false" to omit the javascript.

⚠️⚠️⚠️

HEY! You are injecting javascript into the login page for your precious server!

You should probably have a look at the content of that file, and probably host it yourself 💀

custom_text_header.js

⚠️⚠️⚠️

FAQ
Backups

The script will create a backup of the login.php file if one does not exist.
Uninstall/Restore the original

To uninstall the theme set the variable DISABLE_THEME to "true"
Can I selfhost this?

Of course! Just clone the repo into your webserver. Remember to change the DOMAIN variable in the bash script.
My server is not connected to the internet! How can I add this?

With the current version of the bash script, that is not possible as it injects the stylesheet using the a URL and not a file path. However, nothing is stopping you from just doing some small changes to the script and replace the href urls to the path you stored the files. I will try and create a version of the script that is made for local hosting in the future.
:rage4: I hate the flickering!! :rage4:

To remove the background flickering you need to edit the css file. Now since you don't have any control over those files, you'll need to fork it and setup Github pages or selfhost them. You can't use the raw link from Github, as they don't pass the mime types.

The background flickering can be disabled by setting the --body-animation root variable to none

The <pre> tag flicker can be disabled by setting --custom-text-header-animation to none.
:rage4: I hate the CRT lines!! :rage4:

Set the --body-before and --body-after root variables to none
:rage4: I want my own logo!! :rage4:

Fork it and change the --logo variable or if you're using stylus ect, just add a new --logo root variable below the import line.

@import url(https://gilbn.github.io/theme.park/CSS/addons/unraid/login-page/retro-terminal/red.css);
:root {
--logo: url(https://domain.com/your-snowflake-logo-here.png) center no-repeat;
}

Available CSS variables:

:root {
--main-bg-color:black;
--body-before:#00ff771a;
--body-after: #00ff7733;
--body-animation: flicker;
--logo: url(https://gilbn.github.io/theme.park/CSS/addons/unraid/login-page/alien/logo/wings_green.png) center no-repeat;
--text-color: #37f592;
--input-color: #37f592;
--link-color: #37f592;
--link-color-hover: #68ffff;
--case-color: #37f592;
--button-text-color: #37f592;
--button-text-color-hover: #000;
--button-color: #37f592;
--button-color-hover: #68ffff;
--selection-color: #68ffff;
--custom-text-header:#37f592;
--custom-text-header-shadow:#37f592;
--custom-text-header-animation: textflicker;
--input-font: 'Share Tech Mono', monospace;
--text-font: 'Share Tech Mono', monospace;
--loginbox-background-color: transparent;
--text-shadow: 0 0 8px;
--text-shadow-color: #37f592;
--box-shadow: 0 0 15px;
}

- 📫 How to reach me **felbeeey@gmx.net**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://twitter.com/felbeeey" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/twitter.svg" alt="felbeeey" height="30" width="40" /></a>
<a href="https://instagram.com/felbeeey" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg" alt="felbeeey" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/felbeeey" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/youtube.svg" alt="felbeeey" height="30" width="40" /></a>
<a href="https://discord.gg/https://discord.gg/Vf8gWQQv" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/discord.svg" alt="https://discord.gg/Vf8gWQQv" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://developer.android.com" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/android/android-original-wordmark.svg" alt="android" width="40" height="40"/> </a> <a href="https://angular.io" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/angularjs/angularjs-original.svg" alt="angularjs" width="40" height="40"/> </a> <a href="https://azure.microsoft.com/en-in/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/microsoft_azure/microsoft_azure-icon.svg" alt="azure" width="40" height="40"/> </a> <a href="https://www.gnu.org/software/bash/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/gnu_bash/gnu_bash-icon.svg" alt="bash" width="40" height="40"/> </a> <a href="https://www.blender.org/" target="_blank"> <img src="https://download.blender.org/branding/community/blender_community_badge_white.svg" alt="blender" width="40" height="40"/> </a> <a href="https://getbootstrap.com" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/bootstrap/bootstrap-plain.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cs/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/csharp/csharp-original.svg" alt="csharp" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.docker.com/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://www.framer.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/framer/framer-icon.svg" alt="framer" width="40" height="40"/> </a> <a href="https://cloud.google.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://grafana.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/grafana/grafana-icon.svg" alt="grafana" width="40" height="40"/> </a> <a href="https://graphql.org" target="_blank"> <img src="https://www.vectorlogo.zone/logos/graphql/graphql-icon.svg" alt="graphql" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.adobe.com/in/products/illustrator.html" target="_blank"> <img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" alt="illustrator" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/java/java-original-wordmark.svg" alt="java" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://kafka.apache.org/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/apache_kafka/apache_kafka-icon.svg" alt="kafka" width="40" height="40"/> </a> <a href="https://www.elastic.co/kibana" target="_blank"> <img src="https://www.vectorlogo.zone/logos/elasticco_kibana/elasticco_kibana-icon.svg" alt="kibana" width="40" height="40"/> </a> <a href="https://kotlinlang.org" target="_blank"> <img src="https://www.vectorlogo.zone/logos/kotlinlang/kotlinlang-icon.svg" alt="kotlin" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://mariadb.org/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/mariadb/mariadb-icon.svg" alt="mariadb" width="40" height="40"/> </a> <a href="https://www.mathworks.com/" target="_blank"> <img src="https://raw.githubusercontent.com/simple-icons/simple-icons/master/icons/mathworks.svg" alt="matlab" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://www.nginx.com" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/nginx/nginx-original.svg" alt="nginx" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://www.oracle.com/" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/oracle/oracle-original.svg" alt="oracle" width="40" height="40"/> </a> <a href="https://www.photoshop.com/en" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/photoshop/photoshop-plain.svg" alt="photoshop" width="40" height="40"/> </a> <a href="https://www.php.net" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/php/php-original.svg" alt="php" width="40" height="40"/> </a> <a href="https://www.postgresql.org" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank"> <img src="https://devicons.github.io/devicon/devicon.git/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://www.qt.io/" target="_blank"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/0b/Qt_logo_2016.svg" alt="qt" width="40" height="40"/> </a> <a href="https://www.sketch.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/sketchapp/sketchapp-icon.svg" alt="sketch" width="40" height="40"/> </a> <a href="https://www.sqlite.org/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/sqlite/sqlite-icon.svg" alt="sqlite" width="40" height="40"/> </a> <a href="https://unity.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/unity3d/unity3d-icon.svg" alt="unity" width="40" height="40"/> </a> <a href="https://unrealengine.com/" target="_blank"> <img src="https://raw.githubusercontent.com/kenangundogan/fontisto/036b7eca71aab1bef8e6a0518f7329f13ed62f6b/icons/svg/brand/unreal-engine.svg" alt="unreal" width="40" height="40"/> </a> <a href="https://www.adobe.com/products/xd.html" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/adobe-xd.svg" alt="xd" width="40" height="40"/> </a> </p>

<h3 align="left">Support:</h3>
<p><a href="https://www.paypal.me/dominicfelber"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="felbeeey" /></a></p><br><br>
