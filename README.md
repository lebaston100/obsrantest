
# Random obs action generator

This is a simple and very mission specific tool that sends random obs actions at a specified rate until you stop it. Can be used for all kinds of stuff like stress-testing or reliability-testing obs.

Right now it can:
- Switch to a random scene
- Switch the preview to a random scene if studio mode is enabled
- Transition the preview scene to program
- Toggle the visibility of a random scene item
- Switch to a random transition

### Requirements

- The [obs-websocket plugin](https://github.com/Palakis/obs-websocket/releases/tag/4.9.1) (only version 4.9.1)
- An internet connection

### Setup obs-websocket

- Download the obs-websocket installer and run it or use the zip file for a manual install
- Start OBS, open the "Tools" menu and select "websocket server settings"
- Make sure that "Enable Websocket server" is checked, "Server Port" is 4444
- If you want/need to, you can also set a password if you are running in an untrusted network

### Setup for this

-  [Download this repository](https://github.com/lebaston100/obsrantest/archive/master.zip) OR clone it (you only need the obsfun.html file)
- Additionally if you set a password in obs-websocket: Open the html file with a text editor and replace the "mypassword" with your password where it says "// Set password here" and save the file
- Open obsfun.html in a browser or as a custom obs browser dock

### Usage
- With the slider on the top you can select the speed at which actions are executed. Be careful beause setting it to the fastest might/can crash obs!
- Click the start button to start the timer. Click the button again to stop.
- Enable and disable actions from the list. They can be enabled/disable anytime, even when running.
- "Status:" will show "GO!" if it's sending an action, otherwise "Sleeping"
- "Last ran action:" will show what the last action did

If you want to run the pages on another device in the network that is not the obs-pc, then you can manually set the obs-pc ip by editing the variable in the line before the password configuration line.

And please don't bother me about the non-existing UI unless you have a PR ;)

If you have any problems, just open a Github issue or join my [Discord Server](https://discord.gg/PCYQJwX).