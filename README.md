
# Random obs action generator

This is a simple and very mission specific tool that sends random obs actions at a specified rate for as long as you want it to. Can be used for all kinds of stuff like stress-testing or reliability-testing obs.

Right now it can:
- Switch to a random scene
- Switch the preview to a random scene (if studio mode is enabled)
- Transition the preview scene to program (if studio mode is enabled)
- Toggle the visibility of a random scene item
- Switch to a random transition
- Toggle the mute status of a random input (this won't do anything if a specific input does not support audio)

### Requirements

- OBS 28 and up

### Setup 

- Start OBS, open the "Tools" menu and select "obs-websocket Settings"
- Make sure that "Enable Websocket server" is checked, "Server Port" is 4455
- Copy the websocket password(If "Enable Authentication" is enabled) for later by clicking on "Show Connect Info"-Button -> Next to the "Server Password" field -> "Copy"-Button
- [Download this repository](https://github.com/lebaston100/obsrantest/archive/master.zip) OR clone it (you only need the obsfun.html file)
- If you set a websocket password in OBS: Open the html file with a text editor and replace the "obsPassword" with your password where it says "// Set password here" and save the file

### Usage

- Open obsfun.html in a browser or as a custom obs browser dock
- With the slider on the top you can select the speed at which actions are executed. Be careful beause setting it to the fastest might/can crash obs!
- Click the start button to start the timer. Click the button again to stop.
- Enable and disable actions from the list. They can be enabled/disable anytime, even when running.
- "Status:" will show "Running!" if it's working on an action, otherwise "Sleeping"
- "Last ran action:" will show what the last action did

If you want to run the pages on another device in the network that is not the OBS Machine, then you can manually set the obs-pc ip by editing the "obsHost" variable in the line before the password configuration line.

The current UI features 100% UI, 0% UX.

If you have any problems, just open a Github issue or join my [Discord Server](https://discord.gg/PCYQJwX).