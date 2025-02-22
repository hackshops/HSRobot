# Getting Started with the HSRobot Kit

The HSRobot kit comes with everything needed to have fun, but needs a bit of elbow greese to get going.

The Raspberry Pi powering HSRobot has been configured to automatically setup a wireless Hotspot.  

NOTE: A software named `VNC Server` is already installed and configured to run on the Raspberry Pi. You will need to install the [`VNC Viewer`](https://www.realvnc.com/en/connect/download/combined/?lai_vid=qqx2bKKyXFJLv&lai_sr=10-14&lai_sl=l) software on your computer to be able to access HSRobot.

1. Ensure the battery is fully charged. Connect the USB cable from the battery to the Raspberry Pi's power port on HSRobot. When HSRobot is ready, the `green` LED next to the power port will stay lit and green.

2. Connect the 9V battery to the 9V connector on HSRobot. The `red` LED on the motor controller should turn on.

3. You will next connect your computer to the HSRobot's Hotspot.

4. On your computer, click the WiFi connection option and look for HSRobot's Hotspot. Click `Connect` and enter the password you set when you created the Hotspot. 

    ![WiFI List](https://github.com/hackshops/HSRobot/blob/main/images/WiFiList.png)

    ![HSRobot WiFi Password](https://github.com/hackshops/HSRobot/blob/main/images/HSRobotHotspotWiFiPassword.png)

5. After your computer connects to the Hotspot, we need to connect to it using the VNC Viewer software. Launch VNC Viewer on your computer. After the software is launched and read, we need to setup a new connection to HSRobot. Select `File -> New Connection...` from VNC Viewer's main menu.

    ![HSRobot New VNC Connection](https://github.com/hackshops/HSRobot/blob/main/images/VNCNewConnection.png)

6. This should bring up the screen shown below.

    ![HSRobot VNC Configure Connection](https://github.com/hackshops/HSRobot/blob/main/images/VNCConfigureConnection.png)

7. Enter the IP Address of HSRobot. This should be `10.99.50.1`. The last 3 numbers should match the HSRobot number. If your HSRobot is 501, then set this value to `50.1`. This is just a convention. If you have manually setup a new hotspot, ensure you enter the correct IP Address.

8. Enter a `Name` for the connection. And Click OK. Your VNC Viewer screen should look something like the screen below.

    ![HSRobot VNC Connections](https://github.com/hackshops/HSRobot/blob/main/images/VNCWithConfigs.png)

9. To connect to HSRobot, click the connection for HSRobot on the VNC Viewer's main menu. Your screen should look something like the screen below.

    ![HSRobot VNC Credentials](https://github.com/hackshops/HSRobot/blob/main/images/VNCConnectToPi.png)

10. Enter the password for HSRobot and click `OK`. Your screen should look something like the screen below.

    ![HSRobot Home Screen](https://github.com/hackshops/HSRobot/blob/main/images/PiHomeScreen.png)

11. Next, let's test HSRobot using the pre-loaded Scratch program. On the desktop screen you should see an item with the name `Robot.sb3`. This is a sample scratch program that'll run on HSRobot.

12. Let's launch Scratch programming software. From the Raspberry Pi icon on the top left, select `Programming` and then `Scratch 3`.

    ![HSRobot Scratch](https://github.com/hackshops/HSRobot/blob/main/images/PiScratch3Menu.png)

13. This should bring up the Scratch programming software similar to the screen below.

    ![HSRobot Scratch Home](https://github.com/hackshops/HSRobot/blob/main/images/Scratch3HomePage.png)

14. To run the Scratch program, select `File -> Load from your computer` and navigate to the `Robot.sb3` file on your desktop. This should bring up the screen similar to the screen below.

    ![HSRobot Scratch Load](https://github.com/hackshops/HSRobot/blob/main/images/PiLoadFromComputer.png)

15. After the program loads your screen should look something like the screen below.

    ![HSRobot Program](https://github.com/hackshops/HSRobot/blob/main/images/HSRobotProgram.png)

16. If you see the yellow block with the title `When Flag clicked` you are all set and ready to test HSRobot. Make sure HSRobot is firmly on the ground and has no obstructions. Click the green flag to run the program. HSRobot should move forward, stop for 5 seconds, move back and finally come to a stop. 

## What to do if the yellow block with the title `When Flag clicked` is not setup?

1. On the left side of the Scratch 3 programming software, you should see a yellow circle named `Events`. Click the Events block.  

    ![HSRobot Scratch Events](https://github.com/hackshops/HSRobot/blob/main/images/PiControlBlocks.png)

2. Select the `When Flag clicked` option and drag it to the empty white space in the middle. 

3. Next click the pink colored `My Blocks` option on the left to list the pre-configured blocks that setup HSRobot.

    ![HSRobot Scratch My Blocks](https://github.com/hackshops/HSRobot/blob/main/images/PiMyBlocks.png)

4. Select the `Move Forward` block and drag it to the empty white space and attach it below the `When Flag clicked` block.

5. Click the yellow `Control` circle and drag the `wait 1 seconds` block and attach it below the `Move Forward` block. Change `1` to `5` by clicking inide the circle.

6. Next click the pink colored `My Blocks` option on the left to list the pre-configured blocks that setup HSRobot. Select the `Move Reverse` block and drag it to the empty white space and attach it below the `wait 5 seconds` block.

7. Click the yellow `Control` circle and drag the `wait 1 seconds` block and attach it below the `Move Reverse` block. Change `1` to `5` by clicking inide the circle.

8. Next click the pink colored `My Blocks` option on the left to list the pre-configured blocks that setup HSRobot. Select the `Stop` block and drag it to the empty white space and attach it below the second `wait 5 seconds` block.

9. Click the green flag to run the program. HSRobot should move forward, stop for 5 seconds, move back and finally come to a stop.
