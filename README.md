# Pokemon TCG LINUX Install
An overview on how to get Pokemon TCG live on Linux.<p align="center">
<img src="https://d1i787aglh9bmb.cloudfront.net/assets/img/tcgl/logos/en-us/logo.png"/>
<img width="560" height="303" alt="Linux_Logo_Small" src="https://github.com/user-attachments/assets/08f883dd-09db-4f64-80ac-6e11fbca636e" />
</p>

<h1>Forwarding the TCG live client through Heroic Launcher on Linux Nobara</h1>
This tutorial outlines how to forward the Windows Client for Pokemon TCG Live through a compatibility launcher called "Heroic Game Launcher" to get the game running on Linux operating systems. .<br />

<h2>Video Demonstration</h2>

https://www.youtube.com/watch?v=sLdnG7Roxls&t=129s

<h2>Environments and Technologies Used</h2>

- Linux Nobara 44 (Fork of Fedora)
- Heroic Games Launcher
- Wine/ Winetricks (Windows Wine Command Launcher)
- Terminal/ Konsole
- Proton Compatability Layers

<h2>Operating Systems Used </h2>

- Linux Nobara 44

<h2>Total Step Index</h2>

- Step 1 Flathub Install
- Step 2 Download the TCG Live MSI client
- Step 3 Launch Heroic Launcher
- Step 4 Add "New Game" on Heroic
- Step 5 "Run Installer First" on Heroic
- Step 6 Live Installer Errors, Just click "yes".
- Step 7 Don't run Live just yet.
- Step 8 Go into Live Settings for the game you just added.
- Step 9 Click "Advanced Settings"
- Step 10 Back to Wine and go into Winetricks.
- Step 11 Go into Winetricks Gui and run Wine CMD Shell.
- Step 12 Find TCG Live directory you installed and copy location link.
- Step 13 Launch game, login with Live creds.
- Step 14 F12, Copy "callback" in console line on browser. Relaunch game with command, Paste in OG CMD shell callback line.
- Step 15 Game successfully launched! Have fun. 

<h2>Configuration Steps</h2>
<h2>Step 1 Heroic Install (Flathub distro Dependent)</h2>
<p>
<<img width="1920" height="1080" alt="Step_1_Flathub_Install_Konsole" src="https://github.com/user-attachments/assets/928cbb9b-ce82-43f8-a9f9-c6e537e967e0" />
<img width="1920" height="1080" alt="Step_1_Flathub_Install_Konsole_2" src="https://github.com/user-attachments/assets/3aef3ec8-1ea0-4c00-b09f-d159561b8e48" />
</p>
<p>
I highly encourage anyone who is on Nobara 44 to just use Heroic Launcher that seems to be packaged with the distro upon install.*
If you happen to need to install Heroic. You may need to install Flathub or Flatpost versions to install the game. (Distro dependent) the example shown is one method of installing the Heroic Launcher app.
</p>
<br />
<h2>Step 2 Launch Heroic Launcher</h2>
<p>
<<img width="873" height="556" alt="Step_2_Launch_Heroic" src="https://github.com/user-attachments/assets/6558b033-10ad-4313-b3cf-68eabfa3a2d7" />
</p>
<p>
Once Heroic is sorted out, lauch the app via the konsole or by the shortcut created in the application launcher or by the one you may have created on your desktop.
</p>
<br />
<p>
<<img width="1920" height="1080" alt="Step_3_Download_Game" src="https://github.com/user-attachments/assets/61361d53-fc1f-4db6-9aad-4f943b296e28" />
</p>
<p>
Head on over to the Pokemon TCG Live site and download the client. Link below!
https://tcg.pokemon.com/en-us/tcgl/
</p>
<br />
