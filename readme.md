


<h1> Arcade1Up Rasperry Pi Mod collection , tips , tricks and more! </h1> 


  
  A collection of a few things that are helpful for modding an Arcade1Up cabinet. 






<h2> Emulation / ES Theme </h2>
https://github.com/djdarien/arcade1up-rpi-easy-setup/blob/main/es-theme-super-arcade1up-5x4-master.zip
  Emulation Station theme is for 5x4 horizontal (Asteroids , Street Fighter, etc)


<h2>  Use Original power buttons & volume slider </h2>
<h3> Power switch</h3>
Connect the black wire to Pin 5 (GPIO3) & the red wire to Pin 6 (Ground) of the GPIO header

<h3> Volume switch </h3>
Connect the brown wire to Pin 7 (GPIO4), red wire to Pin 9 (Ground) & the black wire to Pin 11 (GPIO17) of the GPIO header.

You will need to connect to your Pi from a terminal (Putty on Windows) and run the below command:

bash <(curl -s https://raw.githubusercontent.com/orlandovald/arcade1up/master/setup.sh)
This is what the script will do,

Install all required dependencies (python libraries and Git)
Clone this repo to get the python, bash and other scripts
It will prompt if you want to configure the Power switch, press 'Y' or 'y' to configure. Skip with any other key.
It will prompt if you want to configure the Volume switch, press 'Y' or 'y' to configure. Skip with any other key.
It will prompt if you want to configure the Power relay, press 'Y' or 'y' to configure. Skip with any other key.
You skipped one by mistake? No worries, you can re-run the command. The script will automatically skip anything that has been already configured.

Pin configuration
After installation you should make any neccesary updates to the default configuration which can be found in the /home/pi/arcade1up/config/config.ini file.

You can see the default values for config/config.ini , view them over here >> https://github.com/orlandovald/arcade1up/blob/master/config/config.ini

Info and more at: https://github.com/orlandovald/arcade1up


<h2> PI 4 images from Arcade Punks.com </h2>
https://www.arcadepunks.com/download-raspberry-pi-4-images/

<h2>  Hide console output on boot  </h2>
Edit cmdline.text located at /boot/cmdline.text and change it to console=tty3

<h2> Hide Raspbery Pi Logo on boot </h2>
Also at cmdline.text located /boot/cmdline.text and add logo.nologo

<h2> Vertical Screen setup (For Pac-Man, Galaga cabs,etc) </h2>
Edit and change config.txt located at /boot/config.txt and copy/replace to display_rotate=3
