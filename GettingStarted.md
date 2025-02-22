# Getting Started with the HSRobot Kit

The HSRobot kit comes with everything needed to have fun, but needs a bit of elbow greese to get going.

The Raspberry Pi powering HSRobot has been configured to automatically setup a wireless Hotspot. 


Once the Raspberry Pi is powered on, the HSRobot kit is ready to go! A software named `VNC Server` is already installed and configured to run on the Raspberry Pi. You will need to install the [`VNC Viewer`](https://www.realvnc.com/en/connect/download/combined/?lai_vid=qqx2bKKyXFJLv&lai_sr=10-14&lai_sl=l) software on your computer to be able to access HSRobot. 

## How to setup a wireless Hotspot on HSRobot

You will need to connect HSRobot to a network (wired or wireless) that your computer is connected to so you can use the VNC Viewer software from your computer to access HSRobot. Alternatively, you can connect HSRobot to a monitor, keyboard and mouse and directly access HSRobot.

1. Power on the Raspberry Pi
2. Access the Setup New Connection menu available on the top right corner area of the screen.

    ![HSRobot Connection Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotCreateMenu.png)

3. Select the `Create Wi-Fi Hotspot` option.

    ![HSRobot Create Hotspot Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotCreateNew0.png)

4. Enter a name for the Hotspot, select the WiFi security type, add a password and select the `Create` option.

    ![HSRobot Create Hotspot Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotCreateNew.png)

5. The Hotspot is now created. Before you can successfully connect to it, you'll need to configure a few additional settings to ensure the hotspot setup is permanent. Access the menu again and select `Edit Connections...` option.

    ![HSRobot Connection Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotCreateMenu.png)

6. This should bring up the screen shown below.

    ![HSRobot Connection Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotConfig.png)

7. You should see the newly created Hotspot listed on the screen. Select the Hotsopt and click the `gear` icon at the bottom of the screen. This should bring up the screen shown below.

    ![HSRobot Connection Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotWifiAssignToMacAddr.png)

8. In the `Device` dropdown option make sure you select `wlan0` with the MAC address. 
9. Next, let's make the hotspot permanent. Select the `General` tab and check the option `Connect automatically with priority` as shown below.

    ![HSRobot Connection Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotAutoConnectConfig.png)

10. Next, let's assign a known IP address to HSRobot so you can easily remember the IP Address to connect to. Select the `IPV4 Settings` tab. Click the 'Add' button on the left and set the IP address to `10.99.50.1`. NOTE: The last 3 numbers after `10.99.` should match the HSRobot number. If your HSRobot is 501, then set this value to `50.1`. This is just a convention.

    ![HSRobot Connection Menu](https://github.com/hackshops/HSRobot/blob/main/images/HotspotIPAddressConfig.png)

11. Click the `Save` button.

12. Restart HSRobot and you should be able to connect to the Hotspot using the hotspot name and password you set.

