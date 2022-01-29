<table><tbody><tr><td><b>
<h1>BTE ASEAN TPLL RPA <img src="https://i.imgur.com/Qf3TC6w.gif" alt="_LOGO_" width="5%" height="5%" img align="Left"/></h1>
A tool to semi-automatically copy and paste tpll coordinates from Google Maps to Minecraft in a faster and efficient way.

<div align="Right"><sub>licensed by <a href="https://github.com/Codestian">Codestain</a><hr/>
</td></tr></tbody></table>
     
## 📑 requirements
- any kind of window 10/11 desktop
- chrome
- microsoft email *(`@hotmail.com` account)*
- [power automate desktop](https://powerautomate.microsoft.com/en-us/desktop/)
- *a willing to sign up and download external app*
---
## ⚠️ pre request
- **DO NOT** try to use this if you dont fit the requirement.
- this tool is client-side only, the bot could broke if you have very high ping in the server.
- <details><summary>why you should try this tool</summary>

     - build-the-earth manual tpll workflow for SEA country is painful and slow.
     - since its client side, you can use this tool anywhere(not just in this build team).
</details>

---
## 📥 What it contains 
The tool comprises of two components. To begin using the tool, download this repository and follow the installation instructions.

---
## :one:: Google Chrome Extension
Used to collate the tplls the end user has selected and exports them to a text file.

#### 📩 Installation

0. download this repository to your local desktop
1. Open Google Chrome and go to chrome://extensions/.
2. Ensure developer mode is on.
3. Click on the `Load unpacked` button and navigate to [your_desktop/bte-asean-rpa/extension](https://github.com/ASEAN-Build-The-Earth/bte-asean-rpa/tree/main/extension) folder.
4. The BTE extension should appear.
5. Go to [Google Maps](https://www.google.com/maps/) and click on the extension. You should see a light gray square.
6. Click on the square to start. The extension will collate the tplls when you right click a place and presses the coordinates to copy.
7. To ensure everything goes smoothly, press f12 to open the developer tools window and go to the console.
8. When a tpll has been successfully collated, a message will be logged.
9. To finish, click on the extension square again and a text file containing all the tplls collated will be automatically downloaded. Ensure you enable the multiple files download option.

NOTE: Try not to select more than 50 tpll points, since the extension is slightly unstable and you may lose the selected points. Do it slowly.

---
## :two:: Power Automate Flow

Reads the tplls from the text file generated by the Chrome extension and places a gold block on the coordinates.

#### 📩 Installation *(It is only supported on Windows 10 and 11)*

0. signup at [power automate website](https://powerautomate.microsoft.com/en-au/) and log in to the dashboard 
    - <details><summary>navigate to my flow tab</summary>

         > ![image](https://user-images.githubusercontent.com/77855014/151671546-260b8735-d972-41d9-83a1-e295a06e97d0.png)
    - <details><summary>Install Power Automate As Desktop</summary>
  
         > ![image](https://user-images.githubusercontent.com/77855014/151671572-17c9dde5-2690-4d97-ae20-60a8756e9dd3.png)
</details>
</details>

1. Open the Power Automate program on your computer. 
2. Create a new flow.
3. Pick preferred design in [bte-asean-rpa/power_automate](https://github.com/ASEAN-Build-The-Earth/bte-asean-rpa/tree/main/power_automate) and copy the `copy-me.yaml` file to the center of the empty space.    
    - <details><summary>each flow design have different instruction in its readme, so consider read it.</summary>

         > ![image](https://user-images.githubusercontent.com/77855014/151671851-b1a6285c-ad87-401e-adce-00cf7724773e.png)
</details>

4. The flow should be automatically created.
5. Whenever you would like to use the bot, look through the flow and ensure the `/tpll` elevation is set correctly in config line. It is recommended to set it to +1 of the ground 
6. By default, the bot uses the glass block to indicate a tpll point.
7. To run the bot, ensure your player character ingame is in creative mode and flying.
8. When the bot starts, you will be prompted to select the text file generated by the chrome extension.
9. Once you have selected it, immediately set the mouse focus to the minecraft window. Do not press `esc`. The bot will unpause the game by itself.
10. Grab a coffee and look at the bot doing your job for you. If it is not working as expected, just press stop in the Power Automate window and try again. ☕
---
