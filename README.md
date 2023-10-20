# dinaterm
A fully functional terminal app to run on Dina or any other browser.

DinaTerm is a slightly modified of pyxterm.js https://github.com/cs01/pyxtermjs.

The app runs on localhost, port 5001. 

The included shell script is provided for convenience. Call the script to start the app. Use the argument --stop to kill it. It is not advised to stop the script while running commands in the terminal. A warning is shown with the help of yad dialog https://github.com/v1cont/yad to prevent coincidental undesired actions. Install yad to use this feature. 

DinaTerm was developed to be an extension for Dina Browser - https://github.com/IonTeLOS/Dina.

Dina is a minimal browser built with tauri and Pake and uses the WebKit rendering engine. 

The installation of Dina is suggested but not required to use DinaTerm.

Launch dinaterm with the --browser foo argument to use your foo browser to show DinaTerm

You can launch DinaTerm in fullscreen using the --fullscreen argument. This option is available only in Dina Browser.

Pake and pyxterm.js are credited external projects with their own licenses. Learn more about Pake at https://github.com/tw93/Pake. 

To run DinaTerm, create a Python virtual environment, install the requirements and run dinaterm shell script from inside the virtual environment and from the same folder.

Create an executable of DinaTerm: first create a Python virtual environment, install the requirements and run: 

pyinstaller --add-data "index.html:." --clean --onefile dina-term.py --name dina-term

A ready-made executable of DinaTerm is provided in the Releases. The .deb package in the Releases downloads dina-term executable during installation.

The icons used are Google material icons, the fonts are JetBrains Mono.

To add the repository and install DinaTerm :

wget -qO - https://iontelos.github.io/appy/KEY.gpg | sudo gpg --dearmor -o /usr/share/keyrings/appy.gpg

sudo curl -s --compressed -o /etc/apt/sources.list.d/telos.list "https://iontelos.github.io/appy/telos.list"

sudo apt clean

sudo apt update

sudo apt install dinaterm

DinaTerm and Dina run on Linux._
