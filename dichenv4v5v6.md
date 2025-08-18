# Dichen v4

More coming soon, firmware and tools in the releases

## Firmware flashing steps

What to prepare

A Main PC (Gaming PC) with an HDMI port, capable of outputting the required resolution and refresh rate.
A Second PC (Cheat PC) with an HDMI port, capable of outputting the required resolution and refresh rate.
3 HDMI cables, capable of outputting the required resolution and refresh rate.
Before diving into the official installation tutorial, there are some essential information that you need to be aware of.
The resolution inputted in the fuser must be same. (The refresh rate can be different)
For example, if the main PC inputs 1080p 240Hz and the second PC inputs 1080p 60Hz, the output result will cause the ESP rendering overlay to run at only 60fps. As a result, the ESP rendering overlay will appear laggy.
​
### Setup

> All actions here should be done on Main PC (Gaming PC) !!!
Use an HDMI cable to connect the Main PC (Gaming PC) and the Main Monitor.
Right Click on your desktop and click Display Settings.

Change to your desired solutions and hz (Recommend set to max settings of your monitor). For example, if you like to use fuser at 1080p240hz, set display to 1080p + 240hz.

### Extracting .bin (EDID File).

Download Monitor Asset Manager Setup.exe and save it wherever you’d like.
Run Monitor Asset Manager Setup.exe and complete the installaion.
If it doesn’t auto-launch after install then search for Moninfo in your Windows Search Bar and run it as Administrator.
Make sure Real-time is selected.

### Setup Fuser
Conenct the power cable provided with the box to the fuser and turn on the power.

You should see the first light “D1” turn on (if it doesn’t turn on press the big red power button)

Connect the data cable & Install the driver
All actions should complete on Main PC (Gaming PC) !!!
Grab your USB-C to USB-A cable.
Plug in USB-C end to your fuser; USB-A end into your Main PC (Gaming PC).

Search Device Manager in your windows search bar and open it.

It should look like this under Ports (COM & LPT). If it does, skip to the next big step. If it doesn’t, continue to Step 7.

If it doesn’t and show as USB Serial, complete Driver Install.

### Install Driver
CH340 Driver
CH340 Driver for Kmbox
Download the CH340 Driver from above.
Extract the folder and open the extracted folder.
Right click the CH341SER.EXE and click Run as Administrator.

Click INSTALL and then OK.

Now go back to Device Manager and you should see your fuser show up under Ports (COM & LPT)
Take note of the COM port it’s on. For example, mine’s on COM3 (if you have multiple COM ports showing, just unplug your fuser and see which one dissapears, then re-plug it in)

​
### Inject EDID

EDID Injector
Dichen EDID Injector
Download EDID Injector from above.
Save it wherever you’d like and right click it and click Run as Administrator.

Select the correct COM port.
Select your desired resolution. For example, I want 1920x1080.
Click that button (it’s the automatic easier injection).
Click that button to browse your files and select the .bin you saved earlier.
Click that button to inject.

You’ll see some random characters pop up, that’s fine. Close the dialog boxes and you can close all previously used applications and windows
Unplug your USB-C to USB-A cable from the Main PC.
​
# Wire Configuration

There are 3 Ports on the fuser. Grab your 3 HDMI cables and plug them in as follows:
HDMI goes to the Main Monitor.
HDMI1 goes to Main PC (Gaming PC).
HDMI2 goes to second PC (Gaming PC).

Once everything is plugged in, all lights should be on.
​
# Indicators

D1 - Power indicator. If the light is on it has power
D2 - Fusing/Overlay status. If the light is on it means the fuser is overlaying the second PC’s output
H2 - Second PC input status. If the light is on then it means the fuser is getting a signal from the second PC.
H1 - Main PC input status. If the light is on then it means the fuser is getting a signal from the main PC.

Each button has a function:
K1 - Press it once: cycle through resolutions. It should default on 1080p. Press the button to cycle until you reach your desired resolution. Press and hold: Show current input information like resolution and refresh rate.
K2 - Increase the fusing strength/tolerance. The higher it goes, the more of the gray it will delete during fusing.
K3 - Resets the fusing strength/tolerance to default. This is what I use. It works nicely for every cheat I’ve tried.
K4 - Toggle fusing/overlay.

​
## Debugging

​
Multiple Monitors

If you want, you can plug in multiple monitors to your second PC. For the easiest usage:
Use Case
Some DMA software uses Client Mode (menu and radar integrated into one software), and this type of product is best used with a Second PC (Cheat PC) outputting two HDMI connections.
Users who want a dedicated screen for viewing the radar. (Users can also access the radar directly on their other devices within the same local network.)
Importants
Your Second PC (Cheat PC) must have atleast two video output i/o (HDMI / DP) and a Second Monitor.
Some products have a monitor selection option, so you can directly using that settings without this setup.
First, your second PC (Cheat PC) should have two HDMI ports, each connected to:
Fuser
Second Monitor
On your Second PC (Cheat PC), go to Display Settings, and you should see two monitors appearing in the settings.

Choose the screen that outputs the display to the fuser. To identify it, click the Identify button, and a number should appear in the bottom left corner of each monitor.

Select the Fuser Output Monitor, tick Make this my main display.

Setup is now complete. When running the DMA Software, the Main Display should default to showing ESP and Wallhack. Drag the Radar Client windows to the second monitor, and it will work perfectly.
​
Reset the Fuser

If you want to reset the fuser back to factory setting (you might do this if your EDID isn’t working and you’ve exhausted all options), just plug the fuser back in via the USB-C to USB-A cable and do this:
Select the correct COM port.
Select the desired resolution.
Click the third button.


