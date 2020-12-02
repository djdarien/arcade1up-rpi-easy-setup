


<h1> Arcade1Up Rasperry Pi Mod collection , tips , tricks and more! </h1> 


  
  A collection of a few things that are helpful for modding an Arcade1Up cabinet. 






Emulation Station theme is for 5x4 horizontal (Asteroids , Street Fighter, etc)






<h2>  Use Original power buttons & volume slider </h2>
<h3> Power switch</h3>
Connect the black wire to Pin 5 (GPIO3) & the red wire to Pin 6 (Ground) of the GPIO header

<h3> Volume switch </h3>
Connect the brown wire to Pin 7 (GPIO4), red wire to Pin 9 (Ground) & the black wire to Pin 11 (GPIO17) of the GPIO header.
<br></br>
You will need to connect to your Pi from a terminal (Putty on Windows) and run the below command:
<br></br>
*git clone https://github.com/dmanlfc/arcade1up.git

Info and more at: https://github.com/orlandovald/arcade1up


<h2> PI 4 images from Arcade Punks.com </h2>
https://www.arcadepunks.com/download-raspberry-pi-4-images/

<h2>  Hide console output on boot  </h2>
Edit cmdline.text located at /boot/cmdline.text and change it to console=tty3

<h2> Hide Raspbery Pi Logo on boot </h2>
Also at cmdline.text located /boot/cmdline.text and add logo.nologo
