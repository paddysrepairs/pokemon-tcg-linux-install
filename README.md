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
<<img width="1920" height="1080" alt="Step_3_Download_Game" src="https://github.com/user-attachments/assets/61361d53-fc1f-4db6-9aad-4f943b296e28" />
</p>
<h2>Step 3, Download the Game Client!</h2>
<p>
Head on over to the Pokemon TCG Live site and download the client. Link below!
https://tcg.pokemon.com/en-us/tcgl/
</p>
<br />
<h2>Step 4, Add Game in Heroic!</h2>
<p>
<img width="1920" height="1080" alt="Step_4_Add_Game" src="https://github.com/user-attachments/assets/5b805362-7aa4-4b26-af98-ae4698dfb814"/>
</p>
Next we are going to go to the top left in Heroic and click "Add Game" the blue button as you can see pictured.
<br />
<h2>Step 5, Run Installer first in Heroic!</h2>
<p>
<img width="1920" height="1080" alt="Step_5_Installer_First" src="https://github.com/user-attachments/assets/384dc4ce-65b0-4d7a-b0c9-d90150dfb5de" />
</p>
Once we are into the "Add Game" section, we are going to fill out the required info for the game above. (You can add custom images at this point if you like. Then, we are going to run installer first and install the game client exacltly like you would on a Windows machine.
<h2>Step 6, Ignore installer </h2>
<p>
<img width="1920" height="1080" alt="Step_6_Installer_Errors_Yes" src="https://github.com/user-attachments/assets/74bd3e58-c99e-4927-a4f3-35d3faedb2e8" />
</p>
While running the installer you are going to run into some "vc_redist" errors. Just click "yes" as its fine to ignore these and continue the install. 
<br />
<h2>Step 7, Don't Run the Game Just Yet!</h2>
<p>
<img width="1920" height="1080" alt="Step_7_Installer_Dont_Run" src="https://github.com/user-attachments/assets/61355ba3-dc02-4443-a8fe-7749d3527bd5" />
</p>
Don't run the game just yet! Click the finish button and make sure launch game is not set launched.
<h2>Step 8, Go into Settings</h2>
<p>
<img width="1920" height="1080" alt="Step_8_Settings" src="https://github.com/user-attachments/assets/9fec9cf3-49be-4b4f-b056-0dde549507ac" />
</p>
Now that the game is installed, we want to right click on the "Pokemon TCG Live" game we just installed and go into its "Settings".
<h2>Step 9, Go into "Advanced Settings</h2>
<p>
<img width="1920" height="1080" alt="Step_9_Advanced_Settings" src="https://github.com/user-attachments/assets/3b24cc8c-70d9-46dd-8309-4cc9d131ccab" />
</p>
After going into settings, we want to find the "Advanced" tab.
</p>
</p><img width="3840" height="3760" alt="Step_9_Advanced_Settings_2" src="https://github.com/user-attachments/assets/48b71410-ea02-42dc-af20-e99f00cbdf26" />
</p>
We want to go into "Environment Variables" and add the following the "Variable Name" and "Variable" Tabs.
Variable Name= WINE_CPU_TOPOLOGY and Value= 2:0,1
These are important to make sure the game runs stable.
<br />
<h2>Step 10, Back to Wine Normal Settings</h2>
<p>
<img width="741" height="905" alt="Step_10_Back_to_Wine" src="https://github.com/user-attachments/assets/0005e6e5-4be7-40b2-b7a1-fdc8e693cf96" />
</p>
Once we are done with "Advanced Settings" we are going to go to "Wine" and scroll to the bottom.
<br />
<h2>Step 11, Open "Winetricks"</h2>
<p>
<img width="741" height="905" alt="Step_11_Winetricks" src="https://github.com/user-attachments/assets/d75a9ac4-6781-4532-89ed-b9d8184c2bfc" />
</p>
The next thing we want to access is "Winetricks" within Heroic Launcher! As highlighted, Click it to access the Wine layers.
<img width="1065" height="905" alt="Step_11_Winetricks_2" src="https://github.com/user-attachments/assets/2445e279-9e72-4854-8f49-261fad8f3397" />
Open the "Winetricks GUI" as shown.
<img width="1100" height="606" alt="Step_11_Winetricks_3" src="https://github.com/user-attachments/assets/01f2acaf-b6cf-4859-b22a-34023828db30" />
Select the "default prefix".
<img width="1100" height="606" alt="Step_11_Winetricks_4" src="https://github.com/user-attachments/assets/9fd9a104-361b-4023-88ba-3e600bc01e42" />
Next, run a "Wine CMD shell" as highlighted. THE NEXT STEPS ARE CRUCIAL TO GETTING THE GAME RUNNING.* Pay close attention, and be sure to leave the original command prompt you start here open until we are done.
<br />
<h2>Step 12, Find Original Directory of Install.</h2>
<p>
<img width="1920" height="1080" alt="Step_12_Copy_Directory" src="https://github.com/user-attachments/assets/be805420-f623-459d-a92b-571edc999b67" />
<p/>
Find where you installed the "Pokemon TCG Live" client. It should be in a similar location to what I have highlighted above under your "Home" directory.
<p>
<img width="534" height="362" alt="Step_12_Copy_Directory_2" src="https://github.com/user-attachments/assets/083c277b-18e5-4343-b5f8-6516f8bc32ae" />
</p>
type cd command to open a location like you would in Windows and middle click to paste the directory you just copied to the clipboard in your command shell! You must make sure that the directory has quotations copied at the start and finish of your pasted directory.* 
<h2>Step 13, Launch game through Wine CMD shell</h2>
<p>
<img width="726" height="512" alt="Step_13_Launch_Game" src="https://github.com/user-attachments/assets/cc4a3fda-3373-4d6c-9ce1-894ecef63704" />
</p>
From the location we just opened in Step 12. Type in quotations "Pokemon TCG Live.exe" to launch the game client.
<p>
<img width="1920" height="1080" alt="Step_13_Login" src="https://github.com/user-attachments/assets/91114073-20b4-452c-b754-9daafffb3c07" />
</p>
After we start the game client. It will prompt you to login into "Pokemon Trainer Central" in your default chosen browser.
